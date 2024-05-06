
# Mushroom Species Classification

## Project Overview
to do

## Dataset
**'inatur_urls.csv'** exported from iNaturalist with the following parameters:
- **Categories**: Fungi including Lichens
- **Place**: Leningrad Oblast, Russia
- **Data Quality**: Only Research Grade observations from iNaturalist

Data collected with custom script ('**get_data_inaturalist.ipynb**')  
Labels are folder names.  
Only species with more than 99 observations were selected for this dataset (one photo = one observation)

## Training model - `mushrooms_classification.ipynb`

### Overview
Jupyter notebook contains the process of training a MobileNet_v2 model for classifying 21 different mushroom species. The pre-trained weights (`MobileNet_V2_Weights`) from ImageNet are utilized, which originally achieved 71.878% top-1 accuracy and 90.286% top-5 accuracy on the ImageNet-1K dataset.

### Performance
On our mushroom dataset, the model achieved approximately 93% accuracy, demonstrating the effectiveness of transfer learning for specialized image classification tasks.

### Training Details
- **Optimizer**: SGD with learning rate of 0.01 and momentum of 0.9.
- **Learning Rate Scheduler**: CosineAnnealingLR, adjusted across epochs to optimize learning.



