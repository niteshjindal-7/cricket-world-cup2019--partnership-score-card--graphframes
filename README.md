# cricket-world-cup2019-[partnership-score-card--graphframes]

**Please download below set up files which might help you in importing and using the packages used in the notebook:-**
#######################################################################################################################

<> **Refer below link to install PySpark:-**

https://changhsinlee.com/install-pyspark-windows-jupyter/

<> **Refer below steps to install latest version of graphframe module after PySpark installion:-**

1. Check the spark version installed by using below command in command prompt-

`spark-submit --version`

2. Check the version of graphframe from below link which is suitable for installed Spark version and install it-

https://spark-packages.org/package/graphframes/graphframes


3. Copy the `jar file` to the location where python is installed in Spark(python folder in the installed spark) 

4. Copy the `jar file` to spark location as a zip file. refer below sample command, which can be run in window power shell-

`cp 'C:\\Users\\XXXXX\\AppData\\Local\\Programs\\Spark\\spark-3.1.2-bin-hadoop2.7\\jars\\graphframes*.jar' 'C:\\Users\\XXXXX\\AppData\\Local\\Programs\\Spark\\spark-3.1.2-bin-hadoop2.7\\python\\graphframes.zip'`

5. Unzip it and cut items present in the same subfolder folder and paste them in outer folder name graphframe folder.

6. Add the new path in the `environmental variables`. For an example, add below path if you have installed files in graphframes directory-

C:\Users\XXXXX\AppData\Local\Programs\Spark\spark-3.1.2-bin-hadoop2.7\python\graphframes\

7. Return to jupyter notebook and refresh it.Then, run -

`from graphframe import *`


<> **JAVA INSTALLATION DETAILS:-**

C:\Windows\system32>java -version

java version "1.8.0_301"

Java(TM) SE Runtime Environment (build 1.8.0_301-b09)

Java HotSpot(TM) 64-Bit Server VM (build 25.301-b09, mixed mode)

<> **Spark Version:-** 
spark-3.1.2-bin-hadoop2.7 
It can be download through below link-

https://mirrors.estointernet.in/apache/spark/spark-3.1.2/spark-3.1.2-bin-hadoop2.7.tgz


**graphframe jar file path:**

C:\\Users\\...\\Programs\\Spark\\spark-3.1.2-bin-hadoop2.7\\graphframes.zip

graphframes-0.8.1-spark3.0-s_2.12


**Load the scrapped 'matches data', Data Preprocessing and extract the required information. 
In the notebook, we have followed below steps in detail for the use case - Identify Strong & Weak Partnership of a player using Graph Analytics:-**

1. Data Preprocessing Phase[Matches_data.csv]

2. Generate Partnership Score data. Treat partnership scores as edges in graph analysis

3. Generate Batsmen Score data from preprocessed data of matches. We will treat Batsman total score as vertices in graph

4. Use Graph Frame to get the close and far association between players in terms of partnership scores. It will help determining the strong and weak partnership of a player.

5. Analysis on the team where batting partnerships could not stand longer.




**References:-**

'How to install and invoke pyspark in windows environment -'

https://changhsinlee.com/install-pyspark-windows-jupyter/

https://www.apache.org/dyn/closer.lua/spark/spark-3.1.2/spark-3.1.2-bin-hadoop3.2.tgz

https://graphframes.github.io/graphframes/docs/_site/user-guide.html

https://spark.apache.org/docs/1.6.1/sql-programming-guide.html

