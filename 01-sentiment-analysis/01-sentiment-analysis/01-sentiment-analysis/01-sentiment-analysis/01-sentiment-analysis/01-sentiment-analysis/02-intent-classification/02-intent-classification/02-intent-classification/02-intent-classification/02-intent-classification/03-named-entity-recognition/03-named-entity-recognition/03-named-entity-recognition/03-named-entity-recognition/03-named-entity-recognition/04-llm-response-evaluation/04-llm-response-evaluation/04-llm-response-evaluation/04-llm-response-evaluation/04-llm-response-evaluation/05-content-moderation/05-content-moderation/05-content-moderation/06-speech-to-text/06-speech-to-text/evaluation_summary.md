Evaluation Summary – Speech-to-Text

1. Project Overview

This project evaluated 20 synthetic speech-to-text examples by comparing AI-generated transcripts against reference transcripts.

The objective was to identify transcription errors, correct inaccurate outputs, and assess how individual errors affect meaning and communication.

2. Dataset Statistics

Total examples reviewed: 20

Evaluation Result	Number
Examples containing transcription errors	17
Examples without transcription errors	3
Total examples	20

3. Error Categories Identified

The dataset covers several types of transcription errors.

Error Category	Examples
Negation errors	ST001, ST015, ST019
Word omissions	ST002, ST009, ST012
Word substitutions	ST004, ST010, ST014, ST016, ST018, ST020
Number substitution	ST005
Number omission	ST013
Entity-related error	ST008
Proper noun error	ST011
Contraction and punctuation difference	ST006

These categories reflect the original dataset annotations. The quality audit recommends reviewing the classification of ST006.

4. High-Impact Findings

Negation Errors

Missing negative expressions can completely reverse a speaker’s intended meaning. This was particularly evident in customer complaints and refund inquiries.

Number and Identifier Errors

Incorrect dates and order numbers can lead to delivery problems, incorrect records, and unnecessary customer service follow-ups.

Entity Recognition Errors

Incorrectly transcribed email addresses and location names can affect communication and service delivery.

Action-Related Substitutions

Confusing words such as “upload” and “download” can cause support teams to misunderstand a customer’s technical problem.

5. Quality Assurance Findings

The quality audit identified opportunities to improve annotation consistency.

These included:

* Distinguishing meaning-changing errors from minor wording differences.
* Separating punctuation issues from word-recognition errors.
* Reviewing grammatical-form changes.
* Prioritising numbers, names, email addresses and other identifiers.
* Ensuring corrected transcripts remain faithful to their references.

6. Evaluation Limitations

This project uses synthetic reference transcripts and simulated AI-generated outputs.

It does not claim:

* Evaluation of actual audio recordings.
* Testing of a commercial speech recognition system.
* Measured Word Error Rate (WER).
* Independent expert validation.
* Model training or deployment.

A reliable WER calculation would require actual audio-derived transcripts and reference transcripts with aligned word sequences.

7. Conclusion

This project demonstrates practical skills in transcription comparison, error identification, text correction, entity verification, and quality assurance.

It highlights how seemingly small transcription errors can change meaning and affect real-world customer interactions.

The exercise also demonstrates the importance of consistent annotation guidelines and careful human review of AI-generated outputs.
