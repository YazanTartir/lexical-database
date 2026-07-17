# Lexical Database Schema

## Core Objects & Definitions

- Concept
- Lexeme
- Word Form
- Root
- Relation
- Vocabulary Set
- Tag

## Supported Languages

- English
- Spanish
- Arabic

## Parts of Speech

- Noun
- Verb
- Adjective
- Adverb
- Phrase
- Expression

## Design Principles

- Every concept has a unique ID.
- Every word belongs to one language.
- Multiple words can point to the same concept.
- Vocabulary lists are generated from tags.
- Arabic words can optionally belong to a root family.


## Definitions

Concept: Expresses a fundamental unit of meaning at the highest level of the model. Go, Write, Attack, are all units of meaning. These units of meaning need aliases because I'll also search up the Spanish and Arabic equivalents. Additionally, a concept has to differentiate between how a word is used as a noun, verb, adjective, adverb, phrase, and expression. For example, beautiful, to beautify, rapid, and rapidly all express different concepts since they express different meanings. This changes the naming conventions. For example, rapid as an adjective and rapid as an adverb are named like this: RAPID_ADJ, RAPID_ADV. A single concept can connect to many different lexemes. Concept needs to be here to describe a general meaning and connect it with lexemes. Concepts aren't tagged. This label is many-to-many because it will link up with many Arabic, English, and Spanish words.

Lexeme: This is a dictionary entry of an individual word within a given language. Lexemes are primarily singular nouns, adjectives and infinitive verbs. Write, escribir, writer, and كَاتِب are all lexemes because they reserve single dictionary definitions. I'm using the English meaning of a dictionary. Arabic dictionaries are defined by root, and that's not helpful for me. A single lexeme can connect to many concepts, a root and word forms. Lexemes are tagged with LexemeTag. This label is many-to-many because it can link up with many different Concepts and Word Forms, but it will usually link up with many word that are not of the same conjugation through Relations.

WordForm: This is an alternation on a word connected to a lexeme. For example, writer is a lexeme, but writers is a word form. Escritor is a lexeme, but escritora, escritores and escritoras are word forms. This placement is where adverbs, all participles, female singular, and all plurals are placed. Rápidamente, rápida, rápidos and habido are all word forms. WordForm is many-to-many because a single word form such as fui can connect to many different lexemes and connect to other word forms through Relation.

Relation: This is the connecting mechanism between words that aren't related by conjugation. Synonyms, antonyms, derivations and relations connect word forms to other word forms, and even lexemes to other lexemes. Relation is many-to-many for flexibility.

Root: This is an Arabic-specific mechanism. An Arabic word will usually be connected to other Arabic words through the root. This is one-to-many due to how intertwined Arabic words are to a single root.

LexemeTag: This connects lexemes directly to tags. This is many-to-many because one lexeme can be connected to many different tags, and one tag can go on many differen lexemes.

VocabularySet: This is a high level relation between words with a specific pedagogical intent made to organize and search words easily within a specific list. This is many-to-many because of the organizational pattern.
