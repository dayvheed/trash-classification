# trash-classification
The model classifies what kind of trash an image is

Methodology
1. The necessary preprocessing steps were taken - pixel normalization, label encoding
2. A CNN architecture was built for feature extraction
3. The CNN was trained and evaluated. 
4. The CNN was used as a feature extractor, where a Random Forest classifier was placed on top of it for image classification. 
5. The CNN + RF model was trained and evaluated
6. Again, the CNN was used as a feature extractor. But this time, an SVC sat on top of it.
7. The CNN + SVM model was trained and evaluated. 

Results
1. CNN only had an accuracy of 68.44%
2. CNN + RF had an accuracy of 71.00%
3. CNN + SVC had an accuracy of 75.87% 

Discussion
Interestingly, the CNN + SVC produced better results. This goes to show that sometimes, classical methods can produce good results that NN. 
They get really powerful when they are combined with a NN to serve as an inital  feature extractor. 
It was observed that the models generally classified glass as plastic. The confusion could be explained as the images of plastic and glass are closely alike. 

Further work could be an attempt to explore transfer learning approaches especially models such as ResNet, VGGNet and MobileNet. 

If you have any queries, feel free to let me know. 