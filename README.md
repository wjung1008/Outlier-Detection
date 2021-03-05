# Outlier-Detection
Surface Crack Outlier Detection using Variation Auto-Encoder (VAE)

## The biggest advantage of using outlier detection is utilizing unbalanced dataset to train the network.
* By training the model only with normal images without cracks, the network is trained to reconstruct an image without any cracks.

![image](https://user-images.githubusercontent.com/60275617/110174186-bf871200-7dcd-11eb-868d-df9d2fe1445f.png)
#### Figure 1. Original image (Left) and Reconstructed image (right)

* So, when an image with crack is input to the network, there will be discrepency between the original image and the reconstructed image.

![image](https://user-images.githubusercontent.com/60275617/110174791-aaf74980-7dce-11eb-81b2-80b3e74fd3c3.png)
#### Figure 2. Checking the discrepency between the original image and the reconstructed image on images without cracks

![image](https://user-images.githubusercontent.com/60275617/110174888-d9752480-7dce-11eb-845a-9264d0f34924.png)
#### Figure 3. Visualize the original image and the reconstructed image

* Hence, we are able to classify images with cracks and images without cracks.

## When the model is tested with the images with cracks:
![image](https://user-images.githubusercontent.com/60275617/110175081-2ce77280-7dcf-11eb-8420-4f3e08aa4ad5.png)
#### Figure 4. Checking the discrepency between the original image and the reconstructed image on images with cracks

* As anticipated, most of the images are well above the threshold.

![image](https://user-images.githubusercontent.com/60275617/110175192-5ef8d480-7dcf-11eb-89cf-2577276714a3.png)
#### Figure 5. Visualize the original image and the reconstructed image

[Surface Crack Dataset](https://www.kaggle.com/arunrk7/surface-crack-detection)
[Alibi detect](https://docs.seldon.io/projects/alibi-detect/en/latest/index.html)
[Reference](https://www.youtube.com/watch?v=RJ4oB6MWTsA&ab_channel=%EB%B9%B5%ED%98%95%EC%9D%98%EA%B0%9C%EB%B0%9C%EB%8F%84%EC%83%81%EA%B5%AD)




