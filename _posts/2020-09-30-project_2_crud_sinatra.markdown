---
layout: post
title:      "Project 2 : CRUD Sinatra"
date:       2020-09-30 14:34:05 +0000
permalink:  project_2_crud_sinatra
---


The content of your blog post goes here.Project 2 : CRUD Sinatra

I  finished building my first full-fledged Ruby app using Sinatra.The project was done as part of my coursework for Flatiron's Full Stack Developer Program.

This post is a basic wrap-up for the project, including how I got started.The first thing I did was not to  code, but write out a basic overview of what the app needed to do :

 User can create, read, update and delete an linetracker.

Interface:  user can view linetracker form ,  user can submit linetracker form ,  user can edit linetracker, user can delete linetracker



User class :   attributes => username and  password ,  user signs up/ log in , has many linetrackers

			
User controller and views :   '/users/signup '=> renders sign up form , 'users/signup' => processes sign up form , creates user ,  post ,  '/users/login' => renderslogin form ,  '/users/login' => processes login form , post ,  need to set sessions

,  user can view their linetrackers, '/users/:id/linetrackers'
			 
			 
			 
			 
linetrackers class :   attreibutes => name, country, currency, date, time, amount, notes , linetracker belongs to user
			 
			 
			 
linetracker controller and views :   '/linetrackers/new' => renders new order form , '/linetrackers' => submit linetracker

, '/linetrackers' =>  renders all linetrackers , '/linetrackers/:id' =>  renders one instance,  '/linetrackers/:id/edit' => renders update form for an instance

, 'linetrackers/:id' => updates instance  ,    '/linetrackers/:id/delete' => deletes instance
			 
After I had a clear idea of what my project was going to look like, I used "corneal new " command to create my 
sinatra environment . In my Controller,  I have an  application_controllers where I  enabled sessions and created a method called helper. In addition, in  th app directory, I also created three more files called user_controller, linetracker_controller and session_controller. First in the user_controller, I set up the sign up route. Second, in the session_controller, I set the log in and out routes. Finally, the rest of the routes are put in the linetracker_cottroller to impliment the CRUD  functionality. In my model, I created two classes: user and linetracker. Those two classes will inherit from ActiveRecord some macro. In the user class, I used the macro "has_may" linetrackers, has_secure_password to be able to use password_digest to protect the user password. While in the linetracker class, I used the macro "belongs_to" user. Finally in the the view directory, I created two folders: users and linetrackers. In those deux folders, I created different files that I will be able to put HTML, CSS, and Ruby code to be rendered and used rake  to create my tables users and linetrackers.


	 
			



