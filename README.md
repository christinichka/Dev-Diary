# Dev-Diary
## This diary contains a daily log of what I have learned while coding. 

#### The date format for this log is MM-DD-YYYY

05/14/2021 - Successfully looped through the ArrayList and the HashMap objects to be able to print the data from the CSV. Here is my code: 
```    
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
            // Use print instead of println so that a new line is not printed after No Results to match the test output
            System.out.print("No Results");
        }
    }
```

05/13/2021 - Learned how to declare variables so that setters and getters can work to properly be able to instantiate the class. Instantiated a student in the Student class with my name, the number of credits and GPA.

05/12/2021 - Spent today learning about Java Arraylists that store HashMap objects which have a String of keys and a String of values. I am not quite printing the correct thing to the console yet. 

05/11/2021 - This is my very first entry to the Dev-Diary.
