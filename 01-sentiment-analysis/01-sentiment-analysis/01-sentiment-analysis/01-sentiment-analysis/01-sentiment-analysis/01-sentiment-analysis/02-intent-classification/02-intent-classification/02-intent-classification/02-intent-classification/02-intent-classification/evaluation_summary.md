Evaluation Summary

Advanced Customer Intent Classification

Project: Customer Support Intent Classification
Prepared by: Rupech Nkengafack
Dataset: 40 synthetic customer-support messages
Evaluation Type: Annotation review and qualitative assessment

1. Project Overview

This project explored how customer-support messages can be classified into actionable intent categories while capturing urgency, sentiment and secondary requests.

The dataset contains 40 simulated customer interactions covering common support scenarios, including refunds, order tracking, cancellations, billing disputes, account access and technical problems.

2. Annotation Framework

Each message was reviewed using the following fields:

* Primary Intent: The customer’s main reason for contacting support.
* Secondary Intent: An additional identifiable request or issue, where applicable.
* Urgency: The level of attention required.
* Sentiment: The emotional tone expressed in the message.
* Confidence: The annotator’s confidence in the assigned labels.

3. Evaluation Findings

The annotation exercise highlighted several challenges:

Overlapping intents:
Some messages contained more than one issue. Identifying the primary reason for contact required distinguishing the customer’s main request from supporting context.

Intent versus sentiment:
Negative language did not automatically indicate a complaint. A frustrated customer could still primarily be requesting a refund, account correction or technical solution.

Secondary-label consistency:
Some related topics did not necessarily represent separate customer intentions. The audit identified cases where secondary labels needed reconsideration.

Urgency interpretation:
Urgency needed to reflect the practical impact of the issue rather than the emotional intensity of the message alone.

Taxonomy limitations:
Certain messages, particularly positive order-status updates, exposed situations that were not perfectly represented by the existing intent categories.

4. Quality Review

A self-review was conducted across the dataset to identify:

* Potentially unnecessary secondary labels.
* Cases requiring reconsideration of the primary intent.
* Confidence ratings that may have been too high.
* Ambiguous examples requiring clearer annotation rules.
* Opportunities to improve consistency between similar messages.

The review also reinforced the importance of documenting uncertain decisions rather than forcing every message into an apparently obvious category.

5. Skills Demonstrated

This project demonstrates practical experience in:

* Multi-label text annotation.
* Customer intent classification.
* Sentiment identification.
* Urgency assessment.
* Confidence scoring.
* Ambiguity resolution.
* Annotation guideline development.
* Quality assurance and error identification.
* Structured dataset documentation.

6. Limitations

This project uses synthetic customer-support messages and represents an independent portfolio exercise.

The annotations have undergone self-review, not independent second-annotator validation. No machine-learning model was trained or benchmarked, and no model accuracy or inter-annotator agreement is claimed.

7. Conclusion

The project demonstrates that reliable intent classification involves more than assigning categories to messages.

An effective annotation process requires understanding customer context, separating primary requests from secondary information, applying consistent guidelines and reviewing uncertain decisions.

The exercise strengthened my ability to approach customer-support data from both an annotation and quality-assurance perspective.

Disclosure: Independently developed portfolio project using simulated data. No paid client assignment is represented.
