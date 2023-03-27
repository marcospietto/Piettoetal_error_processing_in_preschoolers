# Data from Pietto et al (Brain Sciences, 2023)
Preschool children show neural responses and make behavioral adjustments immediately following an error. commission. However, there is a lack of evidence regarding how neural responses to error predict subsequent behavioral adjustments during childhood. The aim of our study was to explore the neural dynamics of error processing and associated behavioral adjustments in preschool children from Unsatisfied Basic Needs (UBN) homes. Using EEG recordings during a Go/No-go task, we examined within-subject associations between the ERN, frontal midline theta power, post-error slowing, and post-error accuracy. Post-error accuracy increased linearly with post-error slowing, and there was no association between the neural activity of error processing and Post-error accuracy. However, during successful error recovery, frontal midline theta power, but not ERN amplitude, was associated positively with Post-error slowing. These findings indicated that preschool children from UBN homes adjusted their behavior following an error in an adaptive form and that the error-related theta activity may be associated with the adaptive forms of post-error behavior. Furthermore, our data support the adaptive theory of Post-error slowing and point to some degree of separation between the neural mechanisms represented by the ERN and theta.
# How to cite us
#### Please, if you like it / use it cite us:
Pietto, M. L., Giovannetti, F., Segretin, M. S., Lipina, S. J., & Kamienkowski, J. E. (2023). EEG dynamics of error processing and associated behavioral adjustments in preschool children. Brain Sciences.
# Data
Inside the file "Piettoetal_error_processing_in_preschoolers.m," you can find two structures: EEG and BEHAVIOR. The EEG structure contains the event-related activity, while the BEHAVIOR structure contains behavioral measures used for analysis.

|Name 	                                                   | Size 	  | Bytes   | Class  |	Description|
|----------------------------------------------------------|--------------------|--------|-------------|--------------------------------------------------------------
|EEG.error_correct              | 1X1      | 9153546 | struct |  Event-related activity from error and correct responses |
|EEG.error_correct.ERP   | 128x93x3      | 285696  | double |  Time-domain amplitude. Time x Subjects x Conditions. Condition #1 = correct-locked activity; Condition #2 = error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.error_correct.THETA | 128x93x3      | 285696  | double | Time-frequency power in Theta band. Time x Subjects x Conditions. Condition #1 = correct-locked activity; Condition #2 = error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.error_correct.SPECTRA | 3x128x93x30      | 8570880  | double | Time-frequency power in the spectrum range 1-30 Hz. Conditions x Time x Subjects x Hz. Condition #1 = correct-locked activity; Condition #2 = error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.error_correct.ID_SUBJECT   | 1x93      | 10602  | cell |  Subject's ID |
|EEG.single_double_error             | 1X1      | 4383402 | struct |  Event-related activity from double and single error responses: a false alarm followed by another false alarm and a false alarm followed by a hit |
|EEG.single_double_error.ERP   | 128x45x3      | 138240  | double |  Time-domain amplitude. Time x Subjects x Conditions. Condition #1 = single_error-locked activity; Condition #2 = double_error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.single_double_error.THETA | 128x45x3      | 138240  | double | Time-frequency power in Theta band. Time x Subjects x Conditions. Condition #1 = single_error-locked activity; Condition #2 = double_error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.single_double_error.SPECTRA | 3x128x45x30      | 4147200  | double | Time-frequency power in the spectrum range 1-30 Hz. Conditions x Time x Subjects x Hz. Condition #1 = single_error-locked activity; Condition #2 = double_error-locked activity; Condition #3 = difference between Condition #2 and #1 |
|EEG.single_double_error.ID_SUBJECT   | 1x45      | 5130  | cell |  Subject's ID |
|EEG.single_error_tertiles             | 1X1      | 5708916 | struct |  Event-related activity from single error responses separated by their post-error slowing into tertiles |
|EEG.single_error_tertiles.ERP   | 128x58x3      | 178176  | double |  Time-domain amplitude. Time x Subjects x Conditions. Condition #1 = single_error 1st tertile-locked activity; Condition #2 = single_error 2nd tertile-locked activity; Condition #3 = single_error 3rd tertile-locked activity |
|EEG.single_error_tertiles.THETA | 128x58x3      | 178176  | double | Time-frequency power in Theta band. Time x Subjects x Conditions. Condition #1 = single_error 1st tertile-locked activity; Condition #2 = single_error 2nd tertile-locked activity; Condition #3 = single_error 3rd tertile-locked activity |
|EEG.single_error_tertiles.SPECTRA | 128x45x30x3      | 5345280  | double | Time-frequency power in the spectrum range 1-30 Hz. Time x Subjects x Hz x Conditions. Condition #1 = single_error 1st tertile-locked activity; Condition #2 = single_error 2nd tertile-locked activity; Condition #3 = single_error 3rd tertile-locked activity |
|EEG.single_error_tertiles.ID_SUBJECT   | 1x58      | 6612  | cell |  Subject's ID |
|EEG.TIMES   | 1x128      | 1024  | double |  time in ms |
|BEHAVIOR.DATA   | 103x9      | 7416  | double |  Subject x Behavioral measures |
|BEHAVIOR.NAMES_VARIABLES   | 1x9      | 1286  | cell |  Names of behavioral measures of columns in BEHAVIOR.DATA |
|BEHAVIOR.ID_SUBJECT   |  1x103    | 11742  | cell |  Subject's ID |


Note.
The EEG variables correspond to event-related activity originating from the region of interest located at F3/F4.
