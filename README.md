# xq-data

This data is from recordings of live math tutoring sessions done on PRACTICE Benefit Corp tutoring software for a Semi Auto Tutor project funded by the XQ Institute. 


This repo contains the following data files:

### annotated-data/
- `CodeTable_TrainingSet.csv`: The coding schema that maps to 'contentFocus', 'contentCode', and 'exemplar' in the `XQ_Training_Set.json` file. Altogether there around 300 available codes, only a fraction of which are actually in use so far. The schema is pretty far along, but not final. More codes are added as we encounter new needs. 
- `XQ_Training_Set.json`: JSON file containing a sample of segments extracted from over 40 different transcripts
- JSON fields:
```
"source": Transcript ID 
"start": Timestamp
"stop": Timestamp
"speaker": Speaker role (Tutor, Student)
"contribution": Text output by the speech-to-text algorithm
"correct": Where relevant, the annotator's assessment as to whether the student's contribution is "correct"
"dialogAct": The annotator's dialog act classification
"contentFocus": Corresponds to a specific focus within the lesson
"contentCode": A content-specific tag
"exemplar": A text string, in some cases with embedded components, that serves multiple purposes, including (a) assessment of student contributions (e.g. we can test whether the student's contribution matches the exemplar), (b) a source for NLP algorithms to use in generating contributions; and (c) reviewing the match between the initial contribution and the exemplar, as a check on the "fit" of the tag.
"codeFit": The annotator's judgement as to the extent to which the full code is a good match for the initial contribution. The primary test is whether an NLP process which takes the dialog act and exemplar as inputs might be able to output a string (e.g., a tutoring move) that is roughly equivalent to the original contribution (Column E)
```

### raw-transcripts/
- JSON files containing the audio file transcripts
- These recordings were done using a single audio stream. The transcriptions were at times jumbled because the two speakers spoke over each other and will therefore require additional cleanup.
- Any new recordings will have dual channel audio. 
- JSON fields: 
```
"start": Timestamp
"stop": Timestamp
"speaker": Speaker Role (Tutor, Student)
"dialogue": The text output by the speech-to-text algorithm
```

The contact for XQ is annotation@eduworks.com
