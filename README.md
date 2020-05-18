# Mask R-CNN for Skin Detection and Segmentation
Instance segmenting more than 2 classes in an image, where image dataset is from publicly available data, for annotation we are using VGG annotator latest version Here we defined 2 classes :
• Acne 
• Skintag

Below are the examples for model's accuracy
# Acne

![](/Detected%20Skin%20images/acne.jpg)

![](/Detected%20Skin%20images/acne1.jpg)

# Skintag
![](/Detected%20Skin%20images/skintag.jpg)
![](/Detected%20Skin%20images/skintag1.jpg)
![](/Detected%20Skin%20images/skintag2.jpg)
 
# Train a new model starting from pre-trained COCO weights
python skin.py train --dataset=/path/to/datasetfolder --weights=coco

# Resume training a model that you had trained earlier
python skin.py train --dataset=/path/to/datasetfolder --weights=last

