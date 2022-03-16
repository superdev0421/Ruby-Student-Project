# Stukent Champ Challenge

This is a hiring test for potential Stukent employees who are interested in working on our Ruby on Rails projects. The challenge is designed to see how well the candidate can learn new things in Rails and configure it to be used with a Single Page Application (SPA). This is a Rails 5.1 application. In order to complete the challenge you will need to use `ruby 2.4.1` and `yarn`. If you use rvm, the `.ruby-version` and `.ruby-gemeset` files are already created for you.

## The Challenge
The candidate will complete the outlined steps below. For each step there should be at least 1 git commit so that the history of the application can be viewed at each step. If you cannot complete the step, create a commit message for that step and explain where you got stuck and why in the commit message. Then proceed to the next step.

  1. Clone this repository and setup the application to get it working in the development environment on your machine.
  1. Change the database from using sqlite to postgres.
  1. Add 5 ficticious posts using the application.
  1. Add the Spectre (https://picturepan2.github.io/spectre) CSS library to the application and test it to make sure it is working correctly.
  1. Using the Spectre library, update the look and feel of the scaffold to your liking. Do not spend a lot of time on this, just make it look better than the raw Rails scaffolding.
  1. Update the application to add the following feature: Whenever a post is created or edited, the factorial of a random number between 1 and 10 should be calculated and shown alongside the title of post in the `show` action. For example, a title could be `My Post about Factorials 120` where 120 is the factorial of 5. Every time the post is created or edited the factorial number should change. The number you generate should be located in its own database column and the actual title should remain as the user entered it so that when they edit a post they do not see the factorial number.
  1. Using the pre-installed webpack and react libraries, rewrite the posts scaffold as a single page react application (SPA). Move all JS and CSS into the SPA so that it is being compiled by webpack. Feel free to modify the application in any way to make it a good user experience. Make sure that all CRUD operations on posts can still be performed. Do not use CoffeeScript. Incorporate language features from ES6 and later. You may use Redux if you wish but it is not required.
  1. Move the factorial calculation to the client-side SPA so the application continues to function as it did previously when it was being calculated in Rails.
  1. Take some time to use your own innovation and creativity to improve the app. Add some complexity technically and/or give it a visual makeover. Describe what you did and why in the git commit comment.


## Challenge Submission
To submit your completed challenge, please perform the following:

  1. Export your PostgreSQL databse using `pg_dump` and save it to the root directory of your application. Name the dump file `champ.dump`
  1. Zip up the champ directory into `[YOUR NAME]_champ_challenge.zip`.
  1. Email your zip file or send a download link to `turbo@stukent.com`

