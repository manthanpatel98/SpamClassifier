
# **SpamClassifier**
## **Predicting Whether a Message is Spam or not.**
---
### Web APP on Heroku

![Predicting Restaurant Review Heroku Project](https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Spam.gif)

### **[The Project on Heroku](https://spamclassifiersms.herokuapp.com/)**
---
## **Understanding The Project**

### **The Dataset**
***
#### **Initial Dataset**
![Dataset](https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Screenshot%20(100).png)
#### **Converted into Structured Dataset**
![Dataset](https://github.com/manthanpatel98/SpamClassifier/blob/master/README-Resources/Screenshot%20(101).png)
* Here, initially in our data Message and its final output is separated by Tab space so i have separated them by Tab and created 2 columns. Hence, 
* Later After cleaning the columns, I converted **"Rating"** Column, which is actually a numerical column, into the column that has two labels **"Positive"** and **"Negative"**.
* I considered Rating **Above 3** as **"Positive"** and **Below 3** as **"Negative"**.
* To understand detailed Project approach, check my [**Restaurant-Review.ipynb**](https://github.com/manthanpatel98/Restaurant-Review-Sentiment-Analysis/blob/master/Restaurant-Review.ipynb) or [**model.py**](https://github.com/manthanpatel98/Restaurant-Review-Sentiment-Analysis/blob/master/model.py)
* This project has around **10,000** Reviews, so for CountVectorizer, **max_features=9000** gave best results after trying values like 2500, 5000, 7500... Which I think is most important thing to achive higher accuracy value. 
***
### **Applied Algorithms & Their Accuracy**
***
| Algorithm | Accuracy |
| ---    | ---    |
| Random Forest | 89.28% |
| MultinomialNB | 90.84% |
| SVM | 76.68% |

* After Checking Accuracy for these Three Algorithms, I decided to use **MultinomialNB** in **Web App**.
