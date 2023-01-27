# X-Ray_pneumonia__phase_4

**Authors:** [Ilan Haskel](https://www.linkedin.com/in/ilan-haskel-86280812b/), [Justin James](https://www.linkedin.com/in/jtdjames/), [Roshni Janakiraman](https://www.linkedin.com/in/roshni-janakiraman/), [Leif Schultz](https://www.linkedin.com/in/leifschultz/), and [Brandon Sienkiewicz](https://www.linkedin.com/in/brandon-sienkiewicz-data-science/)

## Project Overview

Using data from the Guangzhou Women and Children's Medical Center, we built a Neural Network model to classify chest X-ray images as either healthy, viral pneumonia, or bacterial pneumonia. Our model can be used to help pediatric hospitals quickly and accurately diagnose pneumonia, improving patient outcomes and hospital resource allocation.

## I. Business Understanding

**Stakeholder**: Children's Hospital C-Suite

### Business Case

Pneumonia is the primary cause of childhood hospitalization [[1]](https://pubmed.ncbi.nlm.nih.gov/25695124/). Pediatric pneumonia is lethal without proper treatment, accounting for 14% of all childhood deaths [[2]](https://www.who.int/en/news-room/fact-sheets/detail/pneumonia). As the disease progresses, pediatric pneumonia requires a significant amount of hospital resources for treatment and poses a high cost of care for patients [[3]](https://www.sciencedirect.com/science/article/pii/S2352646719300274). Therefore, timely and accurate diagnosis of pneumonia is critical for successful treatment.

However, there are complications to obtaining a quick and accurate pnuemonia diagnosis. To determine the right treatment protocol, doctors need to determine whether pneumonia is *bacterial* or *viral* [[4]](https://www.nejm.org/doi/full/10.1056/NEJMoa1405870), which cannot be determined solely based on clinical features [[5]](https://pneumonia.biomedcentral.com/articles/10.15172/pneu.2014.5/464#Sec4).

Although chest X-ray evaluation is considered the gold standard for diagnosing pneumonia [[6]](https://academic.oup.com/cid/article/31/2/347/293404), this method has key limitations. Chest X-ray interpretation is labor intensive and prone to human error [[7]](https://www.thelancet.com/journals/landig/article/PIIS2589-7500(21)00106-0/fulltext). There is a shortage of radiologists with the required training for this task [[8]](https://www.ajronline.org/doi/full/10.2214/AJR.12.10375).  Even for experienced radiologists, reliability and accuracy scores range from 38-76% [[9]](https://www.ajronline.org/doi/10.2214/AJR.19.21521).

Artificial Intelligence can improve the process of diagnosing pneumonia accurately and efficiently. Computer aided diagnostic systems have shown reasonable accuracy in detecting infections from X-rays. When aided by AI, radiologists are significantly more accurate at diagnosing pneumonia compared to unassisted [[10]](https://www.thelancet.com/journals/landig/article/PIIS2589-7500(21)00106-0/fulltext). Computerized models can increase the overall efficiency of the diagnostic process by reducing work burden on radiologists. Quicker detection allows doctors to start treatment protocol sooner, which can reduce severity and duration of illness.  

### Goals of Current Project

We sought to create and optimize image classification models that could diagnose pneumonia from chest X-ray images. Our specific goals for these models were to:

1. Accurately distinguish pneumonia *positive* cases from *negative cases*
2. Given a new chest X-Ray image, accurately classify case as *bacterial pneumonia,* *viral pneumonia* or *non-pneumonia*
3. Minimize *false negative* diagnoses, given lethality of pneumonia without proper treatment
4. Increase the efficiency of the chest X-ray diagnostic process by deploying a quick, simple-to-run testing system.

## II. Data Understanding

### Data Source:

Originating from a larger study [[11]](https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5), this project's data consists of Chest X-Ray Images from pediatric patients (ages 1-5) at Guangzhou Women and Children’s Medical Center, taken as part of patients’ routine clinical care. We used a subset of this data, obtained from [Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), and reorganized the data into 3 folders (Bacterial/Viral/Normal).

The current dataset consists of 5,863 Chest X-Ray images (JPEG).

### Data Quality: 

In the [original study](https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5), X-ray images were screened for quality control and graded by two expert physicians before being cleared for training the AI system. 

### Data Exploration:

### 







## III. Data Preparation

Our first steps in preparing the data involved resizing the images by dividing by 255. Next we one hot encoded the labels in order for our mode to classify multiple categories. We then split the data into a training set, a validation set, and a test set, in order to begin modeling.

## IV. Data Modeling

One of the most important factors in choosing our model was the model’s ability to limit false negatives. Even if it made our model slightly less accurate overall it was important our model rarely classified pneumonia x-rays as healthy x-rays. 

## V. Model Evaluation and Deployment

### Final Model Evaluation

#### Healthy vs. Pneumonia



Our model is exceptionally good at identifying whether someone is healthy or not. It can with 95? percent accuracy determines whether or not someone has pneumonia. In addition this model only classified a pneumonia x-ray as healthy ??? percent of the time.

#### Bacterial vs. Viral



One of the other advantages to our model is its ability to classify an x-ray as either a viral pneumonia infection or a bacterial infection. Not only does it classify someone as being healthy or having pneumonia it can also determine what type of pneumonia the person has. Our model was able to accurately predict bacterial pneumonia ??? percent of the time and was ??? percent accurate in predicting viral pneumonia.

## VI. Conclusion 