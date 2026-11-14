NER Evaluation Summary

Customer Support Named Entity Recognition

Prepared by: Rupech Nkengafack
Project Type: Independent AI Annotation Portfolio
Dataset: 30 synthetic customer-support messages
Annotation Records: 56 entity mentions

1. Project Overview

This project explored the identification and classification of named entities in customer-support messages.

The objective was to transform unstructured text into structured information that could support information extraction, data processing and natural language processing applications.

2. Entity Categories

The dataset covers ten entity categories:

* PERSON
* ORGANIZATION
* LOCATION
* DATE
* TIME
* MONEY
* ORDER_ID
* PRODUCT
* EMAIL
* PHONE

3. Annotation Approach

Each message was examined to identify relevant entity mentions.

The annotation process involved:

1. Understanding the message in context.
2. Identifying individual entities.
3. Selecting precise text boundaries.
4. Applying the appropriate entity category.
5. Reviewing annotations for consistency and completeness.

Multiple entities within the same message were recorded as separate annotation rows.

4. Quality Review Findings

The self-review identified several areas requiring attention:

Boundary consistency:
The distinction between complete addresses and individual location components requires clearer rules.

Entity classification:
Case references and order identifiers may require separate categories because they serve different purposes.

Contextual inference:
An organisation should not automatically be identified from an email domain without sufficient supporting information.

Temporal expressions:
Relative expressions such as “yesterday” and “tomorrow” require a consistent inclusion policy.

These findings demonstrate the importance of maintaining clear annotation rules and reviewing edge cases.

5. Skills Demonstrated

This project demonstrates practical understanding of:

* Named Entity Recognition.
* Information extraction.
* Entity classification.
* Text-boundary identification.
* Contextual interpretation.
* Structured dataset preparation.
* Annotation guideline development.
* Quality assurance and error identification.

6. Limitations

The dataset consists of simulated customer-support messages and is intended for portfolio demonstration.

The annotations were reviewed through self-assessment rather than independent annotator validation.

No machine-learning model was trained, and no model performance or benchmark accuracy is claimed.

7. Conclusion

This project demonstrates the process of converting ordinary customer messages into structured, labelled information.

It also highlights the importance of accurate entity boundaries, consistent classification rules and careful handling of ambiguous information.

The quality review provided practical insight into how annotation guidelines can be improved when inconsistencies or taxonomy limitations are identified.

Disclosure: Independently developed portfolio project using synthetic data. No paid client assignment is represented.
