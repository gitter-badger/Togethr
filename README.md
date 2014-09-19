Togethr
=======

Togethr is an open-source project that aims to increase access to care for the 73% of students who experience a mental health crisis during college. Of the 2.2 million students who sought counseling in 2012, 41% reported difficulty receiving treatment because of long waits and inconvenient services. 

Our Rails-based platform will offer a solution for the 88% of campuses that do not have the staff to accomodate the increasing number of students seeking help. We will provide virtual (text and video-based) counseling as well as convenient scheduling for in-person sessions. While students are on a waitlist, they will be able to text-chat anonymously with peers who are in a similar situation for immediate support. 



CITATIONS:
National Alliance on Mental Illness, 2012  ;
American College Health Association, 2012


##MVP Plan Overview
1. Design wireframes.
2. Plan issue requests and database associations.
3. Create landing page with counselor and student login and mailing list signup for students at schools that haven't signed up yet.
3. Create student signup requiring .edu email and liability waiver.
4. Create counselor signup requiring a passcode from Togethr.
5. Create student platform with appointment scheduling and text and video-chat sessions.
6. Create counselor platform with calendar, text and video-chat sessions, and session note tracker.
 

##Future Plans Overview
1. Create anonymous, text-based student-to-student support feature.
2. Implement reporting system where students and faculty recommend students that need help to counselors.



##Development Environment Setup
To get started,
* Install Rails. If you're using a Mac, we recommend [Rails Installer](http://railsinstaller.org). Under Ubuntu, follow the instructions [here](https://www.digitalocean.com/community/articles/how-to-install-ruby-on-rails-on-ubuntu-12-04-lts-precise-pangolin-with-rvm).
* Install Postgres. For Mac, we recommend [Postgres App](http://postgresapp.com). (If you're using Mac OS X Lion, you may need [this fix for Postgres](http://stackoverflow.com/questions/9354122/how-to-install-postgresql-9-1-on-osx-lion).) Under Ubuntu, follow the instructions [here](http://stackoverflow.com/questions/11092807/installing-postgresql-on-ubuntu-for-ruby-on-rails).
  
* Clone the Togethr Repo:  
  `git clone https://github.com/hilarybarr/Togethr.git`
  
* Install dependencies: 
  ```sh
  cd Togethr
  bundle install
  ```
  
* Configure the app for your local database by copying database.yml.sample to database.yml and adding a valid username and password. Make any changes needed for your database setup ( and possibly `rake db:create`).
  `cp config/database.yml.sample config/database.yml`
  
* Create database:  
  `rake db:create`

* Run migrations:  
  `rake db:migrate`
  
* Load helpful example data into your local database:  
  `rake db:seed`
  

* After installing these dependencies, test your setup by running `rails server` and visiting your site at [http://localhost:3000](http://localhost:3000)

You're ready to help change the world :-)
Shoutout to [CodeMontage](www.codemontage.com) for inspiration when setting up our project.

## License

Copyright (c) 2014 Togethr. See [LICENSE](https://github.com/hilarybarr/Togethr/blob/master/LICENSE) for details.
