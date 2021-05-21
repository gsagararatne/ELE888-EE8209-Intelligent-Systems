# ELE888-EE8209---Intelligent-Systems
A current course I'm studying at Ryerson University where I learn about Machine Learning and implement concepts in MATLAB labs.

## Lab1: Bayesian Decision Theory
During this lab MATLAB was used to find probabilities using sepal length and sepal width for Iris Setosa and Iris Versicolour. The objectives were to find prior probability, mean, standard deviation, and posterior probability which was different depending on which data value was given. The prior probability for each class was 0.5 since there were two classes, and it is known that the prior probabilities must be split equally and equal 1 when added. Using the posterior probabilities and a single discriminant function built from the posterior probabilities, predictions on whether a data value belonged to class ⍵1 or  ⍵2 could be made. Looking for the optimal threshold was also important since it sets up boundaries to explore through the raw data to determine if feature data values would belong to class ⍵1 or  ⍵2. The optimal threshold values were found to be 3.098 cm for the sepal width and 5.456 cm for the sepal length, which correspond to the point along both distributions where error is at a minimum. This is also important because when looking at the threshold there may be penalties associated with the posterior probabilities to make it so that a ⍵2 could fall under ⍵1 instead since the boundary acts like it is more skewed to the righter region instead meaning there would be a wider ⍵1 region. Overall this lab allowed for better understanding of MATLAB to process statistical analysis. 

ZZZ
Figure x.x. Sepal Width in Cm for Iris Setosa and Iris Versicolour

ZZZ
Figure x.x. Sepal Length in Cm for Iris Setosa and Iris Versicolour

ZZZ
Figure x.x. x1 vs x2 with Threshold Boundary Lines (red = ⍵1, black = ⍵2) 

## Lab2: Linear Discriminant Functions
When using training data for the purposes of assisting with the evaluation and then classification of data within a set, the more samples used the better the field of view and overall representation of the data there is. By having a better representation of the data, a better classification boundary between the classes can be created, since with more training data points the average of each class becomes more accurate as well as extremities in features for each class are more present. The result of having a better classification boundary between the classes is higher accuracy and less error, meaning less misclassification of the data. In this lab, it was clear that dedicating 70% of the data for training was better for a clearer divider of the data than dedicating 30% of the data for training, even though in both cases there was no misclassification of the data as the accuracy was 1 for both classes. This is evident in Figures 1 and 2, as the majority of data for each class was further from the line of the linear classifier when using 70% of the data for training, meaning that the data was more clearly separable. 

---ADD MORE---

ZZZ
Figure x.x. 

ZZZ
Figure x.x. 

ZZZ
Figure x.x. 

ZZZ
Figure x.x. 

## Lab3: Multilayer Neural Networks
The objective of this lab was to implement a multi-layer neural network using the back propagation algorithm to classify sets of linearly non-separable data. This was done by constructing a 2-2-1 neural network (2 inputs, 2 hidden neurons, 1 output) using the batch back propagation algorithm to first solve the classical XOR problem and then to classify a larger set of wine data. 

While observing how the initial weight vectors were chosen by using the rand() function it was clear that randomization affected the amount of epochs required for convergence, since there were times where the initial weight vectors were closer to the actual final weight vectors used to achieve the desired results; this allowed for much quicker convergence. On the other hand, when the randomized initial weight vectors were much different than the final weight vectors, convergence took longer and more epochs were needed to achieve the desired results of the XOR problem and the wine data classification.

Through both parts of this lab, it was discovered that 100% accuracy was much easier to achieve with the XOR problem than the wine data classification. This was likely due to the fact that the XOR problem was very limited in possible inputs and the desired outputs associated with each pair were exact. This contributed to the XOR problem requiring less epochs on average to meet the error threshold .

An important part of the way the output was calculated for both cases in this lab was the activation function. The activation function in machine learning neural networks controls how well the algorithm learns the provided training dataset, and heavily defines and influences the predictions that the algorithm can make. In future experiments, it would be interesting to alternate the activation function in the model to observe how they impact the characteristics of the results, including convergence and accuracy.

Overall, this lab experiment was successful as the 2-2-1 neural network that was implemented to solve each problem was able to produce reasonably accurate results.


## Lab4: Unsupervised Learning
ZZZ
Figure 2.3 

ZZZ
Figure 2.4

ZZZ
Figure 2.5 

ZZZ
Figure 2.6

By comparing the plots in RGB space in Figures 2.3 and 2.4, it is evident that the colour scheme in the two images is slightly different. In the first plot corresponding to the first mean run, there are 5 distinct colours of light green, light blue, grey, dark purple, and pink. On the other hand, the second plot also has 5 colours but instead of a grey colour there is a lighter purple. There is also more blue present in the second run of mean values and less of the pink colour. These differences translate to the photos in Figures 2.5 and 2.6, where the second mean run with the lighter purple colour and more blue seems to be closer to the actual house image than the first run. For example, the door in the second run has a blue colour, which corresponds to the actual colour of the door in the reference image, while in the photo of the second run the door is grey. As mentioned before, there is a large amount of grey in the RGB plot for the first run, so it makes sense that there is grey instead of blue in this image for the door. Additionally, in the second run, the roof is much closer in colour accuracy to the actual roof, corresponding to the light purple colour present in the second RGB plot. However, this colour is not present at all in the first RGB plot, so it attempts to use the pink and dark purple to make up the roof. Overall, it is clear that the second run of mean values was more accurate to the original image. 

