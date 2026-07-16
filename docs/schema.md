# Lexical Database Schema

## Core Objects

- Concept
Purpose:
Represents a language-independent meaning.

Fields

id
definition
notes
- Lexeme
Purpose:
Represents one dictionary entry in one language.

Fields

id
concept_id
language
lemma
part_of_speech
notes
- Word Form
- Tag
- Relation
- Root

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
