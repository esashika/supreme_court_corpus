# Supreme Court Dialogs Corpus v1.01 (released September 2012)
## We will continue to innovate and achieve great results. Just a little help in corpus pre-processing. Rhedson Esashika.

This corpus contains a collection of conversations from the U.S. Supreme Court Oral Arguments (http://www.supremecourt.gov/oral_arguments/) with metadata:

- 51,498 utterances making up 50,389 conversational exchanges
- from 204 cases involving 11 Justices and 311 other participants (lawyers or amici curiae)
- metadata includes: 
	- case outcome
	- vote of the Justice 
	- section in which the conversation took place
	- gender annotation

Case outcome and vote data were extracted from the the Spaeth Supreme Court database (http://scdb.wustl.edu/)

1.   **CASE_ID** unique id of the case.
2.   **UTTERANCE_ID** unique id of the utterance.
3.   **AFTER_PREVIOUS** in {TRUE, FALSE}: TRUE if this utterance is part of the same conversation as the previous utterances, FALSE if this utterance starts a new conversation.
4.   **SPEAKER** the name of the speaker.
5.   **IS_JUSTICE** in {JUSTICE, NOT JUSTICE}: JUSTICE if the speaker is a Justice, NOT JUSTICE otherwise.
6.   **JUSTICE_VOTE** in {PETITIONER,RESPONDENT,NA}: PETITIONER if the Justice eventually voted for the petitioner, RESPONDENT if the Justice eventually voted for the respondent, NA if the Justice did not vote on this case or the speaker is not a Justice.
7.   **PRESENTATION_SIDE** in {PETITIONER, RESPONDENT}: PETITIONER if the line was uttered in the sections supporting the petitioner's case, RESPONDENT if the line was uttered in the section supporting the respondent's case. (The field is left empty if the utterance appears outside these sections, such as in the preamble of the argument.)  Note that while all Justices can speak in both sections, only lawyers supporting the petitioner's case will speak in the PETITIONER section, and only lawyers supporting the respondent's case will speak in the RESPONDENT section.  A detailed description of the structure of the Oral Arguments can be found at: http://www.supremecourt.gov/oral_arguments/ .
8.   **UTTERANCE** the text produced by the speaker.
