
# Manual {#manual}

_Important_ features and technical details are described in this chapter.

## Registration {#register}
<span class='textintro'>Users are required to LOG IN using an existing Facebook or Google account, or can sign up for a login using the “SIGN UP” button. Your gmail account through your university may be used for authentication. </span>

<div class="marginnote">

<span class='texta'>**a. Login**</span> is initially active where you may use the 3rd party login or your account.

<span class='textb'>**b. Sign-Up** </span> click on this tab to register for an account.

<span class='textc'>**c. 3rd party login**</span> click on the facebook or google icons to login using your credentials from your account.

<span class='textd'>**d. Forget password**</span> to reset your password. You are required to provide the email associated with your account. 

<span class='texte'>**e. Proceed**</span> to the web app by clicking on the orange button.

</div>

<a href="static/login.PNG" target="_blank"><img src="static/login.PNG" style="width: 60%"></a>

## Data Preparation
Standard input  using excel, a widely accessible format, is required for COMETS Analytics and can be created from various data file formats. Data Integrity checks for input errors provide meaningful and actionable messages to users for analyses to proceed. See chapter \@ref(input) [Step 1 Data Preparation]


### Create Input

## Harmonization details {#details-harmonize}
The names of metabolites  from each cohort has been mapped  or harmonized to a common name. This important stage facilitates comparison of metabolites across different studies that use different platforms and/or naming conventions.

### Preharmonization
Prior to conducting your cohort analyses, xxx. 

## Integrity checks {#integrity}
Prior to running the models for analyses, CA conducts multi-level checks to ensure data and models are appropriate for analyses.

### Data
The following conditions are checked:

* Missing Subject ID or Metabolite ID in the _VarMap_ sheet
* Subject ID or Metabolite ID provided in _VarMap_ sheet do not correspond to a column in _Metabolites_ and _SubjectData_ sheets, respectively
* Metabolites IDs in _Metabolites_ and _SubjectMetabolites_ sheets do not match
* Subject IDs in _SubjectData_ and _SubjectMetabolites_ sheets do not match

If any of the following conditions failed, the analyses will be suspended and corrections to the data are required. The data integrity checks will also flag the following but will proceed with the analyses:

* Number of subjects in _SubjectData_ and _SubjectMetabolites_ sheets do not match
* Metabolite abundances from _SubjectMetabolites_ contains duplicate columns (metabolites) or rows (subjects)
* There are duplicate subject IDs in the subject information _SubjectData_ sheet
* There are duplicate metabolite IDs in the metabolite information _Metabolites_ sheet

### Models
Models are also validated using the CARET package.


## Correlation Analyses

### Details

### Output

<!--
## Linear Models

### Details

### Output


## Logistic Models

### Details

### Output


## Meta-Analyses

### Details

### Output

-->
