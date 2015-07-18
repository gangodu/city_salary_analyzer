# city_salary_analyzer

A simeple MR job that groups splits based on city and outputs total wages for each city combined.

Working
    Compilation:
        Compile the program to get the class file and create a JAR to run on top of HDFS in Hadoop
        Preferred JAR creation - Eclipse IDE

    Execution:
        A sample input file is provided as input/input.csv
        Upload the JAR and the input file to HDFS
            [Load the JAR to either the home directory or the bin directory in HDFS]
        At the terminal, run the following
            {
                hadoop -jar [jar name] input/input.csv output/output.csv
            }
        An output directory is automatically created
        When the job is completed, the output directory will have output.csv

    Analysis:
        Based on the need, you may use a program like Microsoft Excel to do analysis.
    
Future:
    Other Hadoop ecosystems will be added for analysis and the program itself will be more generic and abstract such that any input can create any output efficiently on any given data set.