# R for Bio Data Science Project - Group 17

## Contributors

| Name                                       | Student number | GitHub username |
|--------------------------------------------|----------------|-----------------|
| Tijn Friederich                            | s262015        | DTUTWFriederich |
| Caroline Aroha Schmidt Morthorst Rasmussen | s215120        | CR-Biotech      |
| Andrea López Martinez                      | s243342        | andrealomar     |
| Marc Magem Planàs                          | s253362        | mmagemm         |

## Dataset

The dataset used for this project was obtained from the Vanderbilt University Department of Biostatistics data repository (https://hbiostat.org/data/). After a comprehensive search, it was selected for its manageable size, untidiness, and potential for extracting relevant biological insights, despite its historical origins.

The data comes from a clinical trial conducted around 1980 (Byar & Green, 1980; PMID: 7013866). During the 1970s and 1980s, high-dose estrogen therapy was used as a conventional hormonal therapy to suppress serum testosterone levels and diminish prostate tumours progression.

However, this treatment led to some side effects, being cardiovascular complications the most prevalent and severe. The objective of this project is to study the relationship between estrogen therapy, patient characteristics, and cardiovascular events, and assess how treatment impacted survival.

Our dataset contains N = 502 observations across 18 variables:

|Variable | Description                                    | Type                                                              |
|---------| -----------------------------------------------| ------------------------------------------------------------------|
| `patno` | Patient identification number                  | Numeric     |
| `stage` | Clinical cancer stage                          | Categorical (`3` = locally advanced, `4` = metastatic) |
| `rx`    | Estrogen treatment                             | Categorical (`placebo`, `0.2 mg`, `1.0 mg`, `5.0 mg`) |
| `dtime` | Months of follow-up                            | Continuous  |
| `status`| Survival status                                | Categorical (`alive`, `dead - prostatic ca`, `dead - heart or vascular`, `dead - cerebrovascular`, `dead - pulmonary embolus`, `dead - other ca`, `dead - respiratory disease`, `dead - other specific non-ca`, `dead - unspecified non-ca`, `dead - unknown cause`) |
| `age`   | Age at tiral start                             | Continuous  |
| `wt`    | Weight index                                   | Continuous  |
| `pf`    | Performance                                    | Categorical (`normal activity`, `in bed < 50% daytime`, `in bed > 50% daytime`, `confined to bed`) |
| `hx`    | History of cardiovascular disease              | Binary (`0` = no, `1` = yes) |
| `sbp`   | Systolic blood pressure                        | Continuous  |          
| `dbp`   | Diastolic blood pressure                       | Continuous  |
| `ekg`   | Baseline electrocardiogram reading             | Categorical (`normal`, `benign`, `rhythmic disturb & electrolyte ch`, `heart block or conduction def`, `heart strain`, `old MI`, `recent MI`) |
| `hg`    | Serum hemoglobin                               | Continuous  |
| `sz`    | Size of primary tumor                          | Continuous  |
| `sg`    | Combined index of stage and histological grade | Ordinal (score) |
| `ap`    | Serum prostatic acid phosphatase               | Continuous  |
| `bm`    | Presence of bone metastases                    | Binary (`0` = no, `1` = yes) |
| `sdate` | Date of study                                  | Numeric     |


## Load data
