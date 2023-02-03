# Directory-Monitor-APP



This is directory monitor application. It monitors a directory (passed in the programme argument) and reads both existing and newly added files in that directory and prints out statistics such as number of dots, total number of words and the count of most used word to the console.

****
The application is made up of four packages: the directory monitor, services, fileProcessor and fileStatistics.


**directoryMonitor package:** contains the class that is the heart of the application, the monitorDirectory class. It takes a directory path and monitors the directory for create events. It calls the methods that read files, processes statistics, creates a folder for processed files, and moves processed files to the processed folder all within that directory. 


**services package:** contains all the interfaces in the program. 


**fileProcessor package:** contains the class that takes care of reading content from files.


**statistic package:** contains the classes the process different types of statistics from the file content. The statistics implemented include: word count, number of dots and most used word.

****
The application was developed with java 11. The only dependencies added are those necessary for testing: JUnit, Mockito.
****
The application can be run through the main method. Once you run the main method, the application starts. However, you have to provide a directory path located in your local machine in the 
programme argument of the Run configuration environment.

Alternatively, you can comment out the first "if condition" in the main method (in the Main Class) that checks if a path was passed in the programme argument
and the assign a valid path to a directory in your local machine to the variable **"passedDirectoryPath"** then run the main method to use the programme.



