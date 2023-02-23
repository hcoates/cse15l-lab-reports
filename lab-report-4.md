Lab Report 4
==========

Steps
--------------

1. Setup Delete any existing forks of the repository you have on your account
2. Setup Fork the repository
3. The real deal Start the timer!
4. Log into ieng6
5. Clone your fork of the repository from your Github account
6. Run the tests, demonstrating that they fail
7. Edit the code file to fix the failing test
8. Run the tests, demonstrating that they now succeed
9. Commit and push the resulting change to your Github account (you can pick any commit message!)

1 Setup Delete any existing forks of the repository you have on your account
-------- 

<img width="326" alt="Screenshot 2023-02-23 at 11 23 26 AM" src="https://user-images.githubusercontent.com/114765933/221009405-71820f2e-73f0-46b9-a06e-a858966e5e75.png">

````
[cs15lwi23apk@ieng6-203]:~:342$ rm -rf l<tab>
````

The command rm -rf lab7 is used to delete the directory lab7 and recursively the files inside it.

2 Setup Fork the repository
------

<img width="836" alt="Screenshot 2023-02-23 at 11 29 02 AM" src="https://user-images.githubusercontent.com/114765933/221010562-43bd1efc-0724-479c-b33d-d0edd045ce21.png">

From the lab7 repository linked on the week 7 lab directions, I forked the repository.

4 Log into ieng6
------

<img width="502" alt="Screenshot 2023-02-23 at 11 31 36 AM" src="https://user-images.githubusercontent.com/114765933/221011056-6739964d-1fe0-4292-b039-3214de6069e8.png">

<img width="504" alt="Screenshot 2023-02-23 at 11 32 55 AM" src="https://user-images.githubusercontent.com/114765933/221011304-68414827-2381-4182-a9bc-d4e8e3b94d20.png">

````
<^R> ssh <enter>
hannahcoates@Hannahs-MacBook-Air-3 ~ % ssh cs15lwi23apk@ieng6.ucsd.edu
````

I used ^R to search through the command line history to ssh into the ieng6 machine.

5 Clone your fork of the repository from your Github account
------

<img width="522" alt="Screenshot 2023-02-23 at 11 34 45 AM" src="https://user-images.githubusercontent.com/114765933/221011644-0ffcbab5-96fa-4f0c-a21d-0b142a89ec8c.png">

````
[cs15lwi23apk@ieng6-203]:~:345$ git clone git@github.com:hcoates/lab7.git <enter>
````

I ran git clone to clone the lab7 repository onto the machine.

6 Run the tests, demonstrating that they fail
------

<img width="569" alt="Screenshot 2023-02-23 at 11 38 56 AM" src="https://user-images.githubusercontent.com/114765933/221012453-99da635f-1f97-4a2e-89a4-76c93ff8301c.png">

````
cd l<tab>

<cmd+c> <cmd+v>
[cs15lwi23apk@ieng6-203]:~:346$ javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java

<cmd+c> <cmd+v>
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore T<tab>
````

The javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java  command was copied and pasted. Then the java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore command was also copied and pasted. 


7 Edit the code file to fix the failing test
------

<img width="571" alt="Screenshot 2023-02-23 at 11 43 43 AM" src="https://user-images.githubusercontent.com/114765933/221013398-19f2a9cb-545d-494c-b04a-f640195a7720.png">

<img width="565" alt="Screenshot 2023-02-23 at 11 44 10 AM" src="https://user-images.githubusercontent.com/114765933/221013479-f9b97d11-8471-4671-a182-eb3eaac13a9d.png">

````
[cs15lwi23apk@ieng6-203]:lab7:355$ nano L<tab>java

Keys pressed:
<^W merge>
<down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down><down>
<left><left><left><left><left><left>
<delete> 2

<^X> y <enter>
````

To correct the code in the file I searched for the method name and then keyed down and left until I got to the part I needed to fix.


8 Run the tests, demonstrating that they now succeed
------
<img width="569" alt="Screenshot 2023-02-23 at 11 48 28 AM" src="https://user-images.githubusercontent.com/114765933/221014343-a61259ad-3e5b-4ad0-bd06-bee3f7e68875.png">

````
<up><up><up><enter>
[cs15lwi23apk@ieng6-203]:lab7:356$ javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java

<up><up><up><enter>
[cs15lwi23apk@ieng6-203]:lab7:357$ java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples
````

The javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java command was 3 up in the search history, so I used up arrow to access it. Then the java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore command was 3 up in the history, so I accessed and ran it in the same way.

9 Commit and push the resulting change to your Github account (you can pick any commit message!)
-----

<img width="494" alt="Screenshot 2023-02-23 at 12 48 10 PM" src="https://user-images.githubusercontent.com/114765933/221026693-f3cb71dd-f400-460c-aa6c-0d1089f2f313.png">

````
[cs15lwi23apk@ieng6-201]:lab7:359$ git add L<tab>java
[cs15lwi23apk@ieng6-201]:lab7:360$ git commit -m update
````

