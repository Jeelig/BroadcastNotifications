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

## Action : BroadcastNotification

Once you install the solution and create your target groups, you will be able to call the following action : BroadcastNotification.
When this action is called, the notification is sent to all the users belonging to the target group.

The action takes in two required parameters :
- target_group : GUID or Name of the target group
- body : Notification content

Other parameters are not mandaroty :

- id
- entityName
- viewId
- title
- body
- icontype
- data
- priority
- toasttype
- ttlinseconds

## Action : BroadcastMessage

Imagine you know exactly the message you want to send to the users Or want to be able to change it without changing you code.
With the BroadcastMessage, this is going to be possible.
All you have to do, is to create a BroadcastMessage, give it a unique "name", and set the target group.
The title and body of the notification are contained within the record. So that every time you send a BroadcastMessage, the notification is built from the record.
In that way, you don't need to edit you code in case you want to change the message that is displayed to the users.

The action takes in one required parameters :

- MessageName


## INSTALLATION

In order to install in your environnement, please download the latest release.

<a href="https://github.com/Jeelig/BroadcastNotifications/releases">Here !</a>

#Envoy
