I'll import from:

- Wiktionary
- Al-Maany
- Your vocabulary lists
- Manual entry

Each source maps differently into the database.


For Wiktionary:

For nouns and adjectives, import the masculine and femine singular and plural forms, as well as derived terms.

For verbs, use the third person singular past tense, masdar, and singular masculine forms of derived nouns and adjectives for lexemes. The third person singular non-past tense verb is included, but it's a word form.

Cross reference citations with other dictionaries, or with the provided dictionary entry.

For Al-Maany:

Use this website for phrases and synonym-building.

For my vocabulary sets:

Import what I can from these sets.

For manual entry:

Search up new words, and add them using the other dictionaries.


Adding a New Word: Decision Chart

         START
          |
          |-- What is the meaning/concept?
          |        |
          |        └── Create or link Concept
          |
          |-- Is this a new dictionary entry?
          |
          ├── YES → Create Lexeme
          |
          └── NO → Create Word Form

Lexeme vs. Word Form Quick Reference

| Language          | Add as Lexeme                               | Add as Word Form              |
| ----------------- | ------------------------------------------- | ----------------------------- |
| English Verb      | base verb                                   | conjugations                  |
| English Noun      | independent noun                            | plural forms                  |
| English Adjective | adjective                                   | comparative/superlative forms |
| Spanish Verb      | infinitive                                  | conjugated forms              |
| Spanish Noun      | noun                                        | gender/plural forms           |
| Spanish Adjective | masculine singular form                     | feminine/plural forms         |
| Arabic Verb       | past 3rd person masculine singular (كَتَبَ) | conjugated forms              |
| Arabic Noun       | dictionary singular                         | plural/dual/declensions       |
| Arabic Adjective  | masculine singular                          | feminine/plural forms         |

Lexeme:
- main verb
- important nouns
- agent nouns
- important adjectives
- masdars
- derived forms with their own meaning

Word Form:
- conjugation
- gender
- number
- case
- tense
- person

Database Entry Workflow:

1. Add Concept
   
   ↓

2. Add Lexemes

   ↓
   
3. Add Word Forms
 
   ↓
   
4. Add Root (Arabic only)
   
   ↓
   
5. Add Relations


Example:

CONCEPT

WRITE

LEXEMES

English:
  write (verb)
  writer (noun)

Spanish:
  escribir (verb)
  escritor (noun)

Arabic:
  كتب (verb)
  كاتب (noun)
  كتابة (masdar)
  مكتوب (adjective)

WORD FORMS

English:
  wrote, written

Spanish:
  escribí, escribiendo

Arabic:
  يكتب, اكتب, كتبوا

ROOT
ك-ت-ب

RELATIONS

writer → derived_from → write

كاتب → derived_from → كتب

كتابة → derived_from → كتب
