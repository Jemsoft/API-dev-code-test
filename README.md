# Jemsoft API Developer Code test

This is a simple project based code test to be completed using hosted version control to allow us to gauge your skills, aptitude, practices and workflows.
###Stack
 - Node Framework: Loopback
 - Database: MongoDB
 - ODM: Mongoose
 - Testing Framework: Jasmine or equivalent
 - Task Runners: your choice of grunt, gulp, bower, etc.
 - Authentication: Oauth (cooked into loopback)
 
###Workflow
 - Use the built in yeoman generator, this will save you time and build your routes and models.
 - Github to be used for version control
 - Gitflow (or feature branch at a minimum) workflow to be followed
 - Test-driven development is favourable, good test coverage is imperative
 
###What we'll be looking for
- Clean, intelligent code
- Re-factoring (we don’t want ‘perfect' code, but we do expect robust, commercial, scalable code)
- Small, re-usable modules, classes, functions
- Third party (open source) code re-use  (we don’t reinvent wheels)
- Dev-ops (task runners such as grunt or gulp, automated testing, etc)
- Consistent syntax and commenting
- Responsible use of callbacks and nesting
- Intelligent error handling

## ***Bonus Round!***
- node.js - cluster friendly/oriented code (the API you’ll be working on if hired will serve tens of millions of calls per month)

##Brief
A lot (most) of the functionality requested is provided by loopback and associated open source projects. We won’t hate on you for rolling your own modules, it's just not necessary.

Using loopback.js create a simple restful API to handle images in both persistent storage and in volatile memory operations (controlled via a header option).

Another header option shall be whether the image is accessible publicly or via their api key only. default should be public. Admin roles can access all images.

The API should allow users to store their own images with both an auto generated alphanumeric ID and a self chosen label, either in a database to be readable and editable later, or in memory only for handling until their session is closed;

They shall be able to add attributes and tags to the image dynamically, as well as add comments to the image.

Implement API metering per access key. All read calls to a publicly exposed image shall be appended to the meterage of the image owner’s account.

The only endpoints strictly required are one to handle and interact with image resources, and one to check account properties such as api call quota usage.

The Endpoints , stack, workflow, and deployment workflow shall be documented in a readme.

The project should be hosted for free on Heroku, AWS, or similar.

Just to reiterate, almost all of the functionality required here is provided by loop back and the opensource loopback gateway, so what we'll be looking closely at is any changes you choose to make outside of the yeoman generator.




