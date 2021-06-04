# Dev-Diary
## This diary contains a daily log of what I have learned while coding. 

#### The date format for this log is MM-DD-YYYY

__06/04/2021__
My theory proved true: some time off did help! First thing this morning I got to work on the form with the drop downs and got it to work within the hour. I had one action labeled incorrectly. I was able to fix that, and also clean up the code and it worked great thereafter. The remainder of the day I spent coding another form with drop down menus titled skills-tracker (see associated repo). It was a little more intensive than the first, but I was successful after that initial struggle. __CHALLENGES = GROWTH OPPORTUNITIES!__ I read the chapter on Thymeleaf and followed along with the video walk thru where I learned about Thymeleaf use with Spring, creating templates in Intellij, populating data into Thymeleaf templates, th uses for looping and if statements, etc. Big learning day! I was pleased to see that it is very similiar to how template literals work in both JavaScript and Python. I am also pleased to note that my confidence is growing in Java and Spring MVC. Very welcome feeling.

__06/03/2021__
I worked on Controllers in Spring. I made different requests to the local host. I used @GetMapping, @RequestMapping, @ Conroller, @ResponseBody, etc. I also learned to make a form with drop downs. I struggled to get the drop down form data to load and kept getting an error. I had been working all day on learning the material so after consulting some peers, researching via Google (my friend), and scouring my code for what could be wrong. I finally decided to stop for the day so that I could approach the problem with fresh eyes. Frustrating to end without a resolution. Coding is addicting and it's hard to stop before the puzzle is solved! I have found though that a little time away works wonders.

__06/02/2021__ Not going to lie...I made a mistake last night while working on Assignment 2 that ate some of my time up. I was supposed to create an abstract class to put the object classes' shared data in and then use the object classes to extend the abstract class. Sounds easy right? I confidently added the JobField class, made it abstract and began moving shared code into it. Then I extended the other classes. Only it didn't run. I could not figure out why the classes couldn't extend the abstract. Was I forgetting an import? No. Was I typing it in wrong? No. What was the issue? Frustrated I logged off for the night. This morning, I log back in and I see that I accidentally made the abstract class in a different package than the class objects!! Oh man. I couldn't believe it and I still don't know how that even happened. But alas, I moved the abstract class to the correct package and like that it ran and all of the autograder tests passed! Lesson learned? Always check the class location is in the correct place! 

__06/01/2021__ 
Missed a few days of logging but I did code on 5/27, 5/28 and 5/31. I have been working on graded Assignment #2 for Unit 2 of LC101 LaunchCode Bootcamp. It's titled "Tech Jobs Object-Oriented Edition". I also feel like Java has not come as naturally to me as JavaScript and Python so I have been spending a lot of extra time re-reading, studying material to make sure I am understanding the process to apply to my assignment. Today I am working on TDD (Test Driven Development) my tests are to test if the field is empty, if the string contains correct labels for each field, that each field starts and ends with a blank space, that the equals method works, etc. I write the test then fix the code in my program to run accordingly. It is tedious at times, but helps catch any holes. I am less intimidated by TDD than I was when I first learned it in Unit 1 so that is a welcome thing.

__05/26/2021__
I wanted to get another perspective on inheritance and polymorphism so I read and completed the exercises in my Head First Java book. Did a lot of tree mapping. Something to remember __Lowest on the inheritance tree WINS!__

__05/25/2021__
Polymorphisms today. Spent some time on an exercise that utilized two Comparator classes. This exercise simulated an ice cream shop and the Comparator classes helped to sort the flavors and cones arrayLists. I got stuck when it came to printing the sorted data to the console. I did a lot of Googling, reading documentation and examples. <br>I found this website with an example that looked like it would work with my Main class:<br> [https://www.geeksforgeeks.org/comparator-interface-java/ ](url)<br>
Here is what I came up with for printing the sorted flavors (sorted by their name per the FlavorComparator class): 
```java
flavors.sort(new FlavorComparator());
System.out.println("\nFlavors");
for (int i = 0; i < flavors.size(); i++)
    System.out.println(flavors.get(i));
 ```

__05/24/2021__
I have not been able to smoothly figure out how to add a new Java project from IntelliJ to an existing GitHub Repository so today was the day I thought I'd take time to work through it. I initially struggled. I kept getting an error that said "error: failed to push some refs to 'GITHUB URL'." Basically my repo only had a ReadMe file and my local file had the project files including the package and classes. Since the two had unrelated files it was not liking me wanting to push to that repo. These are the steps I took to rememdy the issue (thanks to Stack Overflow and my ability to combine multiple answers):

**********
1. git init -b main to initialize an empty Git repository in the local project on my computer
2. git remote add origin GITHUB REPO URL
3. git pull origin main --allow-unrelated-histories to allow for the local files to be added to the repo despite unrelated files.
4. git push --set-upstream origin main
5. git add . to add all of the files since none of them had previously been commited
6. git status to check that the files were added into the staging area
7. git commit -m "Commit message" to git ready to push to the repo
8. git push  
**********

__05/21/2021__
Hands on with Java Unit Testing (Junit) in Intellij. Made unit tests to test if the code outputs balanced square brackets or not. I used the TDD method I learned last unit while testing with JavaScript, and made tests then built my code to make it pass. So far this testing seemed a lot easier than the JavaScript testing, but I am just learning the basics. I chose to mostly use AssertTrue and AssertFalse for these tests as they seemed like a good fit of judging if the square brackets were there and matching pairs, or not.

__05/20/2021__
Completed restaurant menu studio that had been challenging me. I made methods to print the menu, print individual menu items, add menu items, remove menu items. Manipulating Arraylist and using methods to call objects from the Arraylist does not come naturally to me, so I have to reference notes and Google. But I am slowly making headway in my understanding and ability.

__05/19/2021__
Read the chapter and took notes about Unit testing with Java JUnit. Practiced writing tests using @Test, @Before, @After and Assertion Methods. 

__05/18/2021__
Review day - spent some time watching some videos about Java topics and making sure I understand before moving forward. Here are a few of my notes:
- The power of back slash to print double quotations, tab, new line, etc. \"\"\\ Will allow double quotations to print
- Difference between float and double types. They are similiar in that they return a number with a decimal value. The exception is that float has a maxmimum length, whereas double can take an unlimited amount of digits.
- Nested loops are great for iterating through 2D Arrays.
- Difference between ArrayList and HashMap. ArrayList is ordered and items can be accessed through the index. HashMap is unordered and can be accessed through the keys and values.
- Within Classes variables are things it KNOWS, methods are things it DOES.
- Methods do one specific task.


__05/17/2021__ 
Worked on creating a Restaurant package in Java with two classes of Menu and MenuItem. Found a diagram website to help me visualize how I might construct the classes. [https://app.diagrams.net/](url)


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
