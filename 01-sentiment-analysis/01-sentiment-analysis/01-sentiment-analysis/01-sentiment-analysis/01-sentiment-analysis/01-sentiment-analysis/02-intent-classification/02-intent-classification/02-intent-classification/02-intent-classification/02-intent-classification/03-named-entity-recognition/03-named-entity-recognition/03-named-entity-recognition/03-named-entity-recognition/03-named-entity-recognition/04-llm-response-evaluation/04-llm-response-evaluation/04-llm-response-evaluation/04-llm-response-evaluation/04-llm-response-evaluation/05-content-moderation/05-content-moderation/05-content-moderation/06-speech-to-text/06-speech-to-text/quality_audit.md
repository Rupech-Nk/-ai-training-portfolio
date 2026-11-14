Quality Audit – Speech-to-Text Evaluation

1. Audit Overview

This audit reviews the 20 synthetic transcription examples to assess error classification, correction accuracy, consistency, and preservation of meaning.

The review focuses on identifying incorrect labels, ambiguous cases, and transcription errors that could affect real-world communication.

This is a self-review of the portfolio dataset, not an independent validation exercise.

2. Detailed Findings

Record ID	Finding	Recommended Action
ST001	The missing negation reverses the meaning of the customer’s message.	Retain Negation Error.
ST004	“Guarantee” is related in meaning to “warranty” but does not reproduce the reference wording.	Retain Word Substitution and distinguish verbatim accuracy from semantic similarity.
ST005	Fifteenth is transcribed as fiftieth, changing an important date.	Retain Number Substitution.
ST006	“I’ve tried” becomes “I tried.” This changes the verb tense/aspect rather than simply expanding a contraction.	Reclassify as Word Substitution or grammatical-form error. Review the punctuation separately.
ST008	The spoken email address is rendered incorrectly as “rupech text.”	Retain the entity-related error, but clarify that the period in the email address was not correctly represented.
ST011	Douala is misspelled as Duala.	Retain Proper Noun Error.
ST012	The opening word “No” is omitted, removing an important correction or disagreement marker.	Retain Word Omission.
ST013	One digit is missing from the order number.	Retain Number Omission.
ST015	The missing negation changes the meaning of the complaint.	Retain Negation Error.
ST019	The missing negation reverses the reported refund status.	Retain Negation Error.

3. Classification Improvements

The current annotation taxonomy could be made more precise.

Recommended improvements:

* Separate meaning-changing substitutions from minor wording differences.
* Record punctuation errors independently from word-recognition errors.
* Introduce a grammatical-form or tense error category.
* Treat email addresses, order numbers, dates, and other identifiers as high-priority entities.
* Distinguish exact transcription accuracy from preservation of general meaning.

4. High-Impact Error Analysis

Several errors deserve particular attention because they could create practical problems:

Negation errors: ST001, ST015 and ST019 demonstrate how omitting a short word can reverse a customer’s message.

Number errors: ST005 and ST013 show why dates and order identifiers require careful verification.

Entity errors: ST008 and ST011 demonstrate the importance of accurately capturing email addresses and place names.

Action-related errors: ST018 changes “upload” to “download,” potentially causing an incorrect technical support response.

5. Consistency Review

The dataset includes three examples labelled No Error: ST003, ST007 and ST017.

These examples provide useful controls for checking whether an evaluator can recognise accurate transcripts instead of assuming every example contains an error.

The corrected transcripts should remain faithful to the reference wording rather than introducing unnecessary improvements.

6. Recommended Improvements

Before finalising the project:

1. Reclassify ST006 to reflect the change in tense/aspect.
2. Clarify the treatment of punctuation differences.
3. Standardise the error taxonomy across all records.
4. Prioritise meaning-changing errors involving negations, numbers, names and actions.
5. Keep the reference transcript as the source of truth when making corrections.

7. Conclusion

The review demonstrates that transcription evaluation requires more than spotting spelling mistakes.

An effective evaluator must recognise subtle changes in meaning, distinguish lexical errors from formatting differences, and pay close attention to information that could affect customer interactions.

The findings are recommendations for improving the dataset. They should not be treated as corrections already applied.
