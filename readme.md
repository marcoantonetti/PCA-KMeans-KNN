Written by me not AI
Exercise 1:
In this proyect for university machine learning lecture course of UTN - Buenos Aires, I was given a wine data set and I had to apply non supervised algorithms to classify them.
The notebook is in spanish and it has comments at the end.

Dependent variable Y: Class of wine. 
Independent Variable X: A vector of 13 dimensions such as % alcohol, tanins, acidity, magnesium, etc
Conclusion: The wines classified better in 3 classes.

First I normalized the vector's dimensions data to a mean of 0 and standard variation of 1. So that we can compare them despite there measure unit.

Then I applied PCA to reduce the dimensions to just 2. PC1 (36.2%) and PC2 (19,2%). And analize which dimensions dominated PC1 and PC2

I trained test split the data to a test_size of 0.29. 0.29 got me a better accurracy.

KMeans: The best adjusted score was for a k = 3. For this algorithm, the wines classified better in 3 clases / clusters.

Affinity Propagation: This algorithms finds the best suited quantity of clusters by itself. Accuracy > 90%. Providing k = 7 clusters / clases. However a rand score 0.42 was observed

Because the dataset was already classified in 3 classes I already knew that k = 3 should have been the right cluster number.

Exercise 2:
Face Recognition
I was given a data set of images of faces and their names and I had to applied non supervised and supervised algorithms to classified them by their name/face. Only people with 70 images of their face where used.

Sample: 1288
Independent Variable X: Vector of 1200 dimensions which are euclidian distances between two specific points of a person's face.
Dependent Variable Y: Person name. The owner of the face.

PCA: Reduced the 1200 dimensions to just 59 Vectors
Trained test split data: test size of 0.20

Supervised algorithms
Logistic Regression: Accuracy of 0.81
Knn: Accuracy of 0.72 with neighbors (n) = 8. N = 8 gave me the best accuracy
SVM: Accuracy of 0.84 with a non-lineal kernel (rbf) and a decision boundary margin of 1. This gave me the best accuracy.

Conclusion: Logistic regression and SVM algorithms over a PCA allowed me to create a face recognition model with an accuracy of > 0.80
