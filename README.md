# RANZCR CLiP Catheter-and-Line-Position-Challenge
Using Deep learning models to classify the presence and correct placement of tubes on chest x-rays to save lives

# Overview
**The Royal Australian and New Zealand College of Radiologists (RANZCR) is a not-for-profit professional organisation for clinical radiologists and radiation oncologists in Australia, New Zealand, and Singapore. The group is one of many medical organisations around the world (including the NHS) that recognizes malpositioned tubes and lines as preventable. RANZCR is helping design safety systems where such errors will be caught.**

**In this competition, you’ll detect the presence and position of catheters and lines on chest x-rays. Use machine learning to train and test your model on 40,000 images to categorize a tube that is poorly placed.**

**The dataset has been labelled with a set of definitions to ensure consistency with labelling. The normal category includes lines that were appropriately positioned and did not require repositioning. The borderline category includes lines that would ideally require some repositioning but would in most cases still function adequately in their current position. The abnormal category included lines that required immediate repositioning.**

**If successful, your efforts may help clinicians save lives. Earlier detection of malpositioned catheters and lines is even more important as COVID-19 cases continue to surge. Many hospitals are at capacity and more patients are in need of these tubes and lines. Quick feedback on catheter and line placement could help clinicians better treat these patients. Beyond COVID-19, detection of line and tube position will ALWAYS be a requirement in many ill hospital patients.**

# Data Description

**In this competition, you’ll detect the presence and position of catheters and lines on chest x-rays. Use machine learning to train and test your model on 40,000 images to categorize a tube that is poorly placed.**

**What files do I need?**

You will need the train and test images. This is a code-only competition so there is a hidden test set (approximately 4x larger, with ~14k images) as well.

train.csv contains image IDs, binary labels, and patient IDs.

TFRecords are available for both train and test. (They are also available for the hidden test set.)

We've also included train_annotations.csv. These are segmentation annotations for training samples that have them. They are included solely as additional information for competitors.

Files

train.csv - contains image IDs, binary labels, and patient IDs.

sample_submission.csv - a sample submission file in the correct format

test - test images

train - training images

Columns

>StudyInstanceUID - unique ID for each image

>ETT - Abnormal - endotracheal tube placement abnormal

>ETT - Borderline - endotracheal tube placement borderline abnormal

>ETT - Normal - endotracheal tube placement normal

>NGT - Abnormal - nasogastric tube placement abnormal

>NGT - Borderline - nasogastric tube placement borderline abnormal

>NGT - Incompletely Imaged - nasogastric tube placement inconclusive due to imaging

>NGT - Normal - nasogastric tube placement borderline normal

>CVC - Abnormal - central venous catheter placement abnormal

>CVC - Borderline - central venous catheter placement borderline abnormal

>CVC - Normal - central venous catheter placement normal

>Swan Ganz Catheter Present

>PatientID - unique ID for each patient in the dataset

# Models Used

1. [ResNet50](https://keras.io/api/applications/resnet/#resnet50-function)
2. [XceptionNet](https://keras.io/api/applications/xception/)

[Link to Competition](https://www.kaggle.com/c/ranzcr-clip-catheter-line-classification/overview)

**Do check my Implementations and let me know if any improvements can be made**
