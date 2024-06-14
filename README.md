### General Overview

**Challenge:** The Saber Pro Tests are standardized exams administered in Colombia to assess the quality, knowledge level, and competencies of higher education students, which include institutions such as universities and technical colleges. These tests are part of the Colombian Government's efforts to monitor and improve the quality of higher education in the country.

The Saber Pro Tests consist of five generic components: English, Critical Reading, Citizenship Competencies, Quantitative Reasoning, and Written Communication.

Your task will be to create a classification model that accurately groups students into different performance levels:

- Low
- Medium-Low
- Medium-High
- High

### Description

The dataset contains more than 50 columns that provide detailed descriptions of each student.

These columns include:

- **Socioeconomic Information:** Describes the socioeconomic characteristics of the student, such as their socioeconomic stratum, parents' education level, socioeconomic stratum, and other related details.
- **Institution Information:** Describes the institutions from which the students come.
- **Student Information:** Describes specifics about the student, such as their age, the program they are studying, the mode of study, etc.

Additionally, the dataset includes many other data points that help in accurately classifying the performance levels.

###Solution Approach
Firstly, I conducted data exploration to identify and handle null or potentially unhelpful data. For categorical data, I replaced null values with the mode, and for numerical data, with the mean. Using graphs, I visualized the distribution of data across different labels.

I employed various machine learning models to address the challenge, including Deep Neural Networks with variations in hyperparameters, Random Forest, Logistic Regression, Linear Discriminant Analysis (LDA), Decision Tree, and Naive Bayes classifier. Each model was evaluated based on accuracy. After the initial iteration, Deep Neural Networks demonstrated superior performance. Consequently, I focused on this model, experimenting with different hyperparameters and evaluating it further using metrics such as confusion matrix, precision, recall, and F1 score.
