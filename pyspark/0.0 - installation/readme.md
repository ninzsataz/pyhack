
# Installing pyspark to run in jupyter notebook

---

### Step 1: Install pyspark and findspark

In your virtual environment:

    $ conda install pyspark
    $ conda install -c conda-forge findspark

### Step 2: Create a new folder to store all installation dependencies
 From the command line:

    $ mkdir server

### Step 3: Download dependencies (Spark) into your new folder

Download and extract the following zip/tar files to the ```server``` directory that you just created:

- [spark-2.4.3-bin-hadoop2.7.tgz](https://spark.apache.org/downloads.html)


### Step 4: Confirm installation

1. Run ```java -version``` from the command line. You should see something like this: 

        $ java -version
        java version "1.8.0_211"
        Java(TM) SE Runtime Environment (build 1.8.0_211-b12)
        Java HotSpot(TM) 64-Bit Server VM (build 25.211-b12, mixed mode)

2. Test pyspark by running it in the interactive shell. Run ```pyspark``` from the command line you should see something like this:

        Using Spark's default log4j profile: org/apache/spark/log4j-defaults.properties
        Setting default log level to "WARN".
        To adjust logging level use sc.setLogLevel(newLevel). For SparkR, use setLogLevel(newLevel).
        Welcome to
              ____              __
             / __/__  ___ _____/ /__
            _\ \/ _ \/ _ `/ __/  '_/
           /__ / .__/\_,_/_/ /_/\_\   version 2.4.3
              /_/
        
        Using Python version 3.5.1 (v3.5.1:37a07cee5969, Dec  5 2015 21:12:44)
        SparkSession available as 'spark'.

    Hit CTRL-D or type exit() to get out of the pyspark shell.


3. Run the notebook: ```0.1_basic-commands.ipynb``` and successfully execute each cell


## If you made it this far without any problems, you have successfully run pyspark in jupyter notebook  :-)