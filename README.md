# Dev-Diary
## This diary contains a daily log of what I have learned while coding. 

#### The date format for this log is MM-DD-YYYY

__5/18/2021__
Review day - spent some time watching some videos about Java topics and making sure I understand before moving forward. Here are a few of my notes:
- The power of back slash to print double quotations, tab, new line, etc. \"\"\\ Will allow double quotations to print
- Difference between float and double types. They are similiar in that they return a number with a decimal value. The exception is that float has a maxmimum length, whereas double can take an unlimited amount of digits.
- Nested loops are great for iterating through 2D Arrays.
- Difference between ArrayList and HashMap. ArrayList is ordered and items can be accessed through the index. HashMap is unordered and can be accessed through the keys and values.
- Within Classes variables are things it KNOWS, methods are things it DOES.
- Methods do one specific task.


__05/17/2021__ 
Worked on creating a Restaurant package in Java with two classes of Menu and MenuItem. Found a diagram website to help me visualize how I might construct the classes. https://app.diagrams.net/


__05/14/2021__ 
Successfully looped through the ArrayList and the HashMap objects to be able to print the data from the CSV. Here is my code: 
```java    
   private static void printJobs(ArrayList<HashMap<String, String>> someJobs) {
        // Check if any jobs are in somejobs
        if (someJobs.size() > 0) {
            //Using a loop to iterate over Array of HashMap Objects (Jobs)
            for (HashMap<String, String> aJob : someJobs) {
                System.out.println("\n*****");
                // Then nest a for-each loop to iterate over the Hashmap Objects
                for(Map.Entry<String, String> data: aJob.entrySet()) {
                    System.out.println(data.getKey() + ": " + data.getValue());
                }
                System.out.println("*****");
            }
        }
        // Else if no jobs print "No Results"
        else {
            // Use print instead of println so an extra line is not created below the print
            System.out.print("No Results");
        }
    }
```


__05/13/2021__ 
Learned how to declare variables so that setters and getters can work to properly be able to instantiate the class. Instantiated a student in the Student class with my name, the number of credits and GPA.


__05/12/2021__ 
Spent today learning about Java Arraylists that store HashMap objects which have a String of keys and a String of values. I am not quite printing the correct thing to the console yet. 


__05/11/2021__ 
This is my very first entry to the Dev-Diary.
