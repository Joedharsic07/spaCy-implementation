## Rule-Based Matching :
- It is a method used to identify patterns or specific text in a document based on defined rules
- It helps us to extract entities, keywords, or specific types of phrases without training a model
## Token-based matching 
- It refers to identifying the patterns in text by comparing attributes of individual tokens rather than entire phrases
- It allows for flexible rule definitions based on token properties such as text content, lemma, part of speech, and more
## Attributes used in Token-based matching:
- "TEXT": Matches the exact text of the token.
- "LEMMA": Matches the base form of a word (e.g., "run" for "running").
- "LOWER": Matches the lowercase version of the text.
- "POS": Matches the part of speech (e.g., verb, noun).
- "IS_PUNCT": Matches punctuation tokens.
## Extended pattern syntax and attributes
- It allows highly flexible and detailed pattern definition
- These patterns are represented as a list of dictionaries where each dictionary specifies     
  attributes of individual tokens
- We can combine different attributes and logical operations to create complex matching rules
## Fuzzy matching
- It allows us to match tokens with alternate spellings, typos, etc without specifying every      possible variant.
- The FUZZY attribute allows fuzzy matches for any attribute string value, including custom       attributes.
## Operators and quantifiers:
- Quantifiers let us to define sequences of tokens to be matched
- For example one or more punctuation marks, or specify optional tokens.
## wildcard token pattern:
- It offers many options to write highly specific patterns to write specific patterns
- We can also use an empty dictionary
## Adding_on_match rule:
- It allows you to associate custom callback functions with patterns in the matcher
- These functions are triggered whenever the pattern is matched, enabling you to perform custom   actions, modify match behavior, or extract additional information
## Phrase match
## Efficient phrase matching:
- Efficient phrase matching is a way to quickly find and match specific phrases or sequences of   words in a large amount of text or data.
- Instead of checking word-by-word or letter-by-letter, special algorithms or techniques are      used to speed up the process.
- These methods help save time and resources, especially when searching through large documents   or databases.
## Bag Of Words (BOW):
-  What it is: A simple way to represent text data. It counts how many times each word appears     in a document without considering word order or meaning.
-   It loses context because it doesn’t know the order or meaning of words, just their         
    frequency.
## Global Vectors for Word Representation (GloVe):
- A technique that uses statistics from a large text corpus to find word meanings. It looks at    how often words appear together to create fixed-size vector representations.
- Words have one fixed vector, so it doesn’t understand different meanings (like “bank” for     
  money vs. riverbank).
## Word2Vec:
- A method that learns word meanings by predicting context. It comes in two Methods
    - CBOW: Predicts a word from its surrounding words.
    - Skip-gram: Predicts surrounding words from a given word.
- Like GloVe, it gives each word a single vector, missing multiple meanings.
## BERT:
-  A deep learning model that reads words in both directions (left-to-right and right-to-left)     to understand full context. It is more powerful because it handles word meanings based on       context.
- It is complex and requires lots of data and computing power. 
