# city_salary_analyzer

A simple Map Reduce program that groups splits based on city and outputs total wages for each city combined.

Working:
    Compilation:
        Compile the program to get the class file and create a JAR to run on top of HDFS in Hadoop
        Preferred JAR creation - Eclipse IDE
        Extract input.zip to get input.csv

    Execution:
        A sample input file is provided from input/input.csv
        Upload the JAR and the input file to HDFS
            [Load the JAR to either the home directory or the bin directory in HDFS]
        At the terminal, run the following
            {
                hadoop -jar [jar name] input/input.csv output/output.csv
            }
        An output directory is automatically created
        When the job is completed, the output directory will have output.csv

    Analysis:
        Based on the need, a program like Microsoft Excel may be used to do analysis.
    
Future:
    Other Hadoop ecosystems will be added for analysis and the program itself will be more generic and abstract such that any input can create any output efficiently on any given data set.
    
Nice to know:
    Hadoop version      :   1.5.x [stable]
    Map Reduce version  :   2.7
    Eclipse IDE version :   Kepler
    OS Developed On     :   Mac OSX Yosemite
    OS Tested On        :   RHEL
    Cluster Config      :   
        Hadoop-
            Name Node       :   1
            Data Nodes      :   2
        Map Reduce-
            Job Trackers    :   1
            Task Trackers   :   2
        Replication Factor  :   2
        Number of Mappers   :   10
        Number of Reducers  :   2
