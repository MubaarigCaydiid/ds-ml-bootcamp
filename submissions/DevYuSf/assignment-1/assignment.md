# Assignment one

___

## Question one is

- **Define Machine Learning using a real-life example?.**
Answer:
Machine learning is like computer learning from data which gives you a smarter answer for his own which mean he finds a sample question like your question and gives you the answer that he learns from the data that he already have.
**real example:** you give your machine 2+2 = 4
and someone asked your machine 2+2 he gives 4 because you already told it.
(Reference: [1])

---

## Question two is

- **Compare Supervised Learning and Unsupervised Learning, giving an example of each.**
Answer:
**Supervised learning** is a know data, which mean is already know the ourput of the question for example if you are in a math class and th teacher teaches you 5 times 5 equal to 25 and you rpeat it that data is supervised
**Real World Example:**
when you are using your phone and you need to write your friend a greeting like how are ... before it finished your phone will automatically fill **you** because often when you say: **how are** it will add with **you**.
that is a supervised learning the next word already know or predict.
**Unsupervised learning** is an unknow data or unpredictable data which the machine learns through the actions of the user or you learned your habits
**Real World Example:**
when you are using your phone and usually you type **AsxaapTa waan idin salaamay**
the next time you time **AsxaapTa waan ...** it automatically filled **idin salaamay** because it uses **UnSupervised learning** it learned through your daily habit
(Reference: [2])

---

## Question three is

- **What causes Overfitting? How can it be prevented?**
Asnwer:
**Overfitting** is an undesirable machine learning behavior that occurs when the machine learning model gives accurate predictions for training data but not for new data. When data scientists use machine learning models for making predictions, they first train the model on a known data set. Then, based on this information, the model tries to predict outcomes for new data sets. An overfit model can give inaccurate predictions and cannot perform well for all types of new data.

Why does overfitting occur?
You only get accurate predictions if the machine learning model generalizes to all types of data within its domain. Overfitting occurs when the model cannot generalize and fits too closely to the training dataset instead. Overfitting happens due to several reasons, such as:
•    The training data size is too small and does not contain enough data samples to accurately represent all possible input data values.
•    The training data contains large amounts of irrelevant information, called noisy data.
•    The model trains for too long on a single sample set of data.
•    The model complexity is high, so it learns the noise within the training data.

Overfitting examples
Consider a use case where a machine learning model has to analyze photos and identify the ones that contain dogs in them. If the machine learning model was trained on a data set that contained majority photos showing dogs outside in parks , it may may learn to use grass as a feature for classification, and may not recognize a dog inside a room.
Another overfitting example is a machine learning algorithm that predicts a university student's academic performance and graduation outcome by analyzing several factors like family income, past academic performance, and academic qualifications of parents. However, the test data only includes candidates from a specific gender or ethnic group. In this case, overfitting causes the algorithm's prediction accuracy to drop for candidates with gender or ethnicity outside of the test dataset.

How can you detect overfitting?
The best method to detect overfit models is by testing the machine learning models on more data with with comprehensive representation of possible input data values and types. Typically, part of the training data is used as test data to check for overfitting. A high error rate in the testing data indicates overfitting. One method of testing for overfitting is given below.
K-fold cross-validation
Cross-validation is one of the testing methods used in practice. In this method, data scientists divide the training set into K equally sized subsets or sample sets called folds. The training process consists of a series of iterations. During each iteration, the steps are:

1. Keep one subset as the validation data and train the machine learning model on the remaining K-1 subsets.
2. Observe how the model performs on the validation sample.
3. Score model performance based on output data quality.
Iterations repeat until you test the model on every sample set. You then average the scores across all iterations to get the final assessment of the predictive model.
How can you prevent overfitting?
You can prevent overfitting by diversifying and scaling your training data set or using some other data science strategies, like those given below.
Early stopping
Early stopping pauses the training phase before the machine learning model learns the noise in the data. However, getting the timing right is important; else the model will still not give accurate results.
Pruning
You might identify several features or parameters that impact the final prediction when you build a model. Feature selection—or pruning—identifies the most important features within the training set and eliminates irrelevant ones. For example, to predict if an image is an animal or human, you can look at various input parameters like face shape, ear position, body structure, etc. You may prioritize face shape and ignore the shape of the eyes.
Regularization
Regularization is a collection of training/optimization techniques that seek to reduce overfitting. These methods try to eliminate those factors that do not impact the prediction outcomes by grading features based on importance. For example, mathematical calculations apply a penalty value to features with minimal impact. Consider a statistical model attempting to predict the housing prices of a city in 20 years. Regularization would give a lower penalty value to features like population growth and average annual income but a higher penalty value to the average annual temperature of the city.
Ensembling
Ensembling combines predictions from several separate machine learning algorithms. Some models are called weak learners because their results are often inaccurate. Ensemble methods combine all the weak learners to get more accurate results. They use multiple models to analyze sample data and pick the most accurate outcomes. The two main ensemble methods are bagging and boosting. Boosting trains different machine learning models one after another to get the final result, while bagging trains them in parallel.
Data augmentation
Data augmentation is a machine learning technique that changes the sample data slightly every time the model processes it. You can do this by changing the input data in small ways. When done in moderation, data augmentation makes the training sets appear unique to the model and prevents the model from learning their characteristics. For example, applying transformations such as translation, flipping, and rotation to input images.
(Reference: [3,4])

---

## Question four is

- **Explain how training data and test data are split, and why this process is necessary?.**
Answer:
A very common practice in machine learning is to never use the entire data available to train your machine learning model, but why? We will figure out the solution afterward but let’s first understand, what is data splitting?

Data Splitting

The train-test split is a technique for evaluating the performance of a machine learning algorithm.

It can be used for classification or regression problems and can be used for any supervised learning algorithm.

The procedure involves taking a dataset and dividing it into two subsets. The first subset is used to fit the model and is referred to as the training dataset. The second subset is not used to train the model; instead, the input element of the dataset is provided to the model, then predictions are made and compared to the expected values. This second dataset is referred to as the test dataset.

Components to split

When we decide to split the data, we should know how many splits of data we need. Generally, there are three partitions of data we make, which are:

The Training Set: It is the set of data that is used to train and make the model learn the hidden features/patterns in the data.

The Validation Set: The validation set is a set of data, separate from the training set, that is used to validate our model performance during training.

The Test Set: The test set is a separate set of data used to test the model after completing the training.

Why do we need splitting?

Whenever we train a machine learning model, we can’t train that model on a single dataset or even we train it on a single dataset then we will not be able to assess the performance of our model. For that reason, we split our source data into training, testing, and validation datasets. Now for understanding the need for data split let’s take an example of classroom teaching.

Suppose a mathematics faculty teaches her students about an algorithm. For the explanation the teacher uses some examples, those examples are our training dataset. The student in this case is our machine learning model and the examples are part of the dataset. Because students are learning by those examples that’s why we call it our training set.

And to check whether the students got the concepts of the algorithm correctly, the teacher give some practice problems to the students. By solving those problems students will evaluate their learning and if there is any difficulty they face, they will ask their doubt of the instructor(Feedback of model).

There might be some misunderstanding between the students for some concepts because of which they were not able to solve the problem. So, the teacher might try to explain the problem to the students in a different way(Fine-tuning of parameters).

Students can also improve their learning by solving more and more practice problems(Validation). The more diverse the practice problems are great will be the learning(Cross-validation). Students can improve their accuracy(Cross-validation accuracy) by repeatedly solving practice problems.

But once the class teaching is over and the exam comes, there is no going back to the teacher or solving practice problems. Whatever the students have learned, they need to use it for solving the problems given in the exam(Testing data). And the result that the student gets will be the final accuracy about how well that student learned about that concept.

The summary of this analogy is:

Training data = Classroom teaching

Validation data = Practice problems

Testing data = Exam questions

(Reference: [5])

---

## Question five is

- **Find one case study (research paper or article) that explains how Machine Learning has been applied in healthcare, business, or transportation. Summarize its findings.**
Answer:
this is  article that is a case study of how machine learning has been applied i healhcare also it has it's Summrized key findings.
(Reference: [6])

---

## references

1. <https://cloud.google.com/learn/what-is-machine-learning?hl=en#machine-learning-defined>
2. [<https://www.tableau.com/learn/articles/machine-learning-examples#:~:text=Facial%20recognition%20is%20one%20of,or%20sexual%20exploitation%20of%20children>.](https://www.tableau.com/learn/articles/machine-learning-examples#:~:text=Facial%20recognition%20is%20one%20of,or%20sexual%20exploitation%20of%20children)
3. <https://developers.google.com/machine-learning/crash-course/overfitting/overfitting>
4. <https://aws.amazon.com/what-is/overfitting/#:~:text=Overfitting%20is%20an%20undesirable%20machine,%E2%80%A2>
5. <https://www.linkedin.com/pulse/why-do-we-need-data-splitting-utkarsh-sharma/>
6. <https://pmc.ncbi.nlm.nih.gov/articles/PMC10258084/#Sec1>
