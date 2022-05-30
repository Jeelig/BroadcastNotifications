# BroadcastNotifications
Simplifies notifications for Dynamics 365 and generally Model Driven Apps

![image](https://user-images.githubusercontent.com/1626027/170872201-524d6d9a-57b7-42ce-a39f-0c95bd970ba7.png)

Notifications for Model Driven apps and more specifically Dynamics 365 has been released in mid 2021. And that was a very good news !
In facts, it is possible to send a notification to a user knowing his ID.

This solution adds something above the native feature, so that you can send notifications to teams and a list of users

## Solution content

This solution will add the following components in your environnement :

3 tables

- Target group
- Target group item
- Broadcast Messages

2 actions

- BroadcastNotification
- BroadcastMessage

In the sections below, we will describe the components listed above.

## Target Group

A tagert group, is a group of users. This group can be an team, a security group or a simple list of users. Depending on the field type.
In the case of a list, the user will have the possibility to choose the users to be added into the list.

## Target Group item

A target group item is a user (systemuser) to be added to the targer group, in the case of a list.

## Broadcast Message

A Broadcast Message, is a predefined message, that can be sent to a target group.
The broadcast messagehas this specificity that, the message is predefined and the targer is also predifined in to the record.
So you juste have to specify the message name and it will be sent to all targeted users.
