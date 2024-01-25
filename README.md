# QuizNow-Application

This is the core application for QuizNow, including the tables and business rules and the workspace and game app that supports it.  This depends on the [QuizNow-Component repo](https://github.com/ServiceNowNextExperience/QuizNow-Component) which contains the code and the server configuration for the component to render the questions and answers.

## Install

### Load App into your Instance
In your instance go to Studio > File > Import from Source Control TWICE and import these two application repos
```
https://github.com/ServiceNowNextExperience/QuizNow-Application
```
```
https://github.com/ServiceNowNextExperience/QuizNow-Component
```

### Load Sample Data

In the root of this repo is a file called [QuizNow Sample Data Update Set.xml](./QuizNow%20Sample%20Data%20Update%20Set.xml) which contains sample data.  Download that file then go to "Retrieved update sets" in your instance and use the related link to import this file, preview it and commit it.

### Try it
There will be two new experiences in UI Builder (UIB):

1. QuizNow Workspace (for editing and administering quizzes): `/now/quiznow-workspace/home`
2. QuizNow Game (for playing the game): `/now/quiz/play` (If you loaded Demo Data you may use the code "XYZA" and enter any screen name to start, otherwise go create a Quiz and Quiz Instance using the workspace)
