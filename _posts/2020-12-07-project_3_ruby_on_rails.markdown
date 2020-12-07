---
layout: post
title:      "Project 3 : Ruby on Rails"
date:       2020-12-07 06:41:26 +0000
permalink:  project_3_ruby_on_rails
---


The content of your blog post goes here.Project 3 : Ruby on Rails

I create a elearning platform where students can register for a course and review a teacher. I start the app by making a 

directory (Mkdir 3_p) and then run rails new rails_elearning to generate a new application and use "cd rails_elearning"

to get into the app. I first of all create a User Model by using the command "rails g model User" then that command 

creates a model users and table users. The table user will have an attribute called "name". Inside the Model User, we 

defined couple relationship. I set up a rails device gem so that the user of the app gets authenticated through it. I used 

bundle install when I did put the gem 'devise' inside my Gemfile. After I run the command rails generate device:install to 

get the guidance about the next steps. The first step is to put  in config/environments/development.rb the following:

config.action_mailer.default_url_options = { host: 'localhost', port: 3000 }, then add a root_url which will be 

root"students/index". Finally we add rails g devise:views because we will like to customize our app. I did create devise 

User to set up the model and table. Once done, I run rake db:migrate to update my schema. I create a student with a 

resource generator and that creates a student Controller, Model and table. Inside the student controller I create a 

method called index and a view index. To make the navigation easy, I created a navBar. I place the navBar inside 

layouts/application_html.erb" so that the navBar shows up on every page of our app. Inside our navBar, we used the 

helper method user_signed_in? to display the log out button. After, I create a Course model, views and controller. Idid 

the same with Review. Then I add validation so that errors will occur if those element I specified in my validations are 

not present.
			



