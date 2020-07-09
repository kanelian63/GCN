# Graph Neural Networks


# Graphing
![Graphing](https://user-images.githubusercontent.com/59387983/84757222-d9de4d00-affe-11ea-8dd0-aa6fee084ca0.PNG)
Most machine learning algorithms assume that the input data is in Euclidean space. That is, input data, such as statistical data or images, should be able to be expressed in the form of vectors. However, data represented by objects and relationships between objects, such as social networks, relational databases, and molecular structures, are basically represented by graphs as shown above.


# Theory
![function](https://user-images.githubusercontent.com/59387983/84757355-03977400-afff-11ea-9c3a-9be589460715.PNG)

Since data must be expressed to contain relationship information between all nodes, these information are expressed in an Adjacency matrix.

![tjfaud](https://user-images.githubusercontent.com/59387983/84757357-04c8a100-afff-11ea-9779-327fbe18498d.PNG)

If the above expression is used immediately, the scale of the feature vector is completely changed during the calculation because A is not normalized. Therefore, we use the adjacency matrix A normalized as follows:

![normalized admatrix](https://user-images.githubusercontent.com/59387983/84757359-04c8a100-afff-11ea-8e61-719db790045a.PNG)

The D matrix is a matrix indicating how many nodes are connected, including itself, and can be easily obtained by adding the elements of each row of the adjacent matrix A. We can find the normalized adjacency matrix by finding the inverse of the D matrix obtained and multiplying it before and after the adjacency matrix A.

![Diagonal Node Degree Matrix](https://user-images.githubusercontent.com/59387983/84757368-072afb00-afff-11ea-8fa9-35f339e36acb.PNG)

# Inputs
![input](https://user-images.githubusercontent.com/59387983/84757361-05613780-afff-11ea-813c-c055e14cb2f8.PNG)

The input data is processed in the above format, and the weight matrix of filters is implemented by continuously multiplying the matrix by the filter matrix.

# Lecture
![다운로드](https://user-images.githubusercontent.com/59387983/84760363-dd73d300-b002-11ea-9e4d-2db98c23ce7d.png)

https://www.youtube.com/watch?v=YL1jGgcY78U&list=PLSAJwo7mw8jn8iaXwT4MqLbZnS-LJwnBd&index=29
