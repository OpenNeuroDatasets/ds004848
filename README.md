# Natural viewing reveals an extended network of brain regions involved in processing familiar faces that is disrupted in prosopagnosia

## Overview
This dataset contains fMRI movie-watching and category localiser data in 28
developmental prosopagnosics and 45 neurologically healthy controls.
Participants are additionally grouped by their familiarity with the Game of
Thrones television series.

In movie-watching scans, participants passively viewed a series of short
audiovisual clips (ranging from 50 to 117 s duration; total duration =
12 min 58 s) taken from the Game of Thrones television series.

In category localiser scans, participants viewed images of faces, scenes, and
phase scrambled versions of the face images. These can be used to define face
and scene selective regions of interest.

> Please refer to the folloiwng paper when using this dataset:
>
> Noad, K., Watson, D.M., Andrews, T.J. (In review). Natural viewing reveals an
> extended network of regions for familiar faces that is disrupted in
> developmental prosopagnosia.


## Data Contents
* `participants.tsv` - List of subject IDs in control and developmental
  prosopagnosic groups, along with whether they were familiar or unfamiliar
  with Game of Thrones.

* `slice_timings.tsv`, `fsl_slice_timings.txt` - Slice timings for functional
  scans. The TSV file gives the times in milliseconds, and the text file gives
  the times in normalised units of the TR suitable for entering into FEAT.

  > Scans were acquired with the HCP/CMRR multiband sequence. More information
  > on slices timings can be found at:
  > https://wiki.humanconnectome.org/download/attachments/40534057/CMRR_MB_Slice_Order.pdf

* `behavioural_measures.tsv` - Scores on PI20, CFMT, and Game of Thrones quiz
  tasks (see below for more details). PI20 scores are out of 100. CFMT scores
  are given as percentage accuracies. Quiz scores are given as percentage
  accuracies over all questions as well as broken down by face, scene, and
  narrative questions.

* `Subject Directories` - MRI data directories for each subject:
  - `anat` - T1 anatomical images
  - `fmap` - Magnitude and phase difference fieldmap images
  - `func` - Movie-watching (Game of Thrones) and category localiser data


## Behavioural Measures
We provide two measures of face processing ability (PI20 and CFMT) and a quiz
assessing familiarity with the Game of Thrones TV series. All participants
completed the Game of Thrones quiz, and all developmental prosopagnosics
completed the PI20 and CFMT assessments. Approximately half of the control
subjects also completed the CFMT.

* `PI20` - 20-item prosopagnosia index, used as initial screening for
  developmental prosopagnosia. All developmental prosopagnosic participants
  comleted this.
  > Reference: Shah et al. (2015), Royal Society Open Science, 2(150305), 1-6.

* `CFMT` - Cambridge Face Memory Test, used as secondary screening for
  developmental prosopagnosia. All developmentral prosopagnosic participants
  and approximately half of the control participants completed this.
  > Reference: Duchaine & Nakayama (2006), Neuropsychologia, 44(4), 576-585.

* `Game of Thrones Quiz` - We developed this quiz to assess familiarity with
  the Game of Thrones television series. All participants completed this quiz.
  The quiz comprised 3 types of questions:
  * **Face** questions presented participants with a picture of a character,
    and participants had to provide a name or some defining biographical
    information for that character (e.g., "Jon Snow").
  * **Scene** questions similarly presented participants with a picture of a
    scene from the show and participants had to name or provide some details of
    the location (e.g, "King's Landing").
  * **Narrative** questions were 4-option multiple choice questions about key
    elements of the Game of Thrones story. For example, "Which character was
    Lord of Winterfell and was beheaded at the end of Season 1 - A) Daenerys
    Targaryen, B) Jon Snow, C) Ned Stark, or D) Tyrion Lannister?"


## Notes
* sub-DP15 is missing category localiser and fieldmap scans due to time
  constraints during the scanning session.
