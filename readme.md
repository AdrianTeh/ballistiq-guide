# Ballistiq Software Development Guide

This guide provides information about how Ballistiq works and our recommended practices for software development.

## Project Management and Collaboration

Ballistiq uses Basecamp and Pivotal Tracker for collaboration.

* Basecamp - All business issues, client interaction, design, etc.
* Pivotal Tracker - Software development stories and issue tracking

## Time Management

At Ballistiq, we track time for all software development projects. All developers must enter their times into [Time Tracker](http://time.ballistiq.com) at the end of each day.

We recommend using the [Pomodoro Technique](http://www.pomodorotechnique.com/) for managing time and estimating time. It works effectively by breaking everything down into 25 minute "Pomodoros". Get the [Pomodoro App](http://www.pomodoroapp.com/) to start using Pomodoro in your workflow.

## Git
Ballistiq uses Git for source control. All our projects are hosted on Github. All technical staff are expected to use Git command line. Non-technical staff can use the [Github App](http://mac.github.com/).

## Development Workflow

1. Before starting work on a feature, you must set the corresponding task on Pivotal Tracker to "Started".
2. The feature should be implemented in a separate git branch named as such: {your initials}-{task id}-{task description}. E.g. "LT-12345-add-comments-to-posts"
3. When the task is completed, you should mark the task as "Finished" in Pivotal Tracker and also set it to "Deliver". 
4. Get your code reviewed by a colleague. Do a pull request. 
5. The reviewer should check the pull request. If it all looks good, just leave a comment saying, "LGTM" (Looks Good To Me) or similar.
6. After review, the author should then do the merge into master. Rebase your commits Ensure that all tests run before pushing to Github. You should delete the local and remote temporary branch. 
7. The project lead will Accept/Reject the task on Pivotal Tracker as per client feedback.

### Master branch

The Master branch is expected to be the canonical stable source branch. As such, Master should always strive to be the branch where all tests pass and that the software is stable.


## Ruby on Rails



## Deployment

## Monitoring

## Training

## Equipment / Software