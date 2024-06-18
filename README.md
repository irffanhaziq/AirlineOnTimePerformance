# Data Mangenment Assignment 2

Air travel has become an imporatant part of transportation services, enabling people to connect across various distances for business, leisure, and personal reasons. However, the reliability and punctuality of flights are crucial factors that can significantly impact the passenger experience and the overall efficiency of the aviation industry. Delays and cancellations can lead to frustration, missed connections, and substantial financial costs for both airlines and travelers.


The pre-procese data can be access here : https://tinyurl.com/y8e4b8yk

```
from pyspark.sql import SparkSession
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
from sklearn.model_selection import GridSearchCV

# Create a SparkSession
spark = SparkSession.builder.getOrCreate()

# Load the iris dataset
iris = spark.read.csv("/user/maria_dev/irffan/Iris.csv", inferSchema=True, header=True)
iris.show()
```
