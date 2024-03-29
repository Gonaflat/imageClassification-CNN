# imageClassification
Image Classification - COVID 
# Background
The 2019 novel coronavirus (COVID-19) presents several unique features. While the diagnosis is confirmed using polymerase chain reaction (PCR), infected patients with pneumonia may present on chest X-ray and computed tomography (CT) images with a pattern that is only moderately characteristic for the human eye Ng, 2020. COVID-19’s rate of transmission depends on our capacity to reliably identify infected patients with a low rate of false negatives. In addition, a low rate of false positives is required to avoid further increasing the burden on the healthcare system by unnecessarily exposing patients to quarantine if that is not required. Along with proper infection control, it is evident that timely detection of the disease would enable the implementation of all the supportive care required by patients affected by COVID-19.

In late January, a Chinese team published a paper detailing the clinical and paraclinical features of COVID-19. They reported that patients present abnormalities in chest CT images with most having bilateral involvement Huang 2020. Bilateral multiple lobular and subsegmental areas of consolidation constitute the typical findings in chest CT images of intensive care unit (ICU) patients on admission Huang 2020. In comparison, non-ICU patients show bilateral ground-glass opacity and subsegmental areas of consolidation in their chest CT images Huang 2020. In these patients, later chest CT images display bilateral ground-glass opacity with resolved consolidation Huang 2020.
# Target
Binary classification - images are divided into 2 classes (0 - absence of pneumonia and its signs, 1 - presence of pneumonia and its signs). The goal is to achieve quality classification on future images.
# What was applied?
- The data were split into training and test sets (including training labels and test labels).
- Image augmentation was performed, including parameters such as:
  - shear_range = 0.2,
  - zoom_range = 0.2,
  - horizontal_flip = True
# What models and evaluation were applied?
- CNN
- Keras Tuner for hyperparameters
- Evaluation:
  - Test Accuracy, Test Loss
- Vizualization:
  - Train Loss, Train accuracy curve,
  - Test Loss, Test accuracy curve,
  - Confusion Matrix,
  - Roc Curve
