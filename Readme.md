
# Task Manager Telegram Bot

A Task Manager Telegram Bot built with OPCRouter and MSSQL, capable of creating groups of tasks and tasks inside of these.

## Functions

Here lies all the bot functionallities, with examples on how to use them, as well as it status, implemented or not yet.

- [x] **/Start:** starts a chat with the bot. By using this command you agree to have your telegram data (username, forename and surname) saved on the bot database;
- [x] **/Newtaskgroup {name (min. of 4 characteres)}:** creates a new empty Task Group;
- [x] **/Newtask #{group id} #{title (min. of 4 characteres)} #{description (optional)}:** creates a new Task inside a Task Group. ***Note: '#' are necessary to identify each paramter***;
- [x] **/Task {id}:** shows details of a task;
- [x] **/Concludetask {task id}:** marks a Task as concluded;
- [x] **/Deletetask {task id}:** deletes a Task. ***Note: this action can not be reverted, use it carefully***;
- [x] **/Deletetaskgroup {task id}:** deletes a Task Group. ***Note: this action can not be reverted, use it carefully***;
- [x] **/Taskgroups:** shows all task groups the user has;
- [x] **/Taskgroup {group id}:** shows details about a task group;
- [x] **/Stop:** End the chat. ***Note: all your data will be deleted from the bot database, including your tasks.***

### To-do and Improvments

- [x] Merge **/Allmygroups** and **/Mygroups**.

>The project will be considered under development while the taks above are not completed.

# IMPORTANT
The bot itself is not configurated on the current project for safety reasons, so you will need to create one and include it on the project as it will be explained below. 

## 💻 Requirements and Setting Up

**Development:**<br>
The app was built with OPCRouter 4.26 and Microsoft SQL Server Managment Studio 18. Both files (OPCRouter project and MSQLSMS project) can be found inside this repository. You wil need to import both projects, and then link the created bot to OPC by replacing the Mockup Bot Id present in the telegram plugin to a real one.

**Bot usage:**<br>
Because it's a Telegram bot, you will need a Telegram account to interact with it, once you've configurated it.

## Footnote

> This project was created for studying purposes, only. There are no plans for future support, with news features or improvements, for example.
