# README
A repository for our second project on the engineering course at sparta global. Built in Ruby on rails.



The navigation bar starts with the logo which is used throughout this links back to the index page. Then there are links that show up based on the users permissions all users have a link to the published projects. A spartan, will have a link to their projects, a staff member will have a link to all projects and the index of spartans. At the end, If the user is signed in they will be shown buttons that link to be able to edit their account or logout.
If the user is not signed in they will be shown the form to log in and a button to the sign up page.

On mobile the links and the login and registration methods are hidden and a button is used to show them below the logo.

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

Notes on the index page for projects and users:
All projects are shown in a grid layout via the projects_each partial. However if you are logged in as a Sparta trainee you will be greeted with all your own projects. If you are logged in as a Sparta staff member you will see all projects by all trainees. If you are not a member then you will see all published projects.
All listed projects and users are represented in cards on their respective index pages. Three are shown on each line and are appropriately spaced out. The links have been placed in a footer and separated by lines.
The Spartan index page is styled to conform with the aesthetics of the projects index page. Only admins can see the index of all spartans. Spartans can be edited from this page and only non-staff members can by destroyed.

Notes on different user access:
Using 'spartan_signed_in?' to restrict access to logged in users only and 'current_spartan.admin' to restrict access to admins only, different kinds of users are able to access different features, for example only admins are able to edit another user's project.

Notes on styling:
White background used throughout for consistency and minimalist styling.
Grey backgrounds behind text for ease of reading.
Font size minimum 16px for ease of reading.
Overwrite of bootstraps visited link colour for consistency.
Sparta colours used throughout for consistency.

Notes on admins deleting user accounts:
Admins are able to delete non-admin accounts, they are not able to delete other admins.

Notes on new and edit forms:
Forms have dropdown menus which allow the user to attribute the project being created or updated to a particular spartan. They also have margins on the left and right to be easier to read.