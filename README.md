# Image-Matting-with-Bayesian-Method
Image Matting separates an image into two parts - background and foreground. While a major section of foreground can be marked readily, the detailing becomes relatively difficult, and this is where the Bayesian method comes in. It is implemented over trimaps, which are grayscale images with three sections, black pixels - background, white pixels - foreground, gray pixels - undecided region. 
<img src="https://github.com/shrutipgupta/Image-Matting-with-Bayesian-Method/blob/main/GT18.png">

The method segregates the pixels in the unknown region into foreground or background sections based on their likelihood of being the part of either. The result is an alpha matte, which is having values different from white and black, and impart a sense of overlap or mixing between the background and foreground, giving a more realistic feel to the image. It can be seen here:
<img src="https://github.com/shrutipgupta/Image-Matting-with-Bayesian-Method/blob/main/Predicted_alpha_matte.png">

However, the expected ground truth is as follows: 
<img src="https://github.com/shrutipgupta/Image-Matting-with-Bayesian-Method/blob/main/Ground_truth.png">

The foreground extracted from the image with predicted alpha matte is: 
<img src="https://github.com/shrutipgupta/Image-Matting-with-Bayesian-Method/blob/main/Extracted_with_pred_alpha_matte.png">

While that extracted with the ground truth is:
<img src="https://github.com/shrutipgupta/Image-Matting-with-Bayesian-Method/blob/main/Extracted_with_ground_truth.png">

Note: In case the .ipynb file does not load, it can be downloaded and opened with Colab or Jupyter Notebook. 
