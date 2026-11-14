Customer Intent Classification: Annotation Guidelines

1. Purpose

These guidelines define how customer-support messages should be classified according to intent, urgency and sentiment.

The objective is to produce consistent, explainable annotations suitable for AI training and evaluation workflows.

2. Intent Identification

Annotators must identify the customer’s primary reason for contacting support.

Primary Intent Rules

* REFUND: The customer explicitly requests money back.
* ORDER_TRACKING: The customer asks about delivery, shipment or order status.
* CANCELLATION: The customer wants to terminate an order or service.
* ACCOUNT_ACCESS: The customer cannot access or authenticate their account.
* BILLING: The customer reports payment, invoice or subscription charges.
* TECHNICAL_SUPPORT: The customer reports a malfunction or technical issue.
* COMPLAINT: The main purpose is to report dissatisfaction or poor service.
* INFORMATION_REQUEST: The customer seeks general information.
* ACCOUNT_UPDATE: The customer requests changes to account details.
* REPLACEMENT: The customer requests a replacement for a damaged, defective, missing or incorrect item.

3. Primary and Secondary Intent

The primary intent represents the customer’s main requested outcome.

A secondary intent may be assigned when another distinct issue or request is also present.

Example:

Message: “My order never arrived, and I want my money back.”

Primary intent: REFUND
Secondary intent: ORDER_TRACKING

Do not assign secondary labels simply because a message mentions a related topic.

4. Urgency Classification

Level	Decision Rule
Critical	Immediate intervention is required due to serious risk or major operational impact.
High	A significant problem prevents an important transaction or service activity.
Medium	The customer needs assistance, but the situation is not immediately disruptive.
Low	General questions and routine requests.

Urgency must reflect the actual impact of the issue, not just emotional wording.

5. Sentiment Classification

Label	Meaning
Positive	Expresses satisfaction or appreciation.
Negative	Expresses dissatisfaction or frustration.
Neutral	Communicates a request or information without clear emotional sentiment.

Intent and sentiment must be evaluated independently.

A refund request may be neutral if the customer simply requests a refund without expressing dissatisfaction.

6. Handling Ambiguous Cases

When a message contains several requests:

1. Identify the desired outcome.
2. Determine which request is the main reason for contact.
3. Assign a secondary intent only when justified.
4. Record the reasoning behind the decision.

When intent is unclear, flag the example for secondary review rather than making unsupported assumptions.

7. Confidence Levels

* High: The message clearly supports the selected labels.
* Medium: The intended meaning is reasonably clear but contains some ambiguity.
* Low: The available information does not support a confident decision.

8. Quality Assurance Requirements

Every annotation must be checked for:

* Correct primary intent.
* Appropriate secondary intent.
* Consistent urgency classification.
* Accurate sentiment identification.
* Logical agreement between labels and message content.
* Complete annotation fields.

9. Annotation Principle

Annotate what the customer communicates and requests, not what the annotator assumes the customer might mean.

Document type: Independent portfolio simulation.
