Quality Audit – AI Content Moderation

1. Audit Overview

This audit reviews the 20 synthetic examples in the moderation dataset to assess label consistency, severity decisions, moderation actions, and the handling of ambiguous content.

The review focuses on identifying potential false positives, missed risks, and gaps in the annotation categories.

This is a self-review of the portfolio dataset, not an independent moderation assessment.

2. Key Findings

Record ID	Issue Identified	Recommended Review
CM005	The message expresses emotional distress but does not clearly indicate self-harm intent.	Consider removing the Self-Harm label. A context review may be more appropriate than an automatic escalation.
CM009	The statement is insulting, but it is a single mild remark rather than clear targeted harassment under the current guidelines.	Reclassify as Safe Content and allow, unless the platform’s policy explicitly covers isolated insults.
CM012	The message combines sexual coercion with a threat to expose private messages.	Consider adding a Sexual Coercion or Threats category, or allowing secondary labels.
CM014	The wording implies a threat, but the seriousness depends partly on context.	High severity and escalation are defensible. Preserve the decision while noting the contextual uncertainty.
CM017	The message requests banking credentials through a deceptive link.	Add a Phishing or Fraud risk category instead of relying only on Spam.
CM019	The content promotes exclusion based on disability.	The Hate Speech classification is defensible under the current taxonomy. Ensure disability-based discrimination is covered explicitly in the guidelines.

3. False Positive and Over-Escalation Risks

CM005 – Emotional Distress

A person expressing that they feel overwhelmed or wish to disappear may be experiencing serious distress. However, this wording alone does not establish an intention to self-harm.

The annotation should distinguish emotional distress from explicit or strongly indicated self-harm risk. Escalation should be guided by additional context and the platform’s safety policy.

CM009 – Mild Insult

The statement, “I hope you fail your examination,” is unkind but does not necessarily meet the project’s definition of harassment.

Treating every negative or unpleasant statement as harassment could lead to excessive content removal. The current guidelines should be applied consistently.

4. Taxonomy Improvements

The current category list could be expanded to handle more specific risks.

Recommended additions:

* Phishing/Fraud: Deceptive attempts to obtain passwords, banking information, or other sensitive credentials.
* Sexual Coercion: Sexual pressure, blackmail, or threats involving private images or communications.
* Context Review: A review status for cases where the available wording is insufficient to make a confident decision.

These additions would help distinguish different types of harmful content instead of forcing them into broad categories.

5. Consistency Checks

The following decisions are appropriate under the current guidelines:

* Direct hateful language and targeted harassment should be moderated.
* Explicit threats and imminent self-harm risk require escalation.
* Educational, historical, and fictional discussions should not automatically be treated as harmful.
* Negative opinions and ordinary disagreement should remain permitted.
* Spam and deceptive credential requests should be identified and handled appropriately.

6. Recommended Corrections

Before finalising the dataset:

1. Review CM005 to avoid treating emotional distress as confirmed self-harm intent.
2. Reconsider CM009 as a potential false positive.
3. Expand the taxonomy to capture phishing and sexual coercion more precisely.
4. Clarify how disability-based discriminatory content is handled.
5. Retain contextual review for ambiguous threats.

7. Conclusion

This review highlights an important moderation principle: effective content moderation requires more than identifying harmful language. It also requires understanding context, applying policy consistently, and avoiding unnecessary restrictions on harmless content.

The findings above are recommendations. They should not be treated as corrections already applied to the dataset.
