# Dev-Diary
## This diary contains a daily log of what I have learned while developing programs. 

#### The date format for this log is MM-DD-YYYY

<br>__07/02/2021__<br>
I fixed one of the two failing tests and then got a whitelabel error when adding jobs. It was like one step forward and two steps back. I adjusted my code and went through trying to figure out why things were not passing correctly. I ended up realizing the redirect was "redirect:../" and it needed to be "redirect:./" one little period too much. Figures. Next I moved on to passing the final test of TestTaskFour which was the MySQL test. I had already written a query but it was not working. I went through with a fine fine tooth comb and changed the SELECT to be * (all) instead of naming the columns. I also changed the WHERE to specify the table.column I wanted rather than just passing in the column name. Those two tweaks allowed me to pull all of the columns from the skills table that had been assigned jobs.

I used the terminal to commit my final graded assignment for Unit 2 of my LC101 Web Developer Bootcamp and got the coveted green check mark! Very exciting news. I have the last week of material to read and a studio to do. I feel confident that I will done with that within a few days. I am feeling very accomplished. This bootcamp journey has been humbling. I learned a lot while I was going the self-taught route (prior to the bootcamp), and in so many ways I was self-taught during the bootcamp but the bootcamp challenged me to stretch much more. I am so grateful for LaunchCode and their LC101 Bootcamp. Today was not without it's struggles. Today I was victorious!

<br>__07/01/2021__<br>
TestTaskThree is passed and in the books. The fix for that test ended up being the need to add on a name to the JoinColumn annotation I was close, but added it without quotations and for some reason it didn't occur to me I might need them. I reached out to my peers after spending much time trying to figure out what the issue was with my code. One kind soul eluded to me needing what I had, or a version with quotation marks. Since I already had the first version, I added the quotes which looks like:
```Java 
@JoinColumn(name="employer_id")
``` 
TestTaskFour has two failing tests. I know yesterday I thought I only had one left to pass but some tests were sneakily commented out by LaunchCode and needed to be commented in. Still progress! The project renders as expected and the user is able to add jobs, skills, and employers. The issue I have now is that I am supposed to invoke employerId.get() but it is coming up null and I'm not sure where to fix that. I've tried changing various fields in the Employer and Job classes as well as the HomeController to no avail. It'll probably be something super simple. Needless to say my brain is getting a nice work out today. 

<br>__06/30/2021__<br>
Today I spent some time learning about one-to-one and many-to-many relationships. I also learned about cascade with a one-to-one allows us to specify which ORM or database operations will flow from a class to its model. cascade = CascadeType.all makes sure that all databases will be passed. Additionally, I worked on Graded Assignment 4. I was able to fix the code so that it renders. Right now the form works with exception to adding a skill which gives me a Whitelabel Error Page, same with adding a job. I need to look a little more at those and see where I've gone wrong. I will take the page loading a sign I am on the right track. Just one test to pass for TestTaskThree and one for TestTaskFour then I will be done with all of the graded assignments for LC101. This assignment isn't due until July 19 but I like to stay ahead of the game and surpass deadlines when I am able.

<br>__06/29/2021__<br>
I have been working more on Unit 2 Graded Assignment 4 again today. I made it through most of part 3 but somehow I am not passing the data in properly. I keep getting an error saying "MappingException: Could not determine type for: java.util.List, at table: job, for columns: [org.hibernate.mapping.Column(skills)]" I have been trying to figure out where I need to change the code. I know I am close, but I am little stuck. So I'm going to sleep on it. 

<br>__06/28/2021__<br>
I officially became one of the Evangelists for the St. Louis chapter of Women Who Code. I will be helping to run/maintain the Twitter and LinkedIn accounts for the chapter. I am excited to volunteer with a program that has such a beautiful mission.<br>
I began working on Graded Assignment 4 and made it through the first two sections smoothly. I am understanding and enjoying Java more than ever. It is interesting working with respositories, crud, controllers, etc. This project we are also integrating MySQL into which has been fun to see it sync up. 

<br>__06/26/2021__<br>
I read about and did exercises about relationships in object-relational mapping. This included one-to-one, one-to-many, many-to-one, and many-to-many relationships. I also used Hibernate to help keep track of the relationship within the database. I love using Java, Spring and have it connected to MySQL and how seamless it can be for the user.

<br>__06/25/2021__<br>
Remember how I couldn't figure out why the links weren't showing up. I had an ah ha moment last night at my son's Jazz recital - fragments! I forgot to add links in the fragments template! So this morning I opened it up, linked appropriately and voila - it works! I also completed the Chapter 17 studio which was to create an AbstractEntity class and then extend the Event and EventCategory classes. It went a lot smoother than I expected. On the docket for today is accepting grading Assignment 4 and reading through the requirements. I still have two weeks of course work to complete, but I'd like to be referencing the assignment and completing it as I go, if possible. Wish me luck! <br><br> <h1>I officially graduate LC101 Web Developer Bootcamp on July 19</h1> I will proably be done with my course work before then, but that's the official due date of all coursework. <br>Next up? Finding a job! I am super excited to finally be realizing my dreams! __LiftOff__ which is LaunchCode's career readiness track starts August 2, I'll be participating in that while I apply to and interview for jobs. <h3>Hire Me!</h3>

<br>__06/24/2021__<br>
Almost completed Chapter 17 exercises. I was able to get the All categories and Create categories to render but the links to get there aren't rendering yet. I looked around quite a bit and have not figured out how to get them to show up. I will have a go at it again tomorrow. Feels good to almost have the exercises complete.

<br>__06/23/2021__<br>
Borrowing a laptop yesterday through tomorrow and it's throwing me off of my game. I can't install all of the necessary programs (IntelliJ, MySQL, Java, etc.) Yesterday I did not do much coding but worked on plans to be more ready for applying for jobs (portfolio, blog, github, linkedin, etc.) Today I've been reading Eloquent JavaScript, capturing screenshots of various projects to add to my portfolio site, looking over GitHub. I do need to clean things up a bit around here, and polish it so that I can put my best foot forward when interviewing. I plan to update my readme files in my repositories to better explain the projects, mention technologies and techniques implemented as well. I also want to add screenshots to my github readmes so it is easy for potential employers to see what the project looks like before it is deployed. I'm missing my bootcamp curriculum work but I'll be ready to throw myself back into first chance I get. Funny, Java has grown on me! Greatest feeling!

<br>__06/21/2021__<br>
This morning I finished the studio I started on Saturday. The last problem of the studio definitely made me think. I ended up mapping out what I needed to pull on a piece of paper. Something about writing things down helps me to tease out the details. I needed to print the first and last name of the patron as well as the genre of the book for each book that was checked out. Easier said than done. I needed to pull information from 4 different tables in order to achieve this. I started by first using select statements to pull the information separately. Then once I had that information I looked at how I could join the tables in order for the data to flow the way that was anticipated. Here is what I came up with:
```MySQL
SELECT patron.first_name, patron.last_name, genre.genres
FROM patron JOIN loan
ON patron.loan_id = loan.loan_id
JOIN book ON book.book_id = loan.book_id
JOIN genre ON genre.genre_id = book.genre_id
WHERE book.available = 0;
```
As you can see, first I grabbed the name columns from the patron table, and also the genres column from the genre table. Next I needed to join the patron and loan tables so I did that by joining their loan_ids. Then I joined the book and loan tables at the book_id. Then I joined genre and book tables at genre_id. Finally, I specified that I only wanted books that were checked out so I needed any 0 values within the available column within the book table. Available is a bool so 1 represents true, meaning it is available and 0 represents false, meaning it is checked out or otherwise unavailable.

<br>__06/19/2021__<br>
My peer walked myself and a few other study buddies thru how to do MySQL through the command line. I like that you can print the tables and go back to reference them in the command line. When I use the gui the tables show until I run something else. But the gui is nice for a beginner to think through the process. I went back and forth between the command line and gui for the studio I was working on and I'm starting to find my groove.

<br>__06/18/2021__<br>
I talked with a peer this morning about MySQL. She has experience with SQL and explained that I can use one new query to write all of my queries in and once they are run I don't need to save them. She is also going to show me how to run MySQL through the command line instead of the GUI. Apparently some DBA people like the GUI and some like using the command line. I am open to either. Our course has us do it in the GUI but I think the simplicity of the command line appeals to me. We will meet tomorrow at 10am to go over how to accomplish that. I wonder which camp I will be in? Lucky to have her around to show me the ropes. Today went smoother. I read ahead into the next week material and it explained a lof of the things that I was confused about for this week's exercise and studio. 

<br>__06/17/2021__<br>
I'm a bit confused on whether to use new queries for each new query. I also am not sure if I need to save everything I run in MySQL. I am working my way through the Studio for this week. I feel like it's a little stop and go. 
<br>In other news - I am joining the Leadership team for my local Women Who Code chapter. I am going to be a Network Evangilist. I am super excited to volunteer with Women Who Code St. Louis. I am super passionate about women in the tech field. I am looking forward to helping our chapter grow and be a place of robust support to all who engage with it. I will meet with one of the Directors, Nicki on Monday to find out more about my duties in this role.

<br>__06/16/2021__<br>
Introduction to SQL more specifically MySQL Workbench today. I learned about different types of joining, creating, reading, updating, and deleting tables. I had had a small experience with SQL previous to this so it wasn't too foreign. It was a nice change of pace to think about database. I am looking forward to joining database technology with framework. I am getting excited to join all of this together into a project.

<br>__06/15/2021__<br>
Model validation and enums were the topics for today's studies. I learned that model validation rules (this is where annotations come in handy), while controller checks validation rules when the data is submitted to the server then takes appropriate action when validation fails.  

<br>__06/14/2021__<br>
Today I am working through models, model-binding, and model validation. I did the exercise to add an edit feature to an event list where users could create an event, see all created events, and now edit individual events if the details changed. I'm also working on creating a sign-in feature on the spa-day app at the user-signup-starter-branch. It is not quite rendering yet, but it's on it's way. I'm feeling excited to learn how to validate the information within Java/Spring.

<br>__06/11/2021__<br>
I spent some time practicing JavaScript, hosting some of my previous projects on github.io and also reading about models in Spring. Also was able to help two classmates at separates points in the day to debug their Assignment #3. It felt good to be able to pinpoint some issues to help them get past their blocks. 

<br>__06/10/2021__<br>
Today I feel like I am breaking through some barriers! I was able to complete the rest of graded Assignment #3 and pass all of the autograder tests. Woohoo!! I was struggling with an issue last night where I could not get the data I wanted to pass into one column to show up there. Instead, it was replacing data in the column next to it. Frustrating. I tried moving things around, calling it in other places, etc. No luck. So this morning I tinkered with it a bit more, then asked for suggestions from my peers. One peer asked me if I had removed or commented out a <td></td> since I had opted to use the first of two choices for accomplishing the task and the second choice would have used the td. I commented that out. Voila everything loaded where it needed to. Such a simple fix. I am very grateful to peers for helping me when they are able. The rest of the assignment today went smoothly. That isn't to say that I didn't have a challenge but I finally feel like I am able to navigate through packages, controllers, etc. I got the green check on GitHub classroom and I feel like I am on cloud 9. I needed this win this week.

<br>__06/09/2021__<br>
I had to psych myself up today before starting my coursework after the struggle on the 7th. Somedays just hit me harder. Finally convinced myself I can do this! And guess what? I figured out how to call the information from the form to make it appear on the screen. What I was missing was the model.addAttribute("name", name);, etc. for the different form items and that made all of the difference.

<br>__06/08/2021__<br>
Today I worked on my portfolio website. I have to figure out how to deploy some of my projects (particularly those made with Python). I also need to decide if I want to use screenshots, gifs, or some other means as a thumbnail to link to the projects. Additionally I learned that you can beautify your GitHub profile! See this article to learn more! [https://docs.github.com/en/github/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme](url) I spent part of the day working on beautifying my GitHub profile. I added images for each of the languages, databases, frameworks, IDE's, etc. I've worked with. I also added my social media links as well as some GitHub stats widgets. It's looking a lot more fun than it did yesterday! I spent some time with Eloquent JavaScript as well. I needed a break from bootcamp material for the day, but am looking forward to tackling again it tomorrow!

<br>__06/07/2021__<br>
Learned more about Thymeleaf and adding Bootstrap today. I finished up Chapter 11 reading and my was able to get my code to work with the walk through even though I hit some hiccups. I also created an issue with one of my github repos by merging when I should not have. Happy to say I successfully fixed the issue with a little Googling and a lot of deep breathing! <br>This current curriculum of Spring, Thymeleaf, Bootstrap is a little overwhelming for me today. I think it is so cool what we can accomplish and I so want it to to work! But I am feeling lost with all of these different files to work between. It's hard to know how to call everything so it appears on the screen. I have had some experience with Bootstrap a long time ago. But where I seem to be struggling is within the Spring/Thymeleaf part. I struggle to know what to put in the controller file versus the html template files and calling the fragments from the fragments.html. I feel like I hardly made headway today on my exercises. It doesn't help that the instructions are outdated and vague. Imposter syndrome is hitting me hard this afternoon. I am so commited to becoming a developer, and fear of failure gets amplified in times like these. I will not give up. Just trying to be real. Off to do a power pose, stretch and hydrate! This too will pass. 

<br>__06/04/2021__<br>
My theory proved true: some time off did help! First thing this morning I got to work on the form with the drop downs and got it to work within the hour. I had one action labeled incorrectly. I was able to fix that, and also clean up the code and it worked great thereafter. The remainder of the day I spent coding another form with drop down menus titled skills-tracker (see associated repo). It was a little more intensive than the first, but I was successful after that initial struggle. 
<br>__CHALLENGES = GROWTH OPPORTUNITIES!__<br> 
I read the chapter on Thymeleaf and followed along with the video walk thru where I learned about Thymeleaf use with Spring, creating templates in Intellij, populating data into Thymeleaf templates, th uses for looping and if statements, etc. Big learning day! I was pleased to see that it is very similiar to how template literals work in both JavaScript and Python. I am also pleased to note that my confidence is growing in Java and Spring MVC. Very welcome feeling.

<br>__06/03/2021__<br>
I worked on Controllers in Spring. I made different requests to the local host. I used @GetMapping, @RequestMapping, @ Conroller, @ResponseBody, etc. I also learned to make a form with drop downs. I struggled to get the drop down form data to load and kept getting an error. I had been working all day on learning the material so after consulting some peers, researching via Google (my friend), and scouring my code for what could be wrong. I finally decided to stop for the day so that I could approach the problem with fresh eyes. Frustrating to end without a resolution. Coding is addicting and it's hard to stop before the puzzle is solved! I have found though that a little time away works wonders.

<br>__06/02/2021__<br> 
Not going to lie...I made a mistake last night while working on Assignment 2 that ate some of my time up. I was supposed to create an abstract class to put the object classes' shared data in and then use the object classes to extend the abstract class. Sounds easy right? I confidently added the JobField class, made it abstract and began moving shared code into it. Then I extended the other classes. Only it didn't run. I could not figure out why the classes couldn't extend the abstract. Was I forgetting an import? No. Was I typing it in wrong? No. What was the issue? Frustrated I logged off for the night. This morning, I log back in and I see that I accidentally made the abstract class in a different package than the class objects!! Oh man. I couldn't believe it and I still don't know how that even happened. But alas, I moved the abstract class to the correct package and like that it ran and all of the autograder tests passed! Lesson learned? Always check the class location is in the correct place! 

<br>__06/01/2021__<br> 
Missed a few days of logging but I did code on 5/27, 5/28 and 5/31. I have been working on graded Assignment #2 for Unit 2 of LC101 LaunchCode Bootcamp. It's titled "Tech Jobs Object-Oriented Edition". I also feel like Java has not come as naturally to me as JavaScript and Python so I have been spending a lot of extra time re-reading, studying material to make sure I am understanding the process to apply to my assignment. Today I am working on TDD (Test Driven Development) my tests are to test if the field is empty, if the string contains correct labels for each field, that each field starts and ends with a blank space, that the equals method works, etc. I write the test then fix the code in my program to run accordingly. It is tedious at times, but helps catch any holes. I am less intimidated by TDD than I was when I first learned it in Unit 1 so that is a welcome thing.

<br>__05/26/2021__<br>
I wanted to get another perspective on inheritance and polymorphism so I read and completed the exercises in my Head First Java book. Did a lot of tree mapping. Something to remember __Lowest on the inheritance tree WINS!__

<br>__05/25/2021__<br>
Polymorphisms today. Spent some time on an exercise that utilized two Comparator classes. This exercise simulated an ice cream shop and the Comparator classes helped to sort the flavors and cones arrayLists. I got stuck when it came to printing the sorted data to the console. I did a lot of Googling, reading documentation and examples. <br>I found this website with an example that looked like it would work with my Main class:<br> [https://www.geeksforgeeks.org/comparator-interface-java/ ](url)<br>
Here is what I came up with for printing the sorted flavors (sorted by their name per the FlavorComparator class): 
```java
flavors.sort(new FlavorComparator());
System.out.println("\nFlavors");
for (int i = 0; i < flavors.size(); i++)
    System.out.println(flavors.get(i));
 ```

<br>__05/24/2021__<br>
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

<br>__05/21/2021__<br>
Hands on with Java Unit Testing (Junit) in Intellij. Made unit tests to test if the code outputs balanced square brackets or not. I used the TDD method I learned last unit while testing with JavaScript, and made tests then built my code to make it pass. So far this testing seemed a lot easier than the JavaScript testing, but I am just learning the basics. I chose to mostly use AssertTrue and AssertFalse for these tests as they seemed like a good fit of judging if the square brackets were there and matching pairs, or not.

<br>__05/20/2021__<br>
Completed restaurant menu studio that had been challenging me. I made methods to print the menu, print individual menu items, add menu items, remove menu items. Manipulating Arraylist and using methods to call objects from the Arraylist does not come naturally to me, so I have to reference notes and Google. But I am slowly making headway in my understanding and ability.

<br>__05/19/2021__<br>
Read the chapter and took notes about Unit testing with Java JUnit. Practiced writing tests using @Test, @Before, @After and Assertion Methods. 

<br>__05/18/2021__<br>
Review day - spent some time watching some videos about Java topics and making sure I understand before moving forward. Here are a few of my notes:
- The power of back slash to print double quotations, tab, new line, etc. \"\"\\ Will allow double quotations to print
- Difference between float and double types. They are similiar in that they return a number with a decimal value. The exception is that float has a maxmimum length, whereas double can take an unlimited amount of digits.
- Nested loops are great for iterating through 2D Arrays.
- Difference between ArrayList and HashMap. ArrayList is ordered and items can be accessed through the index. HashMap is unordered and can be accessed through the keys and values.
- Within Classes variables are things it KNOWS, methods are things it DOES.
- Methods do one specific task.


<br>__05/17/2021__<br>
Worked on creating a Restaurant package in Java with two classes of Menu and MenuItem. Found a diagram website to help me visualize how I might construct the classes. [https://app.diagrams.net/](url)


<br>__05/14/2021__<br> 
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


<br>__05/13/2021__ <br>
Learned how to declare variables so that setters and getters can work to properly be able to instantiate the class. Instantiated a student in the Student class with my name, the number of credits and GPA.


<br>__05/12/2021__ <br>
Spent today learning about Java Arraylists that store HashMap objects which have a String of keys and a String of values. I am not quite printing the correct thing to the console yet. 


<br>__05/11/2021__<br> 
This is my very first entry to the Dev-Diary.
