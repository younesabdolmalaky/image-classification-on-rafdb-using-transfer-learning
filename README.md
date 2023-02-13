# image-classification-on-rafdb-using-transfer-learning
This project focuses on classifying images using various state-of-the-art convolutional neural network (CNN) models. In this report, we compare the performance of four different models: EfficientNetV2L, ResNet152v2, ResNet50, and Inception ResNet.
## About datasets
### Real-world Affective Faces Database
#### Details
Real-world Affective Faces Database (RAF-DB) is a large-scale facial expression database with around 30K great-diverse facial images downloaded from the Internet. Based on the crowdsourcing annotation, each image has been independently labeled by about 40 annotators. Images in this database are of great variability in subjects' age, gender and ethnicity, head poses, lighting conditions, occlusions, (e.g. glasses, facial hair or self-occlusion), post-processing operations (e.g. various filters and special effects), etc. RAF-DB has large diversities, large quantities, and rich annotations, including:

29672 number of real-world images,

a 7-dimensional expression distribution vector for each image,

two different subsets: single-label subset, including 7 classes of basic emotions; two-tab subset, including 12 classes of compound emotions,

5 accurate landmark locations, 37 automatic landmark locations, bounding box, race, age range and gender attributes annotations per image,

baseline classifier outputs for basic emotions and compound emotions.

To be able to objectively measure the performance for the followers' entries, the database has been split into a training set and a test set where the size of training set is five times larger than test set, and expressions in both sets have a near-identical distribution.
##### we use single-label subset 
#### Sample Images
![RAF-DB](https://user-images.githubusercontent.com/75095471/218441919-c18f9d1f-08c7-4a3e-af4f-f52f38f322f3.png)

## Model Architecture
We use four different models in this project: EfficientNetV2L, ResNet152v2, ResNet50, and Inception ResNet. All the models are pre-trained on the ImageNet dataset and are fine-tuned on our dataset to obtain better performance.

## Model Comparison for Image Classification
In this project, several state-of-the-art models were trained on an image classification dataset and their performance was compared. The models used were:
EfficientNetV2L - ResNet152v2 - ResNet50 - Inception ResNet

The results of the models' precision on the image classification task are summarized in the table below:

<table>
  <tr>
    <th>Model Name</th>
    <th>Precision</th>
  </tr>
  <tr>
    <td>EfficientNetV2L</td>
    <td>74%</td>
  </tr>
  <tr>
    <td>ResNet152v2</td>
    <td>78%</td>
  </tr>
  <tr>
    <td>ResNet50</td>
    <td>79%</td>
  </tr>
  <tr>
    <td>Inception ResNet</td>
    <td>82%</td>
  </tr>
</table>

As shown in the table, the Inception ResNet model performed the best among all models, achieving an impressive precision of 82%. The ResNet50 model also performed well with a precision of 79%. On the other hand, the EfficientNetV2L model had the lowest precision of 74%.

It is important to note that these results should not be the sole criteria for selecting a model for a specific task as other factors such as computational cost, memory usage, and inference time should also be considered.

In conclusion, this project demonstrated the performance comparison of several popular image classification models and highlighted the importance of considering multiple factors when selecting a model for a specific task.



