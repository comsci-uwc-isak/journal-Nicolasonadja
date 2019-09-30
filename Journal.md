Day 1
Today class was really impressive. I actually learm a lot at the beginning I was really confuse by the teacher style,
but as soon as he star explaining and giving the cource I knew that he know what his taking about.


Day 2
I remenber getting into the terminal of computer something I did not know about and playing around with the concept and key was really helpfull. 
AS now I can manage to  navigate throught the the terminal and even try to writte script in bast. 

Day 3
Today we started how first oficial class. I loved it I need to go throuht verythink this night but it wa really interresting.
- We started topic 3 and when into 3.1  reading acticle about the different type of network like PAN and LAN.
- we look at the types of topology like rings and star.
- Next we worked with raspberry Pi and on how to navigate throught access or write a code in it.

Day 4
As I was expecting today was great. I do not really know what is happenening but the time just go by in the class. I am really into the way Mr Rubben is teaching.
I was engagde with class event if I did not participate that much. 
I think that I am maybe the that is not fully comprehending computer science at this time because most of them star before me as, I change class at the middle of the semester without having any
prior knowlegde like carlos. But this I ereally feel myseft insides the class. It is going me the motivation to continu. 
We start to work on OSI and how every thing is connected. and that nothing will be possible without the physical part. We learn the different layer form the physical to the most abstract. 
The next part was the best we create a code in PUG that we translate into HTML for us to be able to use it in the terminal.

Day 5 
Today was really nice, we work one  donwloading and setting up WebStrom  and intergrate Ctylus, Coffeescript and Pug via out terminal.
In order to create a Webpage with the attribute we wanted, we  had to configurate the WebStrom prefferences to had all the features dwonload throuht the terminal.
Next we played with the code that was already constract for us by the teacher.

This is an example of the html code that I change in order to add a pisture:
doctype html
head
    title My first styled page
    link(rel='stylesheet' href='mystyle.css')
    script(type='text/javascript' src='interactive.js')
    link(rel='stylesheet' href='mystyle.css')
    title My first styled page
ul.navbar
    li
        a(href='index.html') Home page
    li
        a(href='town.html') My town
    li
        a(href='links.html') Links
h1 My first styled page
p
    | Welcome to my styled page!
    section
        nav
            ul
                li.title Study Earth
                li.robot
                    img(src='Earth.jpg' alt='Earth' width='10px')
                    article
                        footer
                            img(src='https://upload.wikimedia.org/wikipedia/commons/9/97/The_Earth_seen_from_Apollo_17.jpg')


DAY 6 (Sept 12)
Today class was relaxing, i am not saying it was too easy but i will say intertaining, we work on creating a logging page by using pug syntax that is convert into HTML. It was facination because as we were going toward the page started to look like a actual logging page. I did not expect that, because i thought it will be harder even if we haven actually work on the back end, I was really happy of the work I have done.



DAY 7 ( September 17)
For today we had class on Data security (app for Symmetrical Key cryptography)
To protect the data it possible to ENCRYPT THE DATA.

For the encryption to work we need it to be Symmetric.
Therefore we have a  
- A public key which is use and know by everybody.
- A private key which is only know by the the person sending the encrypt text.

For the next part of the class we work on on creating an encryption tool as a webside and that was really cool.
And I think when it will be done I may use it as a communication tool with friend.


DAY 8 (Sept 19)
Today in class we work on constracting the code for the encription tool, I can not wait to see it working to use it.
Te thing is in class sometime I feel really lost in class and I think I know why. It because the teaching methode of This year teacher is completely different from the teacher last years. This years I do not clearly see the seperation between the non ib 
lesson and the one that are part of the curriculum. Because even if I like learning new things that are also relevant, I really need to undersdant and clerly integrate what I need to know for the test as my grade need to go up.

DAY 9 (Sept 20)
In class today we worked on pur Ai espetially on the ER diagram to represent the entity pof the data base for our website
Honestly i haven finish it the diagram but I will keep working on it and hope to have it done by the end of this month. Also I really need to get back my licence for SKETCH in oder to get back my design for all the Student page and the admin page.

DAY 10 (Sept 26)
Today in class we work on creating a data base, on Php in order to add the information form our previous login page we create. I find the class really engaging and now I think my plan in Cs are to study for the next week test in order to get a good grade. I hope the test will be too much hard as I need a higher pg. But definetly I will go throught all the content of the chapter to be ready for next week.


DAY 11 ( Sept 27)
http://github.com - automatic!
[GitHub](http://192.168.6.34/welcome.html)

<?php
   include("config.php");
   session_start();
   if($_SERVER["REQUEST_METHOD"]=="POST"){
       //username and password sent from form
       $myusername = mysqli_real_escape_string($db,$_POST['username']);
       $mypassword = mysqli_real_escape_string($db,$_POST['password']);
       $sql = "SELECT id FROM admin WHERE username = '$myusername' and password = '$mypassword'";
       $result= mysqli_query($db,$sql);
       $row = mysqli_fetch_array($result,MYSQLI_ASSOC);
       $active = $row['active'];
       $count = mysqli_num_rows($result);
       //If result matched $myusername and $mypassword, table row must be 1 row
       if ($count == 1){
           $error = "good";
           header("location:welcome.html");
           die();
       }else {
            $error = "Your Login Name or Password is invalid";
       }
   }
?>
<html>
<?php echo $error; ?>
</html>


The precedent code is the code that we use to create the logging page. 
The result is
![Image of my page ](
