# Improving Breast Cancer Detection using Ultrasound and Mammogram Images
- The dataset contains normal and mask images in each category(Ultrasound and Mammogram)
- ImageDataGenerator is used for Image augmentation purpose.
- As it is a Segmentation problem, the model used here is a UNET model.
- The evaluation metrics used are IoU and Dice coefficient.

The steps invoved are:
- Augmented ultrasound images are used to train UNET model.
- Then this model is modified and is trained on Mammogram images.
- In this way the knowledge gained from ultrasound images is transferred(Transfer Learning) to the model trained on mammgoram images and vice-versa.

After Transfer Learning there is an increase in accuracy for mammogram images(88% to 94%) but not for ultrasound images(97% to 95%) since number of mammgoram images are very less as compared to ulrasound images.

Dependecies
- tensorflow
- keras
- numpy
- pandas
- sklearn
- cv2

