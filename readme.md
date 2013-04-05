# Ballistiq  Software Development Guide

This guide provides information about how Ballistiq works and our recommended practices for software development.

## Tracking User Stories, Issues, and Bugs 

Ballistiq uses Basecamp and Pivotal Tracker for collaboration.

* Basecamp - business issues, client collaboration, mockups/designs, etc.
* Pivotal Tracker - User stories and issue tracking

## Time Management

At Ballistiq, we track time for all software development projects. All developers must enter their times into [Time Tracker](http://time.ballistiq.com) at the end of each day.

We recommend using the [Pomodoro Technique](http://www.pomodorotechnique.com/) for managing time and estimating time. It works effectively by breaking everything down into 25 minute "Pomodoros". Get the [Pomodoro App](http://www.pomodoroapp.com/) to start using Pomodoro in your workflow.

## Git
Ballistiq uses Git for source control. All our projects are hosted on Github. All technical staff are expected to use Git command line. Non-technical staff can use the [Github App](http://mac.github.com/).

## Development Workflow

In general we will try to use [Github Flow](http://scottchacon.com/2011/08/31/github-flow.html).

The Master branch is stable source branch and is deployable via production branch.

### Feature Development Workflow

1. Before starting work on a feature, you must set the corresponding task on Pivotal Tracker to "Started".
2. The feature should be implemented in a separate git branch named as such: {your initials}-{task id}-{task description}. E.g. "LT-12345-add-comments-to-posts"
When the task is completed, you should mark the task as "Finished" in Pivotal Tracker and also set it to "Deliver".
3. Get your code reviewed by a colleague. Do a pull request.
4. The reviewer should check the pull request. If it all looks good, just leave a comment saying, "LGTM" (Looks Good To Me) or similar.
5. After review, the **author** (not the reviewer unless there are time constraints) should then do the merge into master. Squash commits `using git merge --no-ff my_branch`. Ensure that all tests run before pushing to Github. You should delete the local and remote temporary branch.
6. The project lead will Accept/Rejectect the task on Pivotal Tracker as per client feedback.

# Web Development Guide

## Ruby on Rails

Web app development is in Ruby on Rails. Specific technologies we use in Rails are:

* [Rspec](https://github.com/rspec/rspec-rails) for testing
* [Factory Girl](https://github.com/thoughtbot/factory_girl) for test factories
* [Paperclip](https://github.com/thoughtbot/paperclip) for files/attachment handling
* [Capistrano](https://github.com/capistrano/capistrano) for deployment


### Ruby Style Guide

* Configure your text editor to:
  * Use 2 space indentation. Indent with spaces.
  * Automatically delete trailing whitespace.
* Comment your code! Don't expect your code to be "so beautiful and readable" that people will understand it.
* Follow [Github's Ruby Styleguide](https://github.com/styleguide/ruby)

### Front end
Front end development technologies:

* [Slim](http://slim-lang.com/)
* [SCSS](http://sass-lang.com/)
* [CoffeeScript](http://coffeescript.org/)

Style guides:

* [Github's Markup Style Guide](https://github.com/styleguide/templates)
* [Github's CSS Style Guide](https://github.com/styleguide/css)
* [Github's Javascript Style Guide](https://github.com/styleguide/javascript)

## Servers

We generally use Amazon EC2 for all our hosting needs. Technologies we use are:

* Ubuntu 12.04 LTS
* [RVM](https://rvm.io/) - Ruby version manager
* Imagemagick for server side image manipulation
* [Nginx](http://nginx.org/en/) web server
* [Phusion Passenger Enterprise](https://www.phusionpassenger.com/), Passenger Community Edition or Unicorn
* Amazon S3 for file storage
* Amazon Cloudfront for file delivery
* Amazon RDS - Mysql cloud hosting

## Deployment

Deployment of web apps should always be automated. For this, we use Capistrano.

## Monitoring

For monitoring, we use:
* New Relic - server performance/uptime monitoring
* Rollbar - error reporting
* Pagerduty - SMS when server/app is down

## Training

### Bootcamp / Basic Training

These training guides provided by [Thoughtbot](https://learn.thoughtbot.com) provide an excellent starting point for getting up to speed with everything. [CodeSchool](http://www.codeschool.com/) is also an excellent resource for learning many of these things.

* [Design](https://learn.thoughtbot.com/design)
* [Web Design](https://learn.thoughtbot.com/web+design)
* [Typography](https://learn.thoughtbot.com/typography)
* [CSS Grids](https://learn.thoughtbot.com/grids)
* [Visual Principles](https://learn.thoughtbot.com/visual-principles)
* [HTML & CSS](https://learn.thoughtbot.com/html-css)
* [Javascript](https://learn.thoughtbot.com/javascript)
* [SASS](https://learn.thoughtbot.com/sass)
* [Ruby](https://learn.thoughtbot.com/ruby)
* [Rails](https://learn.thoughtbot.com/rails)
* [SQL](https://learn.thoughtbot.com/sql)
* [Testing](https://learn.thoughtbot.com/test-driven+development)

#### General

* [Git](https://learn.thoughtbot.com/git)
* [Unix](https://learn.thoughtbot.com/unix)
* [Vim](https://learn.thoughtbot.com/vim)

# Mobile Development Guide

TODO
