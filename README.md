# spamClassfiers
Using different spam classifiers to filter spam emails

Requires the download of Apache Spark, as well as Python 3 and have JDK/JVM installed on deviced before running the notebook.

For Apache Spark: https://spark.apache.org/downloads.html. Follow the instructions and choose the lastest version plus the according package type.
Could also try !pip install pyspark for simplicity. Set up the path for the files accordingling.

Note that 
import findspark
findspark.init()
findspark.find()

Is requires to run on Jupyter lab notebook for some devices. If not needed, then do not have to import and use this library.

There are 3 input files:
spam.csv -> Original dataset
spamx2.csv  -> dataset with twice the size
spamx4.csv -> dataset with 4 times the size

To test out different input files, just alter the code in block [4]: email = sc.read.csv("spam.csv", header=True, sep=",") to the wanted file. The x4 dataset would take a few minutes for SVC to train.
