Named Entity Recognition Annotation Guidelines

1. Purpose

These guidelines establish a consistent approach for identifying and classifying entities in customer-support messages.

The objective is to produce accurate, structured annotations that can support natural language processing and AI model training.

2. Entity Definitions

Label	Definition	Example
PERSON	A person’s full or identifiable name	Sarah Johnson
ORGANIZATION	A company, institution or business	Amazon
LOCATION	A geographic place or identifiable address	Dubai
DATE	A specific calendar date	20 November 2026
TIME	A specific time of day	3:30 PM
MONEY	A monetary value with its currency	AED 250
ORDER_ID	An order or transaction reference	ORD-78421
PRODUCT	A named product or service package	Galaxy S25
EMAIL	A complete email address	sarah@email.com
PHONE	A complete phone number	+971501234567

3. Annotation Rules

A. Exact Text Boundaries

Select the complete entity mention without adding unnecessary surrounding words.

Example:

Text: “I ordered a Samsung Galaxy S25 yesterday.”

Correct annotation: Samsung Galaxy S25 — PRODUCT.

Incorrect annotation: I ordered a Samsung Galaxy S25 — PRODUCT.

B. Preserve Original Text

Do not correct spelling, rewrite names or change the format of an entity.

The annotation must match the original message.

C. Multiple Entities

When a message contains several entities, annotate each one separately.

Example:

“Sarah paid AED 250 to Amazon on 12 November 2026.”

Annotations:

* Sarah — PERSON
* AED 250 — MONEY
* Amazon — ORGANIZATION
* 12 November 2026 — DATE

D. Repeated Entities

If the same entity appears more than once in a message, annotate each occurrence separately.

E. Contextual Interpretation

Use the surrounding message to determine the correct entity category.

For example, “Apple” refers to an ORGANIZATION when it identifies the technology company, while “Apple” can refer to a PRODUCT when it identifies the fruit.

F. Ambiguous Information

Do not invent missing information.

If a message says “I paid yesterday” without identifying an amount, do not create a MONEY annotation.

If an entity cannot be classified confidently, flag it for review.

4. Special Cases

* A street address should be captured as one LOCATION entity when the complete address is provided.
* Currency and amount should be captured together as MONEY.
* Order references should retain their original letters, numbers and symbols.
* Product names should include distinguishing model numbers when present.
* Email addresses and phone numbers should be captured in full.
* Relative expressions such as “tomorrow” and “last month” are not annotated as DATE under this project’s specific-date policy.
* General time expressions such as “noon” are not annotated as TIME unless the project is expanded to include approximate time expressions.

5. Quality Assurance Checklist

Before submitting annotations, verify:

1. Every identifiable entity has been considered.
2. Each entity has the correct category.
3. Entity boundaries are accurate.
4. Original spelling and formatting are preserved.
5. Multiple entities have separate annotation rows.
6. No information has been invented.
7. Ambiguous cases have been flagged for review.

6. Annotation Limitations

This project uses a simplified entity taxonomy designed for customer-support data.

Some entity types may require further distinctions in production datasets. For example, addresses could be divided into street, city and postal-code components, while order references could be separated from other transaction identifiers.

These distinctions should be introduced only when the intended model or downstream application requires them.
