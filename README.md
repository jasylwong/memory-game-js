# Learn enough Rails 

Rails is a web development framework written in the Ruby programming language.

---
## Chapter 1: From zero to deploy
---

###  1.1: Intro
#### 1.1.1 Prerequesites
See website for list of resources

#### 1.1.2 Conventions used in this book
### 1.2: Up and running
#### 1.2.1: Development environment

Three essential components needed to develop web applications:
- Text editor
- File navigator
- Command-line terminal

See website for steps for getting started with the cloud development environment.

#### 1.2.2: Installing Rails
```
$ gem install rails -v 5.1.6
```

### 1.3: The first application ("Hello world")

Start a new rails app using:
```
$ rails new app_name
```
See website for table of main directories in a Rails app

#### 1.3.1: Bundler
To install and include the gems needed by the app:
```
bundle
```
You may need to move sqlite into development and test environment in the Gemfile, to prevent potential conflict with the db used by eg Heroku.

#### 1.3.2: rails server
Run a local webserver to use app:
```
rails server 
```

#### 1.3.3 Model-View-Controller (MVC)
#### 1.3.4 Hello world!
Add a controller action (method) to render the string "hello world"
Then amend the routes.rb in ./config/ for the root: root 'controller_name#action_name'

### 1.4: Version control with Git
#### 1.4.1 Installation and setup
#### 1.4.2 What good does Git do you?
#### 1.4.3 Bitbucket
#### 1.4.4 Branch, edit, commit, merge

### 1.5: Deploying
#### 1.5.1 Heroku setup
Heroku uses the PostgreSQL db, so we need to add the pg gem into the production environment
(remember to also remove the sqlite gem from production environment, as the db is not supported at Heroku).
Run bundle with a special flag to prevent the local installation of any production gems (ie in this case, PostgreSQL):
```
$ bundle --without production
```
(See website for complete steps on deploying to Heroku)
Create a place on the Heroku servers for your app to live:
```
$ heroku create
```

#### 1.5.2: Heroku deployment, step one
```
$ git push -u heroku master
```

#### 1.5.4: Heroku commands
$ heroku help



---
## Chapter 2:
---

---
## Chapter 3:
---
