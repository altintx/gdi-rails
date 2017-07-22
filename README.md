# INTRO TO RAILS
This is an Intro to Rails course, intended for eventual inclusion in the Girl Develop It Core Curriculum. Based on material by Cheri Allen, inspired by Railsbridge.

The course is meant to be taught in four two-hour workshops. Each of the slides and practice files are customizable according to the needs of a given class or audience.

Cheri's slides can be viewed [here](http://cherimarie.github.io/gdi-core-rails/#/).
## Outline

This course is four 2H classes, with two consecutive classes on two consecutive Saturdays.

### Class 1: Introduction

*  What is GDI
*  What is Rails
*  Compare Rails with PHP
*  What's the split between Ruby & Rails
*  Ways to use Rails (front+back end vs just backend)
*  We'll be doing front+back
*  We'll be doing Rails 5
*  What kind of apps does Rails do well
*  What kind of apps does Rails not do well
*  Rails command line tools
*  Exercise: Verify (and correct) installation
*  Exercise: Bundler (verify installed, install if neccessary)
*  Exercise: Verify and install Rails CLI tools
*  Exercise: Make an apps (use Rails)

### Class 2: Data modeling
* Let's build a blog
* How do you identify models? What's the relationship between models & screens? (Data modeling for a blog)
* Exercise: Scaffold a single model blog
* Discuss how requirements change and migration's role in them
* Discuss data relationships
* Exercise: Scaffold an Author; create a migration to add Post belongsTo Author
* Attempting to test will fail because of pending migration
    * how to run migration
    * Now can demo feature; demonstrates hasMany and belongsTo
    * Add Author UI to post/index & post/view
* Now discuss hasAndBelongsToMany
* Exercise: Add comments
    * Scaffold comments
    * Add hasMany relationship to Post
    * migration is different this time. Why? 
    * Add UI to post/view
* Stretch material: Asdd validation if time allows. 

### Class 3: Routing
* Quick review
* REST
* Routes
* Pretty URLs
    * Exercise: Lets make Authors be /author/name instead of /author/1
        * add a slug to author
    * Exercise: how bout posts too
        * add a slug to posts
    * Comments probably doesn't make sense. Why?
  * Demonstrate that link helpers kept our links working
  * Show ```rails routes```
  * Exercise: Filter posts by Author
      * go to /posts?tag=blah or /posts?author=sam
  * Nested Routes
      * /authors/sam/posts
      * make posts be nested under author
* Stretch material: see all comments by a particular email address

### Class 4: Advanced
* Let's send an email to post author when a comment is added
* ActiveMailer
* Test with letteropener gem
* How do you actually run all this?
    * Heroku - easy but costs
    * nginx - mention web servers course
* Stretch marterial: partials. Make an author partial that is included on blog page.
  

## Promotional Blurb
Ready to build on your basic Ruby knowledge to start building full web applications? It's time to learn Rails! 

Rails is a framework that makes creating web applications relatively quick and easy. There is a thriving community around it, a strong job market, and ample resources available to beginners. Rails powers applications like Living Social, Groupon, Twitter, Square, Github and more.

Through classroom instruction, and group excercises, you'll get a solid introduction to the fundamentals of building Rails applications. By the end of the course, you'll have built at database with changing requirements, and a blog, installed and used gems, sent email, and , added pretty URLS (search enginge optimization).

_Please prepare for this class by setting up your development environment_, following this guide: http://docs.railsbridge.org/installfest/. Continue through 'Create a Heroku Account.' 

Note: Rails works best on something based on Unix (Mac or Linux). Using Windows 7 or 8 will be harder. If you have Windows 10, install the Subsystem for Linux and things will be fairly good. If you have something less than Windows 10, install https://git-scm.com/downloads and hope for the best. 

At this time, you will need to provide your own laptop to participate in the course.


