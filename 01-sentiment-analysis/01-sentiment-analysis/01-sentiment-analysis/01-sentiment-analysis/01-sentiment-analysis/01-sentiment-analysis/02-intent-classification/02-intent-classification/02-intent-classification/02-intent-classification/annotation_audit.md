Annotation Audit Report

Advanced Customer Intent Classification

Project: Customer Support Intent Classification
Reviewer: Rupech Nkengafack
Review Type: Self-review of synthetic annotations

1. Purpose of the Audit

This audit reviews the 40 annotated customer messages to identify possible classification errors, unnecessary secondary labels, inconsistent confidence ratings and cases where the annotation guidelines need clarification.

The objective is to improve consistency and ensure that labels reflect what the customer is actually asking for, rather than simply mentioning related topics.

2. Key Review Findings

Record ID	Review Finding	Recommended Action
IC007	The main issue is the delivery driver’s behaviour, not tracking the order.	Keep COMPLAINT as primary; remove ORDER_TRACKING as secondary unless tracking was also requested.
IC011	The customer reports being charged after cancelling. Billing is the main issue.	Keep BILLING as primary; review whether CANCELLATION is a genuine secondary intent.
IC013	The failed password reset link is part of an account-access problem.	Keep ACCOUNT_ACCESS as primary; remove TECHNICAL_SUPPORT unless a separate technical issue is being reported.
IC018	The locked account and urgent payment create two related but distinct issues.	Retain ACCOUNT_ACCESS and BILLING; review urgency as High.
IC019	The customer explicitly wants to return an item and receive a refund.	Keep REFUND as primary; remove COMPLAINT unless dissatisfaction is explicitly expressed.
IC020	The customer reports a failed payment message despite money leaving the account.	Retain BILLING as primary and TECHNICAL_SUPPORT as secondary if both issues are represented.
IC023	Permanently deleting an account is closer to ending the account relationship than updating account details.	Review CANCELLATION as the primary label; remove ACCOUNT_UPDATE if it is only contextual.
IC025	The customer requests a replacement because the product stopped working.	Keep REPLACEMENT as primary; remove TECHNICAL_SUPPORT unless troubleshooting is also requested.
IC028	Changing a delivery address concerns an existing order rather than general profile information.	Consider ORDER_TRACKING as primary, based on the project taxonomy.
IC030	The customer wants to cancel because they are unhappy with the service.	Keep CANCELLATION as primary; do not add COMPLAINT unless there is a separate complaint request.
IC034	The customer wants a missing item replaced.	Keep REPLACEMENT as primary; remove ORDER_TRACKING unless delivery tracking is also requested.
IC035	A charge the customer does not recognise is primarily a billing issue.	Keep BILLING as primary; review whether COMPLAINT is necessary as a secondary label.
IC038	The message expresses satisfaction about an early delivery but does not ask a question or request an action.	Flag as a taxonomy edge case. Review whether ORDER_TRACKING is appropriate for status updates.
IC039	The customer requests cancellation and confirmation that no payment will be taken.	Retain CANCELLATION as primary and review BILLING as a possible secondary intent.
IC040	The customer cannot complete a transaction because the service is unavailable.	Keep TECHNICAL_SUPPORT as primary; remove BILLING unless an actual payment issue is described.

3. Confidence Rating Review

Assigning High confidence to every record can make an annotation dataset appear less realistic.

Confidence should reflect how clearly the message supports the assigned labels.

Recommended approach:

* High: The customer’s main request is explicit and unambiguous.
* Medium: The message contains overlapping issues or requires interpretation.
* Low: The message lacks enough information for a reliable classification.

Records involving overlapping requests or unclear intent should be reconsidered for Medium confidence rather than automatically receiving High confidence.

4. Important Annotation Lessons

The review highlighted several important distinctions:

Intent is not sentiment.
A customer can sound angry while requesting a refund. Their intent remains REFUND, while their sentiment may be Negative.

Related topics are not automatically secondary intents.
A secondary label should represent another identifiable issue or request, not simply background information.

Context should not replace the customer’s actual request.
For example, mentioning a broken product does not automatically mean the customer wants technical support. If they explicitly request a replacement, REPLACEMENT should remain the primary intent.

Unclear cases should be flagged.
When the taxonomy does not adequately describe a message, the reviewer should document the ambiguity rather than force an unsuitable label.

5. Recommended Quality Improvements

For future annotation rounds:

1. Apply secondary labels only when a distinct additional intent is present.
2. Reassess confidence ratings instead of assigning High by default.
3. Distinguish order-related changes from general account updates.
4. Separate customer dissatisfaction from the actual reason for contacting support.
5. Document ambiguous cases for guideline review.
6. Recheck revised annotations against the original message.

6. Review Conclusion

This audit demonstrates the importance of reviewing annotations beyond basic label assignment.

A consistent annotation process requires careful interpretation, clear label definitions, justified confidence ratings and the ability to recognise ambiguous cases.

The findings will inform improvements to the dataset and annotation guidelines.

Disclosure: This is an independent self-review of a simulated customer-support dataset created for portfolio demonstration. It is not an independent second-annotator evaluation.
