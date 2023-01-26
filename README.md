# X-Ray_pneumonia__phase_4

Project Overview

## I. Business Understanding

**Stakeholder**: Children's Hospital C-Suite

### Business Case

Pneumonia is the primary cause of childhood hospitalization.[^1^](https://pubmed.ncbi.nlm.nih.gov/25695124/) Pediatric pneumonia is lethal without proper treatment, accounting for 15% of all childhood deaths.[^2^](https://www.who.int/en/news-room/fact-sheets/detail/pneumonia)  As the disease progresses, pediatric pneumonia requires a significant amount of hospital resources for treatment and poses a high cost of care for patients.[^3^](https://www.sciencedirect.com/science/article/pii/S2352646719300274) Therefore, timely and accurate diagnosis of pneumonia is critical for successful treatment.

There are many complications to quickly and accurately diagnosing pneumonia. To determine the right treatment protocol, doctors need to determine whether pneumonia is *bacterial* or *viral*.[^4^](https://www.nejm.org/doi/full/10.1056/NEJMoa1405870) Clinical features alone are not sufficient to accurately diagnose pneumonia.[^5^](https://pneumonia.biomedcentral.com/articles/10.15172/pneu.2014.5/464#Sec4)

Chest X-Ray evaluation is the current gold standard for diagnosing pneumonia.[^6^](https://academic.oup.com/cid/article/31/2/347/293404) However, this method has key limitations. Chest X-ray interpretation is labor intensive and prone to human error; there is a shortage of radiologists with sufficient training to read chest X-rays.[^7^](https://www.thelancet.com/journals/landig/article/PIIS2589-7500(21)00106-0/fulltext) Even for experienced radiologists, reliability and accuracy scores range from 38-76%.[^8^](https://www.ajronline.org/doi/10.2214/AJR.19.21521)

Artificial Intelligence can improve the process of diagnosing pneumonia accurately and efficiently. Computer aided diagnostic systems have shown reasonable accuracy in detecting infections from X-rays. When aided by AI, radiologists are significantly more accurate at diagnosing pneumonia compared to unassisted.[^9^](https://www.thelancet.com/journals/landig/article/PIIS2589-7500(21)00106-0/fulltext) Computerized models can increase the overall efficiency of the diagnostic process by reducing work burden on radiologists. Quicker detection allows doctors to start treatment protocol sooner, which can reduce severity and duration of illness.  

### Goals of Current Project

We sought to create and optimize image classification models that could diagnose pneumonia from chest X-ray images. Our specific goals for these models were to:

1. Accurately distinguish pneumonia *positive* cases from *negative cases*
2. Given a new chest X-Ray image, accurately classify case as *bacterial pneumonia,* *viral pneumonia* or *non-pneumonia*
3. Minimize *false negative* diagnoses, given lethality of pneumonia without proper treatment
4. Increase the efficiency of the chest X-ray diagnostic process by deploying a quick, simple-to-run testing system.

## II. Data Understanding

### Data Description

### Data Exploration

### Data Quality

## III. Data Preparation

## IV. Data Modeling

## V. Model Evaluation and Deployment

## VI. Conclusion 