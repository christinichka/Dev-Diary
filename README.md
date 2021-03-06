# Dev-Diary
## This diary contains a log of what I have learned while developing programs. 

#### The date format for this log is MM-DD-YYYY

<br>__10/4/2021__<br>
I took the practice exam on 10/1/2021. I realized I know the basics really well. I got above average. However on exception handling I did poorly. My bootcamp taught a very low level of exception handling and I didn't even know what some of the error names were or what they meant. I also had not ever done switch cases though I had seen some others using them on Hackerrank. I also had very little experience with try, catch. So I've been studying these things and more. Still filling in the gaps. It was good to get the first full practice test underway so I could see where some holes were. I plan to take another in a day or two and see how things are shaping up. Just 10 days until I sit for the exam.

<br>__09/30/2021__<br>
This week I've been doing a lot of practice questions for my exam. I am going to take a full practice test tomorrow. Two weeks from today I'll be sitting for the the OCA exam. I hope that I have what it takes. I am getting nervous. 

<br>__09/27/2021__<br>
I have been dealing with an annoying issue since beginning my studies with Java 8. For my bootcamp we used Java 11 and my computer doesn't like to let me easily choose between the two Java versions. Boo. Well I finally found a solution that I think will work for me - at least in IntelliJ. The winning video comes from YouTube Channel Arjun Codes [check it out](https://www.youtube.com/watch?v=A5FHcR3cE-w). 
In summary:
1. Get the path to the bin file for the version of Java you'd like to switch to. In my case, I have Java 11 set as my default and I want to be able to use Java 8 as well so my bin is C:\Program Files\Java\jdk1.8.0_301\bin.
2. Open System Properties and then click on Environmental Variables.
3. In the bottom section titled System variables double click on "Path" once the window opens click on "New" which is located on the right hand side of the window. Paste in the bin path.
4. Now create a new project in IntelliJ and you will see at the top there is a drop down after Project SDK: in the drop down you should now see the default version as well as the one you added to the path of your System variables.

<br>__09/25/2021__<br>
We have a bug on our group project where the button on top of our carousel to take us to see the specific book was only clickable on the outer edges. I was able to fix this issue by adding style="z-index:999;" to the div with class="carousel-inner" and now the entire button area activates. This was our last Saturday meeting as a group. We present the project on Monday evening at our final LiftOff class session.

<br>__09/24/2021__<br> 
Drop down clicking problem fixed! I discovered that I needed to add 
```HTML
onclick="displayDropdownSelection()"
``` 
to the button tag and not just to the li tags with the drop down options. Now the drop down toggles when clicked on the first click as would be expected.

<br>__09/23/2021__<br>
Looked a little more into solving the drop down issue. No dice. I tried moving around scripts, adding or removing different scripts, changing our jquery function, etc. Nothing. Funny thing that this Bootstrap drop down was the unsuspecting nuisannce in this project.

<br>__09/22/2021__<br>
Today I worked on fixing the design of my group's project, adding in background to make text readable and trying to figure out why the drop drown must be clicked twice to make it drop down. I tried many different things but so far haven't been able to fix the issue. My peers are also trying to uncover the reason. 

I made a quizlet today to study Java terms and also practiced some exam prep questions. I am nervous because some of these questions are tricky. But little by little I'm feeling more comfortable with the type of questions being asked.

<br>__09/21/2021__<br> 
I learned something new today. I didn't realize if I forked my group project to my GitHub repo that it would give me an option to catch up to the most updated commits from the repo I forked. Pretty snazzy tip a group member gave me.

Met with my study group today and discussed polymorphism, interface, hibernate, and responsive web design. I taught them about responsive web design and interface. In short responsive web design means to write code one time to look amazing everywhere - in other words we're talking about scalability to all screen sizes and shapes. Bootstrap helps a lot with that. For interface it is an all abstract class. Each class can only inherit one class, however they can implement the behavior of many classes. An example I found in a book was a robot dog would be a part of the robot class, but could implement methods from the pet class to help it behave like a real dog.

<br>__09/20/2021__<br>
One more class to go for LiftOff. My group has completed the mvp and are cleaning up the project to look that way we would like it to. I plan to practice deploying it once it is complete and I have a copy saved on my own GitHub repositories (it's housed on the TA's GitHub for now). The Java exam studying has taken over and I am spending a lot of time reading and practicing concepts from the exam. 

<br>__09/16/2021__<br>
Today I figured out how to get my group project search to submit when the enter key is pressed and not just have to rely on the button. This is what was the outcome. After trying all kinds of JavaScript to help listen to the event - all I really needed was a <form> tag with method and action placed inside to wrap around the entire search area. It's the little things you get hung up on as a software engineer. 

```HTML
	<form name="searchBarWithButton" method="post" action="/search">
```
My LC101 study group has been studying different Java topics to enhance our knowledge for interviews and for on the job. I taught about REST and OOP. Another peer taught about Interitance, Abstraction, Spring Boot and a few other things. Good times. It helps to talk with others and think through about these concepts.

<br>__09/15/2021__<br>
Spent time studying for the Java exam. Also studied up on REST and the benefits and pillars of OOP to teach my study group.

<br>__09/14/2021__<br>
AFS is giving me the opportunity to become Java certified prior to my start date (October 18). I scheduled my Java SE 8 Programmer I exam #1Z0-808 today and I will be sitting for it on October 14. I have one month to prepare. I will studying using video, study guide texts as well as practice tests. I am a little intimidated, but mostly curious about the exam material and feeling up for the challenge. Today I have been going through the videos AFS provided me in the study materials. I am crafting a study plan as well. 

<br>__09/13/2021__<br>
My team met during class yesterday and we worked on figuring out what branches needed to be merged into our master branch. It was a bit of work. We also worked on getting our button to fire on enter press since right now it just works when clicked. It was a good coding session. We have two weeks left on our project. 

<br>__09/10/2021__<br>
I have had the pleasure to help some peers prepare for their technical interviews by sitting in on coding challenges. Coding challenges are nerve wracking! I have been practicing as well because even though I've accepted a position with Accenture Federal Services (YAY!!!) I chose to finish my LiftOff program which requires me doing a graded live coding challenge with the LaunchCode staff. It's nice to practice with others because it shows that we all have our strengths and weaknesses. We also all struggle with anxiety surrounding coding challenges. Something I have learned is that being a software engineer means getting comfortable with being uncomfortable. Technology is always changing and adpating can be uncomfortable at times, but when you start to see change as an opportunity rather than a threat you blossom. Here is a coding challenge I did this morning (solo):

Calculate Average Time
<br>In this problem you are given the speed a train is travelling (x), and you are given the distance the train is travelling (y), you need to calculate how long it will take for the train to arrive at it's destination.

You will need to calculate the time for three trains, and then you will need to calculate the average time of the three trains journeys'.

Example:
Train One: x = 20, y = 150

time = 7.5

Train Two: x = 25, y = 155

time = 6.2

Train Three: x = 32, y = 162

time = 5.0625

Average for all three trains: average time = 6.25416

``` Java
class Main {
  public static void main(String[] args) {
    System.out.println("Hello world!");

    // create three train arrays that will hold the value for their speed x and distance y
    double trainOne = lengthOfTime(20, 150);
    double trainTwo = lengthOfTime(25, 155);
    double trainThree = lengthOfTime(32, 162);

    System.out.println("Train One: " + trainOne);
    System.out.println("Train Two: " + trainTwo);
    System.out.println("Train Three: " + trainThree);

    // function to calculate the average of the three trains journeys
    double averageTime = (trainOne + trainTwo + trainThree)/3;

    System.out.println("Average time: " + averageTime);

  }

  // function to calculate the time for any given train based on their distance
  public static Double lengthOfTime(int x, int y) {
    Double time = (double)y / (double)x;
    return time;
  }
}
```

<br>__09/09/2021__<br>
This morning I saw my teammate cracked the code for the dropdown by switching to a select tag and instead of categories we are going to select author and title because the API was not created well for retrieving categories and gave us all kinds of headaches. It's nice to be able to be flexible but still be able to filter by title or author and then by the user text input. Sadly the JQuery code I worked hard on didn't get used. But that's part of working in a team. I learned a lot and don't regret the time I spent on figuring out the workings of JQuery. I'm looking forward to using it more in the future. I was able to work on some styling this morning and get the select to be the same height as the input and search button. It did not want to change no matter what I did to the css. I ended up finding an answer on StackOverflow that helped me to add some code into the select tag directly. ```HTML class="form-control" style=" height:35px;" id="sel1" ``` did the trick. Happy it finally looks like it is coming together. 

<br>__09/08/2021__<br>
Spent some time on hackerrank again. Worked on my dev blog. Still working on the user authentication but almost there. Spring security is new to me so I spent some time working through a tutorial. 

<br>__09/07/2021__<br>
Today I learned about printf in Java. I had not heard of it previously and had been taught to use print or println. Basically printf gives a formatting string before what to print out. [Here is a good overview video about printf](https://www.youtube.com/watch?v=moQ3Kr8ouiU) I like this concept because it allows me to format say an addition problem to be printed as I want, or a number to include the decimals or not with just a % and a letter.

<br>__09/03/02/2021__<br>
I have been working on coding algorithms today. Below is one I did on [hackerrank](https://www.hackerrank.com/challenges/java-if-else/problem) with the following parameters:
"Given an integer, , perform the following conditional actions:

If  is odd, print Weird
If  is even and in the inclusive range of  to , print Not Weird
If  is even and in the inclusive range of  to , print Weird
If  is even and greater than , print Not Weird
Complete the stub code provided in your editor to print whether or not  is weird."

```Java
public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner sc=new Scanner(System.in);      
        int n = sc.nextInt();
        if ((n%2 == 1) || (n>=6 && n<=20)) {
            System.out.println("Weird");
        } else {
            System.out.println("Not Weird");
        }

    }
}
```
My approach was to find all of the odd numbers and then see if they also were between the numbers 6 and 20 if so I printed weird. If not, printed not weird This problen reminded me of FizzBuzz.


<br>__09/01/2021__<br>
I have been practicing th:each in Thymeleaf today. I love to see how Java works hand in hand with Thymeleaf. I love to see how the model can be set up so that the user can view the data. I also have made some tables with Bootstrap. I am beginning to think Bootstrap Select might be an easier route to go than the Bootstrap dropdown with li tags for our group project so I've been playing around with both to get a feel for what works better to pull in the categories from Google Book api.  

<br>__08/30/2021__<br>
I haven't logged for a bit. I have been continually working on the group project. I am still working on the dropdown menu functionality with the API. Google Books api is a little tricky when it comes to pulling the category. Had a meeting with my team on Saturday and they are going to help me move past some blocks. While we work on getting it going, I am going to get started on the user sign in capability in Java. We will be using MySQL as our database to store the users. 

<br>__8/24/2021__<br>
Updated the readme and styled with some basic markdown for our group project on the repo. [LiftOff Group Project](https://github.com/AbbeyKNorthcutt/abbey-liftoff-group-a)

Our group is working hard. We are working on the menu dropdown, carousel, cleaning up how things work. We are hoping we will have time to add on some other features past the minimum 3 features. 

Worked on Coding Challenge for Class 5. The instructions were as follows, "Create a function that takes a number as an argument. Add up all the numbers from 1 to the number you passed to the function. For example, if the input is 4 then your function should return 10 because 1 + 2 + 3 + 4 = 10." 
Here is what I came up with:
```Javascript
function addUp(num) {
	let sumOfNum = 0;
	for (let i = 0; i <= num; i++) {
		sumOfNum += i;
	}
	return sumOfNum;
}
```
1. Declared a variable called sumOfNum to represent the total sum of all of the numbers from 1 to my given number and set it equal to 0. 
2. Created a for loop to loop through the numbers, adding them together as they loop through.
3. Return the final sum of all of the numbers.


<br>__8/23/2021__<br>
I am still working on the dropdown menu. I've hit a roadblock on getting the value of the selected dropdown. There are plenty of Javascript select and option examples, but my dropdown is coded with bootstrap and might need to use Jquery. I have some working code both in Javascript and JQuery. A peer from my group suggested saving the value in local storage and then retrieving it to compare to the value of the looped data. I'll update when I figure this challenge out.  

LiftOff session tonight. Got to meet some engagement specialists with LaunchCode and hear about what they do to help LaunchCoders find apprenticeships. Sounds like there are a lot of opportunities and gets me even more excited about this field. My group will be doing our first project review tonight with our TA and they will give us tips on how to proceed. We will also practice live coding as pairs.

<br>__8/21/2021__<br>
Met with my group this morning. We merged some branches in our GitHub and dealt with some conflicts. We also worked on getting everything including the Bootstrap to work with the Thymeleaf because it was not working previously. The menu dropdown now shows up. I cropped the landing page image to take off words that were in the bottom and set the background size to be 100% of the page so that there wasn't a weird white area at the bottom if the screen was resized. Right now our project landing page shows the dropdown, search and button as well as the header and background image. It also navigates to the search page upon search and pulls books by title. I am working on the functionality of the dropdown menu. And we will be adding a carousel of books onto the landing as well. The duties are split among team members. 

<br>__8/20/2021__<br>
Yesterday I forgot to log - but I was doing some research on the drop down selection for the dropdown menu. I also studied whiteboarding, practiced some coding algorithms. Today I tackled changing the selected value from the dropdown to show what category the user selected. I got it to work in a CodePen but now I'm struggling to get it to work over in our actual project. I used a little JQuery which is newer to me. The problem could be I might not have implemented it correctly within our Java program. I'm not quite sure yet. Here's what I wrote, 
```Jquery
$(".dropdown-menu li a").click(function(){
  var selText = $(this).text();
  $(this).parents('.dropdown').find('.dropdown-toggle').html(selText+' <span class="caret"></span>');
});
```
Basically it is a click event that will update the dropdown text with the value of the category selected by the user. Works perfectly in my CodePen. Not so much in the actual project. But getting somewhere. Next up: get the code to work in the project & write a function to pull the Json category values according to the user selection. 

<br>__8/18/2021__<br>
Bootstrap dropdown successfully installed on the project site. Took some time to get the dropdown, search text input and search button to do what I wanted it to do. The dropdown wanted to hang out right to all of it, but I was able to create <div class="d-flex align-content-start flex-wrap"> around all of the elements. So now it's looking a whole lot better. I pushed it all to a new branch in our project called dropdown_menu. Tomorrow I will be working on getting the categories to pull based on selection along with the user input. 

<br>__8/17/2021__<br>
I spent a lot of time reading on the Google API about categories and searching stackoverflow today to get an idea of how to create a Bootstrap drop down menu of the categories of books for our Google Books API powered library project. I found several promising examples of drop downs, and I also found that Google Books API uses BISAC for North American genres which will be a big help in determining category names to try to pull. Tomorrow I will put my research into action and begin to code the drop down. I am looking forward to dipping my hands more into Bootstrap.

<br>__08/16/2021__<br>
Read the Google Books API starter section and searched around a bit about implementing it. One of my group members was able to pull the search through the API but was only getting 10 results to list, I found that if we use MaxResults we can pull up to 40 book listings at a time (the max Google allows). During our group meeting today we split up some user stories from our Trello board. I will be helping with the Google Book API to figure out the display of each book, also finding out if we can get a shortened description for our search results page, and creating a drop down menu to filter the categories prior to the search for books. These are all part of our MVP (minimum viable project). By next Monday we need to have a working landing page and at least 1 working feature complete.  

<br>__08/13/2021__<br>
I've been chipping away at a developer blog project built with Java. I am going through methodically and trying to understand each step in such a way that I could explain it during an interview. Something new and cool I learned today was that in the application.properties file if you change the spring.jpa.show-sql to equal true then run the application it will show that the tables are created in the database (MySQL) during the run inside of IntelliJ without having to go over to the MySQL workbench or command line. I think that is rather effective and nifty. I previously had always had false there and didn't fully understand what the options were.

<br>__08/12/2021__<br>
I've missed a few days entries. I have been researching APIs, studying Java and practicing some algorithms. I learned a lot from a recent coding challenge interview so I've been making a game plan to fill in gaps where I was weaker during the interview than I hoped to be and maintain the areas I am strong in. Building projects does help, but practicing explaining things out loud will also benefit me. 

<br>__08/09/2021__<br>
I worked on finding missing numbers in an array and printing them. I also worked on reserving a string. Practicing on HackerRank, CoderBytes, and in Replit. I've been working on assignments for LiftOff in the LiftOff assignment repo including adding my group project wire frames photos to my readme file there. I am beginning to work on user stories and wireframing for my flight deals personal project. It's fun to have a passion project and I'm excited about this one. I also have a leadership meeting today for the Women Who Code St. Louis leadership team. Overall a varied and productive day. 

<br>__08/08/2021__<br>
I forgot my entry last night - so updating now. Yesterday was class 2/8 of LiftOff. Our group was ahead of the game with WireFrames and User Stories. Our Mentor/TA Abbey talked through the project with us and viewed our wire frames and user stories. She told us we could categorize them by color on Trello. Red for minimum viable product (mvp), Yellow for next level features, and Green for the further reaching features. Basically we needed to widdle the project down a bit to make it attainable. If we reach the Red and have time we will shoot for Yellow and so on. We discussed at a team what should be in what category. We also got our GitHub repo set up with the bones of the project. We had some GitHub hiccups because Maven got checked in Springintilizer instead of Gradle but we battled and won the GitHub revert war. Now the project with Gradle is committed and ready for us to start making feature branches. We will discuss more Saturday morning. I am hoping we can each check out some user stories to work on at that point. I also set up a Google Account for our group to use to access the Google Book API, possibly also a Google Voice number for Twilio implementation.

<br>__08/07/2021__<br>
I met with my project team this morning. We finished wire framing out the pages for our project. We used [Miro](https://miro.com/app/board/o9J_l3L3mmw=/?track=true&utm_source=notification&utm_medium=email&utm_campaign=approve-request&utm_content=go-to-miro) which is a free tool. We also added to our user stories on [Trello](https://trello.com/b/BSdWDdNq/liftoff) and added descriptions to each card. We are all eager to start coding our project. Hopefully we get the go ahead during class on Monday. 

Additionally I am preparing for my interview today - learning about Amazon Web Services (AWS), and brushing up on more Java concepts and algogrithms. 

<br>__08/06/2021__<br>
I spent today studying for an upcoming Java interview. Practicing explaining OOP, Polymorphism, Inheritance, Abstraction, Encapsulation, etc. I worked a little on my dev blog project as well. 

<br>__08/05/2021__<br>
I fixed the MySQL schemas - funny thing how closing out the program and going back in after importing can really make a difference. It's the little things I tell you. I also have been working on my Java based blog project. I am glad I have been working on it because my JAVA_HOME wasn't set up yet after migrating to my laptop from my old desktop. Now it's all set up and ready to compile my Java applications, just in time for my LiftOff group project work to begin (we haven't started coding just yet, but will soon I imagine). My blog project will use Java, Spring boot, Maven, MySQL, hibernate and I am hoping to implement Angular framework with it. I haven't integrated Angular with any Java yet so it'll be a learning experience for sure.

<br>__08/04/2021__<br> 
I recently upgraded to a laptop from a older desktop. I thought I had everything migrated over, and then I tried to run my final project from LiftOff. The MySQL tables were nowhere to be found on my laptop. So today was about finding how to get those files onto my laptop from the old computer. So far I've got them imported but they are all inside one schema instead of separately into the schemas for the different projects. I'll have to find out how to organize them back to their proper order. I also did the coding challenge for week 2 of LiftOff. Which was to write function that retrives the minimum and maximums of an array. Here is what I came up with.

``` JavaScript

function minMax(arr) {
	let min = Math.min.apply(null, arr);
//console.log(min);

let max = Math.max.apply(null, arr);
//console.log(max);

return([min, max]);
}

minMax(arr);
```

<br>__08/03/2021__<br>
We have LiftOff! My team is 4 members. We planned our group project. We will be building a Library application where users can register and sign in/out. They can use a menu to sort genres, search for titles, check out a book, etc. We plan to build the project with Java, HTML, CSS, Bootstrap, Thymeleaf, Gradle, MySQL, Twilio API, and an API for book data (possibly Google Books). We have a basic experience with Bootstrap but didn't do a lot with it yet so we will need to learn that better. We also don't know Twilio so we will be figuring that out. I did do a Python tutorial once using Twilio but it was some time ago and this will be a first time figuring out how to use it with Java. Our team also created some user stories on Trello. We also created a wire frame of the landing page. Later this week we will finish wire framing and add to our user stories as needed. I am excited to get started on coding our project! 

<br>__08/02/2021__<br>
Took a little break from GitHub the past week or so while. Still practiced coding but not much uploading. I have my first technical interview tomorrow where I'll actually be answering technical questions and doing coding problems. Excited and nervous all at the same time. Today I am preparing for that interview - reviewing material and doing some alogorithm problems. I also start LiftOff tonight 5:30-8:30pm. I am looking forward to meeting my group, peers, TA and teacher. I am also looking forward to getting another project underway. 

<br>__07/28/2021__<br>
Officially set up for LiftOff on Canvas, Slack and GitHub. Completed the pre-work assigned to be done before our first session on Monday. Learned about wireframes, user stories and set up a Trello board for my project. Some project ideas I have for projects are a blog website, a vitamin cross checker to make sure you aren't getting too much or too little of specific vitamins, an ecommerce site maybe using the dog api to simulate how a shelter could sell the dogs in their care, a hotel and/or flight deals finder. I am also curious about Twilio. I used in to make a weather alert app with the help of an Udemy course, but I'd like to see how else it could be used. So I am thinking I might try to using the Twilio api in my project. It's hard to decide what would be the best project to build first.

<br>__07/20/2021__<br>
Spent time today going through some pre-work for LiftOff before it starts August 2. I brainstormed project ideas. I also did a little HackerRank and Eloquent JavaScript. 

<br>__07/19/2021__<br>
Took a few days break from coding due to some other obligations. Felt good to announce my portfolio website is up on Twitter and LinkedIn today. Fixed a few things on my resume and website. It's all a work in progress but I am proud of what I've accomplished thus far. I'm practicing leetcode today and preparing to start a personal project. Good times! Today is also the official last day of LC101 even though I finished a couple of weeks ago. I am told I'll have a certificate of completeion some time after today. It's the little things that mean so much.

<br>__07/15/2021__<br>
Practiced Java leetcode today. I worked on FizzBuzz and reversing an array. Here is what I came up with:
```Java
import java.util.Arrays;

public class Main {

    public static void main(String[] args) {
        // Run printFizzBuzz
        printFizzBuzz(100);

        // Run reverseArray
        int[] numbers = new int[] {1, 2, 3, 4};
        reverseArray(numbers);
        System.out.println(Arrays.toString(numbers));

    }

    public static void printFizzBuzz(int N) {
        for (int i = 1; i <= N; i++) {
            if (i % 3 == 0 && i % 5 == 0) {
                System.out.println("FizzBuzz");
            } else if (i % 3 == 0) {
                System.out.println("Fizz");
            } else if (i % 5 == 0) {
                System.out.println("Buzz");
            } else {
                System.out.println(i);
            }
        }
    }

        public static void reverseArray(int[] a) {
            for (int i = 0; i < a.length / 2; i++) {
                int temp = a[i];
                a[i] = a[a.length - i - 1];
                a[a.length - i - 1] = temp;
            }
    }
}

```

<br>__07/14/2021__<br>
Spent today finishing the screenshots and edits for my portfolio site. I also wrote detail pages and linked then up for my portfolio site. I also worked on figuring out how to host my project on my hosting plan. I have a site up! [christina-varghese.com](url) I still plan to make some changes and fix some things but I am happy it is up. 

<br> __07/12/2021__<br> 
I missed a few days of logging on here. I have been helping some peers with bugs in their final assignment for the bootcamp. It has also helped me understand the code I wrote better. I do not want to simply give them the code I did. So helping them requires me to formulate questions to ask them to lead them toward the answer. It is fun to see their ah ha moments. I have also worked some on my portfolio site. It isn't as far along as I had hoped, but it is taking shape. I have also been brainstorming a project to make with Java and Spring Boot for fun. I am eyeing a couple of fun APIs, but also have ideas to compare supplment ingredients. The hardest thing is choosing which project to make first.

<br>__07/08/2021__<br>
I broke the navigation links the other day on my portfolio side so I spent some time fixing those, and arranging things on the page, deploying a few projects. I also read/learned about how to deploy Java with Spring projects since GitHub pages doesn't work seemlessly with these types of projects. I plan to take a stab at that in the near future. Possibly using Heroku combined with GitHub. I also spent some time today networking with a fellow LaunchCode grad. He was very generous with his time and information. I really appreciated it.

<br>__07/07/2021__<br>
LC101 coursework is completed! I am on cloud 9 this afternoon!!! I just commited my final changes to the last studio of LC101. I am unofficially an LC101 graduate! Today I learned more about authentication and REST. I took a lot of notes in my studio to help me think through the process of what each method, variable, class, etc. was doing. It's nice to see how it all plays together. The rest of the week I'll be working on getting my portfolio website deployed so I can share it with the world! What's next? I am excited to work on some personal coding projects. I'm going to hit the ground applying to jobs, networking, reaching out to recruiters, and researching companies. Additionally, I'll be practicing some leetcode. Ready for the wild ride of job hunting! LaunchCode's LiftOff also begins August 2 and I plan to participate which will be a fun continuation of my personal goals and aspirations. I am really looking forward to meeting more people who are on a similiar path to me and also the many teachers and teacher assistants. Imposter syndrome sometimes rears it's ugly head - but the truth is I know I'm a great candidate with my previous professional skills as a long time educator (to name just a few: communication, organization, teaching, creatively finding soltions, etc.) along with the skills I gained from LaunchCode's LC101 Web Developer Bootcamp and the skills I picked up on my own previous to that.

<br>__07/06/2021__<br>
Domain and web host shopping today. Spent time comparing some well known web hosting companies and picked a domain. One step closer to deploying my personal portfolio site. I still need to add a few more things, and then upload and connect the domain to the hosting and the files. I should have it up this week if all goes to plan. Also on the docket for today was unit 2, week 10 reading. The topics for week 10 are authentication, REST, field names, HTTP status codes, and more. 

<br>__07/05/2021__<br>
Added screenshots of a few projects to my portfolio site. Worked on navigation kinks and anchor tags.  Also added icons for the programming languages, IDEs, frameworks, etc. I am familiar with. 

<br>__07/04/2021__<br>
Uploading final assingment (TechJobs-Persistent). I plan to finish up the portfolio site this week and also add more screenshots onto GitHub. Already thinking of ideas for more projects I can build for fun. 

<br>__07/03/2021__<br>
I assisted two peers today in debugging their assignments. Neither have finished completely but some of the hints and questions I gave/asked helped them pass some of the tests. I like helping others because it helps me to dig in and think more about why I did what I did and what I could do differently. I also spent time working on my portfolio website. I am almost ready to purchase a domain and hosting. 

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
