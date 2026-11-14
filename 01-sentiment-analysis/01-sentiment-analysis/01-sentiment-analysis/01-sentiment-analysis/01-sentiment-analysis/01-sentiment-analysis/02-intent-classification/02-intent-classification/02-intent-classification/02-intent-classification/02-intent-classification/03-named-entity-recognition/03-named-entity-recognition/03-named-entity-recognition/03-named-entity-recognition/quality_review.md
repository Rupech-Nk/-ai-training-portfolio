NER Quality Review

Entity Identification and Annotation Audit

Project: Customer Support Named Entity Recognition
Reviewer: Rupech Nkengafack
Review Type: Self-review

1. Review Objective

This review examines the entity annotations for completeness, correct classification, boundary accuracy and consistency with the annotation guidelines.

The review focuses on identifying potential weaknesses that could affect the usefulness of the dataset for AI training.

2. Review Findings

Record	Issue Identified	Recommended Action
NER003	The word “yesterday” is a relative date expression.	Exclude it under the specific-date annotation policy.
NER009	“Dubai branch” contains a location reference, but only Dubai is the entity.	Retain Dubai as LOCATION.
NER011	The email address contains the domain brightstar.com, which suggests an organisation but does not explicitly identify its full business name.	Retain the email annotation; review whether Brightstar should be annotated as ORGANIZATION.
NER015	“Last month” is a relative date expression.	Exclude it under the current annotation policy.
NER016	“Tomorrow” is a relative date expression.	Exclude it under the current annotation policy.
NER021	The reference is labelled ORDER_ID, although it is a general case reference.	Consider introducing a separate CASE_ID category.
NER025	The street address and city are annotated separately.	Review consistency with the guideline requiring a complete address to be captured as one LOCATION entity.
NER027	“Before noon” contains a time expression.	Review whether approximate time expressions should be included in an expanded TIME category.

3. Additional Annotation Challenges

Entity boundaries

Selecting too much or too little text can make an annotation unreliable. Entity boundaries should follow the exact text and the project’s annotation rules.

Organisation identification

An email domain may suggest a business name, but the annotator should avoid assuming that the domain necessarily identifies the organisation mentioned in the message.

Identifiers

Order numbers, case references and transaction references can look similar. Their classification should reflect their actual purpose.

Relative dates and times

Expressions such as “yesterday”, “tomorrow” and “before noon” require a clearly defined annotation policy. This project excludes relative dates and approximate times unless explicitly expanded.

4. Recommended Improvements

1. Introduce a separate CASE_ID category for support case references.
2. Clarify whether complete street addresses should be one entity or multiple location components.
3. Define a consistent policy for organisation names inferred from email domains.
4. Keep relative dates separate from explicitly stated calendar dates.
5. Expand TIME annotation rules only when the intended application requires approximate time expressions.
6. Review all entity boundaries before final dataset submission.

5. Review Conclusion

The review highlights the importance of precise entity boundaries, consistent category definitions and careful interpretation of contextual information.

It also demonstrates that annotation guidelines should evolve when real examples expose gaps in the original taxonomy.

Disclosure: This is an independent self-review of a synthetic dataset. It is not an independent second-annotator validation.
