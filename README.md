# xq-data

In 2022, the XQ Institute began a series of recordings of tutoring sessions in order to generate data on which to train machine learning models.

Each recording included the same tutor ("Amber"), a single, rich mathematics problem (see below), and a different student. Students were typically in 8th or 9th grade. The sessions were conducted on a zoom-like platform in which both the tutor and the student could annotate the image. They lasted around 1 hour each.

<img width="1330" alt="image" src="https://user-images.githubusercontent.com/10891410/217782296-fa2d30ef-e1cf-42ef-8f52-c63bbaf2f391.png">

The problem is based on one created by Malcolm Swan, a professor at the University of Nottingham, England. It is designed to reveal student thinking about reading graphs and relating them to a real-world journey. Typically, several misconceptions are uncovered and the tutor uses a productive struggle technique to advance student thinking. The pedagogy is less about "getting to the answer" than "understanding what is going on."

Each session began with only the first (left-most) part of the problem displayed. As the student's thinking progressed, the second and then third parts of the problem were uncovered.

This repo contains the raw transcripts of sessions, one file per session. We will add to it as more sessions are recorded. 

This repo contains the following data files:

- JSON fields: 
```
"start": Timestamp
"stop": Timestamp
"speaker": Speaker Role (Tutor, Student)
"dialogue": The text output by the speech-to-text algorithm
```
