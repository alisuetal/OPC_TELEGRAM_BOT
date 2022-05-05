
# Task Manager Telegram Bot

A Task Manager Telegram Bot built with OPCRouter and MSSQL, capable of creating groups of tasks and tasks inside of these.

## Functions

Here lies all the bot functionallities, with examples on how to use them, as well as it status, implemented or not yet.

- [x] **/Start:** starts the Bot chat. By using this command you agree to have your telegram data (username, forename and surname) saved on the bot database;
- [x] **/Newtaskgroup {name (min. of 4 characteres)}:** creates a new Task Group so you can create Tasks inside of it;
- [x] **/Newtask #{group id} #{title (min. of 4 characteres)} #{description (optional)}:** creates a new Task inside a Task Group. ***Note: '#' are necessary to identify each paramter***;
- [x] **/Task {id}:** shows details of a Task;
- [x] **/Concludetask {id}:** marks a Task as concluded;
- [x] **/Deletetask {id}:** deletes a Task. ***Note: this action can not be reverted, use it carefully***;
- [x] **/Deletetaskgroup {id}:** deletes a Task Group. ***Note: this action can not be reverted, use it carefully***;
- [x] **/Mygroups:** shows the User their first 10 Task Groups;
- [x] **/Allmygroups:** shows the User all their Task Groups;
- [x] **/Group {id}:** shows the User a specific Task Group, and it's Tasks;

### To-do and Improvments

- [ ] Merge **/Allmygroups** and **/Mygroups**.

>The project will be considered under development while the taks above are not completed.

# IMPORTANT
The bot itself is not configurated on the current project for safety reasons, so you will need to create one and include it on the project. 

## 💻 Requirements

**Development:**<br>
The app was built with OPCRouter 4.26 and Microsoft SQL Server Managment Studio 18 .

**Bot usage:**<br>
Because it's a Telegram bot, you will need a Telegram account to interact with it, once you've configurated it.

## Footnote

> This project was created for studying purposes, only. There are no plans for future support, with news features or improvements, for example.
