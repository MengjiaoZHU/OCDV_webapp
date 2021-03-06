# OCDV_webapp  

The goal of our OCDV project is to develop a web-app deployed on AWS. The technique stack is MEAN Stack, which represents for  "MongoDB", "Express", "AngularJS" and  "Node.js".
 
**What we have:**
 
Currently, we have already implement a template front end design and a backend for register and login functions. As for the front end design, it is only basic HTML and CSS. For our backend, we implemented it in Node.js with Express and MongoDB, also we have a simple front end written in AngularJS.
 
_Front End:_  

Our front end design is currently implemented with Angular 2. For now, our interface design contains mainly three parts,

1) The information pages that provide various resources and information that users might need, including locations of Family Justice Centers, testimonials, technology tips for using the app safely, etc. 

2) The OCDV portal that users can log in, upload and manage their records of incidences, evidences of being abused, and keep track of their court days, etc. The portal is not fully functional yet within the newly deployed version on AWS. We'll fix that soon.

3) Escape button: This function is to help users quickly close our website without any trace in case the abusers suddenly come. By clicking this button, user will be redirected to a new tab and redirects the old page to google to hide the browsing history.  

_Back End:_  

According to what we get from Family Justice Center (FJC), we have implemented a completed register, login and authenticate functions, where the user information will be written into MongoDB "mongodb://localhost:27017/meanauth". For now we only ask for users' email, name and password (which has been encrypted for security reason).  
 
Also, for each user, we have design profile, dashboard pages for them, the details of which have not been implemented. Before login, users cannot see the buttons of "Profile", "Dashboard" and "Logout"; after they login, they cannot see "Register" and "Login" buttons.  
 
**What functions we are going to have:**  

All information to display should be read from our database.  

1.	*Profile function:*  
Show user's basic information and the history of her interaction with FJC, such as when she has sought help from FJC, what material she has uploaded, .etc.  
 
2.	*Record the proof of domestic violence:*  
Users should be able to upload images and files to record their domestic violence in order to be as proof for future use. Also, there should be a textbox that they could write descriptions.  
This should be a button in "Profile" page.  
 
3.	*Dashboard function:*  
Show incoming appointments with FJC or attorney, also the events or activities held by FJC. 
Should be worked as a reminder page, better to connect with personal calendar.  
 
4.	*Escape function:*  
This function is to help users quickly close our website without any trace in case their husband suddenly come. The button should be placed on a conspicuous position.  
By clicking this button, user will be redirected to another website, such as google homepage and the "go back" button on the browser cannot be used. Also there won't be any record in browser history.  
 
We will have more user interaction functions which need to discussed with FJC.  

**Run:**  
1.	Enter into "test_meanstack" folder  
2.	Run "node app" in terminal  
3.	Enter into "angular-src" folder  
4.	Use another terminal window to run "ng serve"  
5.	The node.js part is running on "localhost:3000",  
The AngularJS part is running on "localhost:4200"  
 
