# WEBD 236 Lab 1 Starter

Blog engines represent a good problem to solve in an introductory web programming course.  A blog (a shortening of “web log”) is a place for a person to post their thoughts about any subject.  A blog post is an entry in the blog.  Blog posts have a title, content, tags, and a date of posting.  Your assignment is to write a simple blog engine that lets you post as many items as you wish.  We will be revisiting this assignment in subsequent labs (i.e. to hyperlink tags, add commenting, add authentication and sessions, etc.) So, it behooves you to do a good job here.

## Helpful Hints
  - You’ll only need one database table called “posts.”  This table should have five columns: the ID number, the date of posting, the title, the content, and the tags as a single text field (not as a related entity).
  - You should use SQLite (not MySQL) for this project.
  - Make sure that your project works on any server on any directory.  In other words, you should never hard-code a URL with the name or IP address of your machine.  We won’t be using your machine when we test it.  Also, you should not hard-code a directory name in your application.  It should run as [http://somename.glitch.me/index](http://somename.glitch.me/index).
  - Use the MVC framework developed in class.  This will help.
  - To keep data in forms, you will need to echo out the content of variables within tags.  For example, you may have something that looks similar to this:
  
    `<input type='text' name='title' id='title' value='<?php echo($title); ?>' />`

    Of course, you need to make sure that the variable `$title` has some content in it from the last post.
    
  - Remember that every operation that writes to the database should be followed by a redirect whereas every ‘get’ (generally) should be followed by a forward (i.e. a template render). 
