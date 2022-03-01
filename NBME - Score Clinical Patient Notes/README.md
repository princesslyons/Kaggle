# [NBME - Score Clinical Patient Notes](https://www.kaggle.com/c/nbme-score-clinical-patient-notes/overview)

# Contents
  - [Competion Description Notes](#description-notes)
  - [Data Description](nbme-score-clinical-patient-notes/README.md)
  - [Additional Resources](#additional-resources)

## Description Notes:
  - Problem Statement
    - Learning and assessing the skill of writing patient notes requires feedback from other doctors, a time-intensive process that could be improved with the addition of machine learning.
    - Having physicians score patient note exams requires significant time, along with human and financial resources.
  - **Goal**
    - The goal of this competition is to develop an automated way of identifying the relevant features within each patient note, with a special focus on the patient history portions of the notes where the information from the interview with the standardized patient is documented.
    - Making the approach more transparent, interpretable, and easing the development and administration of such assessments.
  - NLP Challenges
    - For example, the feature "loss of interest in activities" can be expressed as "no longer plays tennis."  
  - Features
    - Rubrics that outlined each case's important concepts
    - More such features found in patient notes -> higher the score
    - Real-world issue: scoring patient note exams requires significant time, along with human and financial resources.   
  - Task
    - Identify specific clinical concepts in patient notes
    - Map clinical concepts from rubric (features) to varying ways students express them
      - Ex. "diminished appetite" -> "eating less," "clothes fit looser"  

## [Data Description](nbme-score-clinical-patient-notes/README.md)
  - Clinical Case: The scenario (e.g., symptoms, complaints, concerns) the Standardized Patient presents to the test taker (medical student, resident or physician). Ten clinical cases are represented in this dataset.
  - Patient Note: Text detailing important information related by the patient during the encounter (physical exam and interview).
  - Feature: A clinically relevant concept. A rubric describes the key concepts relevant to each case.
  - See (nbme-score-clinical-patient-notes/README.md)(nbme-score-clinical-patient-notes/README.md) for more details

## Additional Resources
  - Article: [Lessons learned building natural language processing systems in health care](https://www.oreilly.com/content/lessons-learned-building-natural-language-processing-systems-in-health-care/)
