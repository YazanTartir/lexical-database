# Lexical Database

A personal multilingual lexical database for language learning, built with Godot 4 and SQLite.

## Purpose

This project is designed as a cross-language lexical knowledge base rather than a traditional dictionary.

Instead of organizing vocabulary around a single language, every entry is organized around language-independent concepts. English, Spanish, Arabic, and future languages are linked to these concepts through lexical entries and relationships.

The primary goal is to create a searchable, extensible database that supports language learning, writing, translation, and vocabulary expansion. Here is a visual representation of what this process looks like in practice:

       Concept 1   Concept 2
              ▲      ▲
              │      │
              expresses
                  │
                Lexeme
           ╱──────┼──────╲
          ╱       │       ╲
     WordForm     Root    Relation
         │                 │
         └───────┬─────────┘
                 │
                Tag
                 │
           Vocabulary Set


---

## Languages

Current

- English
- Spanish
- Modern Standard Arabic

Planned

- Egyptian Arabic
- Levantine Arabic

Future languages can be added without changing the overall architecture.

---

## Design Philosophy

The database is built around several core principles.

- Every concept exists exactly once.
- Every lexical item exists exactly once.
- Vocabulary lists are generated from tags instead of duplicated.
- Words can belong to multiple vocabulary sets simultaneously.
- Arabic roots are first-class objects.
- Expressions and phrases are treated as lexical entries rather than notes.
- Every object has a permanent ID.

---

## Planned Features

### Search

Search by

- English
- Spanish
- Arabic
- Root
- Tags
- Vocabulary sets
- Expressions
- Inflected forms

### Lexical Relationships

Support for

- Synonyms
- Antonyms
- Derived words
- Root families
- Feminine / masculine forms
- Singular / plural forms
- Verb derivations
- Expressions
- Dialectal variants

### Vocabulary

Generate thematic vocabulary lists automatically from tags.

Examples

- Military & Combat
- Medieval Warfare
- Politics & Government
- Religion & Spirituality
- Dialogue & Action

### Arabic

Support for

- Triliteral and quadriliteral roots
- Verb forms
- Broken plurals
- Regular plurals
- Participles
- Verbal nouns (مصادر)

### Spanish

Support for

- Irregular plurals
- Irregular first-person forms
- Regional vocabulary
- Register differences

---

## Technologies

- Godot 4.5
- SQLite
- Git
- GitHub

---

## Documentation

Additional documentation is stored inside the `docs/` directory.

Planned documentation

- schema.md
- architecture.md
- roadmap.md

---

## Current Status

Project initialization.

The first milestone is designing the complete database schema before implementing the user interface.
