# UAV Acoustic Direction Finding and Tracking: Supporting Data

This repository contains the tabular data supporting **Real-Time Acoustic Direction Finding and Tracking of UAVs: An SRP-PHAT Method Guided by State Feedback**.

The Excel workbooks are organized in the order of the experimental methods and results in the article. Each workbook includes descriptive headings, units, and, where needed, a Notes sheet explaining the fields and statistical methods.

## 01 — Basic data

| Workbook | Contents | Article section |
| --- | --- | --- |
| [01 — Channel numbering map](01_Basic_Data/01_Channel_Numbering_Map.xlsx) | Correspondence between the 64 recorded audio channels and microphone IDs. | 3.1 |
| [02 — Flight recording index](01_Basic_Data/02_Flight_Recording_Index.xlsx) | The 36 flight recordings, their method and height groups, and the nine audio recordings used for offline evaluation. | 3.2 |
| [03A — Standard KF parameter fitting](01_Basic_Data/03A_Standard_KF_Parameter_Fitting.xlsx) | Fitted parameters, counts for the 11 development recordings, and all 99 parameter evaluations. | 3.3 |
| [03B — Standard KF input peak sequences](01_Basic_Data/03B_Standard_KF_Input_Peak_Sequences.xlsx) | The 29,402 basic SRP-PHAT peak outputs used for KF parameter fitting. | 3.3 |
| [04A — Video reference point verification](01_Basic_Data/04A_Video_Reference_Point_Verification.xlsx) | Verification and video reference coordinates for 180 sampled frames, with coordinate differences and distances between points. | 3.4 |
| [04B — Video reference point summary](01_Basic_Data/04B_Video_Reference_Point_Summary.xlsx) | Video reference trajectories for 36 recordings, comprising 21,549 sample times. | 3.4 |

## 02 — Experimental results

| Workbook | Contents | Article section |
| --- | --- | --- |
| [01 — Acoustic-to-image mapping and camera calibration](02_Experimental_Results/01_Acoustic_to_Image_Mapping_and_Camera_Calibration.xlsx) | Mapping parameters and correspondences, camera calibration, coordinate transformations, and independent check points. | 3.4 |
| [02 — Online processing performance](02_Experimental_Results/02_Online_Processing_Performance.xlsx) | Processing performance for individual flight recordings. | 4.1 |
| [03 — Offline performance evaluation](02_Experimental_Results/03_Offline_Performance_Evaluation.xlsx) | Summary metrics, results for individual recordings, evaluation counts, and time series for the four methods using the same audio inputs. | 4.2 |
| [04 — Flight-test tracking validation](02_Experimental_Results/04_Flight_Test_Tracking_Validation.xlsx) | Summary metrics, results for individual recordings, evaluation counts, and recorded online outputs. | 4.3 |
| [05 — Independent angular evaluation](02_Experimental_Results/05_Independent_Angular_Evaluation.xlsx) | Angular-error summaries, results for individual recordings, and direction series for offline and flight-test evaluation. | 4.4 |
| [06 — State feedback and grid sensitivity](02_Experimental_Results/06_State_Feedback_and_Grid_Sensitivity.xlsx) | Comparisons with and without front-end state feedback, grid-spacing sensitivity, computation times, and supporting time series. | 4.5 |
| [07 — Audiovisual time-offset sensitivity](02_Experimental_Results/07_Audiovisual_Time_Offset_Sensitivity.xlsx) | Offline and flight-test results under five audiovisual time offsets. | 3.4 |

## Reading the data

- **Relative height H** is the height relative to the home point displayed in DJI GO, in meters.
- **Recording identifiers:** FULL denotes SF-SRP-PHAT. The flight recording index links online recordings to the nine audio recordings used for offline evaluation.
- **KF development recordings:** S14–S19 and S24–S28 supply the observations used for standard KF parameter fitting. The parameter-fitting and peak-sequence workbooks describe initialization and update counts.
- **Video coordinates** are image positions in pixels. The reference-point verification workbook defines the coordinate axes, sampling procedure, and differences between points.
- **J95** measures the 95th percentile of reference-residual changes over 100 ms; **E95** measures the 95th percentile of reference deviations; **F50** is the exceedance or missing-output rate at a 50 px threshold. The relevant result workbooks specify the valid times and averaging rules used for each evaluation.

Download a workbook using its link above, then open the `.xlsx` file in Excel or another compatible spreadsheet application. The repository can also be downloaded as a ZIP archive from the **Code** menu.
