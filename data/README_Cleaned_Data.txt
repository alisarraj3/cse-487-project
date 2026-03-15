 sex: 1 for female and 0 for male.
age: of the patient.
classification: covid test findings. Values 1-3 mean that the patient was diagnosed with covid in different degrees. 4 or higher means that the patient is not a carrier of covid or that the test is inconclusive.
patient type: type of care the patient received in the unit. 1 for returned home and 0 for hospitalization.
pneumonia: whether the patient already have air sacs inflammation or not.
pregnancy: whether the patient is pregnant or not.
diabetes: whether the patient has diabetes or not.
copd: Indicates whether the patient has Chronic obstructive pulmonary disease or not.
asthma: whether the patient has asthma or not.
inmsupr: whether the patient is immunosuppressed or not.
hypertension: whether the patient has hypertension or not.
cardiovascular: whether the patient has heart or blood vessels related disease.
renal chronic: whether the patient has chronic renal disease or not.
other disease: whether the patient has other disease or not.
obesity: whether the patient is obese or not.
tobacco: whether the patient is a tobacco user.
usmr: Indicates whether the patient treated medical units of the first, second or third level.
medical unit: type of institution of the National Health System that provided the care.
intubed: whether the patient was connected to the ventilator.
icu: Indicates whether the patient had been admitted to an Intensive Care Unit.
date died: If the patient died indicate the date of death, and 9999-99-99 otherwise.

-------------------------New aditions/changes:----------------------
New Column: survived? 1 yes, 0 no.
Yes/No?:  now yes still 1, and 0 means no for all binary columns and -1 means unknown, replaced the 2 for 0 because it is more intuitive and stays binary.
sex column now: 1 female, 0 male
patient type column: 1 for returned home, 0 for hostitalization
Everything except these columns was modified: AGE, CLASIFFICATION_FINAL, DATE_DIED, USMER, and MEDICAL_UNIT

------------------TWO NEW .CSV-----------------

cleaned_covid_positive_and_negative.CSV -> cleaned data indicating all entries

    count: confirmed non-covid/unknown -> 656596
           confmirmed covid  -> 391979

cleaned_covid_positive_only.csv -> filtered out the non-covid or unknown patients

    count: confirmed non-covid/unknown -> 0
           confmirmed covid  -> 391979
