Attached CSV file contains a number of medical cases (extracted from EHRs). Each entry consists of:

- one more more “present” symptoms (symptoms that patient had at the time of visit). For example s_0136 is GYANT code for “earache”.
- one more “absent” symptoms (symptoms that patient did not have). Keep in mind that there may other potential symptoms the patient was never asked about, which are neither “present” nor “absent”
- Age, Sex (1=Male), and Month of visit (which may be helpful, e.g. some conditions are gender-specific, some are seasonal)
- Diagnosis (“DX”) the patient was diagnosed with (using Gyant condition codes)

Ultimately, our goal is to build a ML model that predicts the Diagnosis (DX), based on symptoms and other factors. In the project you can demonstrate doing some or all of the following:
- Perform exploratory analysis and visualization of data 
- Build one or more ML models on the data
- Select the best model, and report its performance and error analysis
- Perform feature selection to find most salient features
- Explore ways to deal with unbalanced data
- Try using external ML classifies (e.g. IBM Watson)
etc, etc