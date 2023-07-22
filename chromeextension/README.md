# CS50x final project extension
#### Video Demo:  <URL HERE>

#### Description:
A chrome extension which when used converts all the images present in the **google chrome tab** to famous bollywood actor **ShahRukh Khan**.This project was inspired by my fan love for SRK and his films. As CS50 helped me in learning different skills, I made this extension as a tribute to SRK and CS50x.

## About ME:
Hello everyone, I am Abhinav Gupta and I am from Durgapur, West Bengal, India. Previously I have undergone through the whole process from week 0 to week 9 and I am here today completing my final project.

## Technologies used in my project:

I have built this project using html, css, json and javascript and I have added screenshots in the video and in this project file.

## Files used:

#### 1. manifest.json:

Over here in this file I have used **manifest version 3** which is supported by google chrome nowerdays. Older manifest versions include 1 and 2. In the name section I have named my file as **CS50 final project extension**. Currently I have made this version **0.0.1** as this is the newest version of this extension ever made by me.
The **content_scripts** contains all the _urls_ on which the project will work upon and for the javascript to execute I have created a file called **content.js**.
For the background service worker I have created a blank file called *background.js*. 
The **icons** are added using an attribute of json file called *icons* and 3 pngs of the same image( 16x16, 48x48, 128x128) have been added in *images* folder of the project file. The **action** on which when the file is executed will give out a notification using a default popup called **popup.html** and I have titled it as *cs50 fan*.
In order to get access from chrome, I have added a permissions attribute of **tabs** which gives access to all tabs. 

#### 2. content.js:

In this javascript we have loaded different ShahRukh Khan images using a tile called *cs50_images* and used a const as **siteImages** with *document.getElementsByTagName* as *img*. 
 We then added a chrome runtime listener by passing request, sender and Response. So if we request task as *srk*, our page gets loaded with different ShahRukh Khan images which we have loaded in **cs50_images**. After we have been abled to load different images on the *img* tags available on the web page, we pass the status as *done* and return the response on the console window using **sendResponse**.

#### 3. popup.html:

We have created a very simple html file with title **CS50_fan** and we linked *popup.js* javascript file and css file of *styles.css*. We then created a header where I have written what the file does on clicking a button. After that I have created a Click button over there which when clicked changes all the images on that page to SRK pictures.

#### 4. popup.js:

Here I have created a *btn.addEventListener* which gets executed which when clicked, lets a **queryOptions** active and then returns the tab id and executes a task called *srk* and which in response displays the status of *response* function.

#### 5. styles.css:

Here in the styles.css file, we have simply added margin and padding to the html file as 0,0 to the body section of **popup.html**. Next we have modified the header h1 by changing background-color, font-size, display and justify content. Similarly we have modified the button of *Click Me!!* using attributes as display, justify-content, align-items, width and height. 

#### 6. background.js:

I have created this javascript file and kept it blank as it was just for reference.

## Screenshots:

![Screenshot of the screen showing the screen.](/screenshots/Screenshot%20(114).png)

![Screenshot of the screen showing the screen.](/screenshots/Screenshot%20(115).png)

![Screenshot of the screen showing the extension.](/screenshots/Screenshot%20(117).png)





## Conclusion:

It was a very interesting project as I have created this project after learning deep concepts of javascript and it took me a lot of time studying and testing before implementing the code. I don't know that why my extension is not being displayed on the screen recording and hence I have attached screenshots in this **project** file.


## About CS50:

CS50 is a openware course from Havard University and taught by David J. Malan
Introduction to the intellectual enterprises of computer science and the art of programming. This course teaches students how to think algorithmically and solve problems efficiently. Topics include abstraction, algorithms, data structures, encapsulation, resource management, security, and software engineering. Languages include C, Python, and SQL plus students’ choice of: HTML, CSS, and JavaScript (for web development).

Thank you for all CS50.
Where I get CS50 course? https://cs50.harvard.edu/x/2023/
















