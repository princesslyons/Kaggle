# [NBME - Score Clinical Patient Notes Data](https://www.kaggle.com/c/nbme-score-clinical-patient-notes/data)
The text data presented here is from the USMLE® Step 2 Clinical Skills examination, a medical licensure exam. This exam measures a trainee's ability to recognize pertinent clinical facts during encounters with standardized patients.

During this exam, each test taker sees a Standardized Patient, a person trained to portray a clinical case. After interacting with the patient, the test taker documents the relevant facts of the encounter in a patient note. Each patient note is scored by a trained physician who looks for the presence of certain key concepts or features relevant to the case as described in a rubric. The goal of this competition is to develop an automated way of identifying the relevant features within each patient note, with a special focus on the patient history portions of the notes where the information from the interview with the standardized patient is documented.

### Important Terms
  - **Clinical Case:** The scenario (e.g., symptoms, complaints, concerns) the Standardized Patient presents to the test taker (medical student, resident or physician). Ten clinical cases are represented in this dataset.
  - **Patient Note:** Text detailing important information related by the patient during the encounter (physical exam and interview).
  - **Feature:** A clinically relevant concept. A rubric describes the key concepts relevant to each case.

### Training Data
  - patient_notes.csv - A collection of about 40,000 Patient Note history portions. Only a subset of these have features annotated. You may wish to apply unsupervised learning techniques on the notes without annotations. The patient notes in the test set are not included in the public version of this file.
    - `pn_num` - A unique identifier for each patient note.
    - `case_num` - A unique identifier for the clinical case a patient note represents.
    - `pn_history` - The text of the encounter as recorded by the test taker.
  - features.csv - The rubric of features (or key concepts) for each clinical case.
    - `feature_num` - A unique identifier for each feature.
    - `case_num` - A unique identifier for each case.
    - `feature_text` - A description of the feature.
  - train.csv - Feature annotations for 1000 of the patient notes, 100 for each of ten cases.
    - `id` - Unique identifier for each patient note / feature pair.
    - `pn_num` - The patient note annotated in this row.
    - `feature_num` - The feature annotated in this row.
    - `case_num` - The case to which this patient note belongs.
    - `annotation` - The text(s) within a patient note indicating a feature. A feature may be indicated multiple times within a single note.
    - `location` - Character spans indicating the location of each annotation within the note. Multiple spans may be needed to represent an annotation, in which case the spans are delimited by a semicolon ;.

### Example Test Data
To help you author submission code, we include a few example instances selected from the training set. When your submitted notebook is scored, this example data will be replaced by the actual test data. The patient notes in the test set will be added to the patient_notes.csv file. These patient notes are from the same clinical cases as the patient notes in the training set. There are approximately 2000 patient notes in the test set.
  - test.csv - Example instances selected from the training set.
  - sample_submission.csv - A sample submission file in the correct format.
