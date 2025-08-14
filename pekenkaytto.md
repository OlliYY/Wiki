---
title: 
description: 
published: true
date: 2025-08-14T09:02:31.487Z
tags: 
editor: markdown
dateCreated: 2025-08-14T08:35:59.343Z
---

## Introduction 

Peke is a Gitlab server maintained by Lapland UAS’s Frostbit software laboratory. Peke can be used by both students and the school's staff for software project management and version control in addition to enabling teamwork. 

 

## Creating a new project 

In order to use Gitlab’s features you must first create a project. A Gitlab project is often referred to as a repository. 

Create a new project by selecting the **“Projects”** tab. Then click on the **“New project”** button. 
![kuva1.png](/pekeohjesivukuvat/kuva1.png)![kuva2.png](/pekeohjesivukuvat/kuva2.png)

Now you should see a new window open where you can create a new project. For this example, we are going to create an empty project by clicking on the “**Create blank project**” button.

![kuva3.png](/pekeohjesivukuvat/kuva3.png)

![kuva5.png](/pekeohjesivukuvat/kuva5.png)



In this view you must give the project a name. After doing so select a namespace for your project. The namespace can be a group or your own username. 

![kuva4.png](/pekeohjesivukuvat/kuva4.png)

![kuva6.png](/pekeohjesivukuvat/kuva6.png)

Each project has three different visibility settings. 

A **private project** requires you to grant each member permission to access the project separately. If you selected a group for the namespace each member of that group gets access to the project automatically. Note that the group must exist before creating the repository in order for it to be selectable. 

In an **internal project** every logged in internal user has permission to access the project. External users do not have permission to access the project. An account can be separately marked as external. 

In a **public project** everyone has access to the project wether they are logged in or not. It is strongly recommended that you only select this option if you know what you’re doing. 

**Never share secrets (API keys, secret keys, passwords...) publicly! Failure to do so can lead to you losing access to the project or potentially an expensive bill!**

![kuva8.png](/pekeohjesivukuvat/kuva8.png)

After this you can create a “**README.md**” markdown file in the project root (**Initialize repository with a README**). Do so if you’re creating a completely new project and not adding already existing code to the project. 

Secondly you can choose if you want the code to be analyzed for vulnerabilities (**Enable Static Application Security Testing (SAST)**). 

Thirdly you can enable secret detection to scan the code for secret and credentials in order to prevent unauthorized access. 

After you’ve made your decisions, you can create the project by pressing the “**Create project**” button. 
![kuva9.png](/pekeohjesivukuvat/kuva9.png)

![kuva10.png](/pekeohjesivukuvat/kuva10.png)

## Inviting users to a private project 

Got to the project page select “Manage” and then “Members” on the left.

![kuva11.png](/pekeohjesivukuvat/kuva11.png)

**Invite Members** – button allows you to invite specific users to the project. 

**Invite a group** – button allows you to invite all users in a selected group to your project. 

**Import from a project** – button imports all users from another project. The users will have the same roles as in the original project.   

![kuva12.png](/pekeohjesivukuvat/kuva12.png)

If you chose to invite a specific user to your project, you can do so by entering their username or email address into the field as seen in the picture below. You should also give the invitee the proper role and set the expiration date of their access to the project if you feel it is necessary. 

You can read more about the privileges each role has here. 

![kuva13.png](/pekeohjesivukuvat/kuva13.png)

## Cloning projects 

Cloning a project means creating an identical copy of the project to your device. You can make changes to the cloned version of the project without said changes appearing in Gitlab. 

 

To clone a project folder to your device you must first go to the projects site and click on the “**Code**” button. After doing so you must choose if you want to copy the clone with **SSH** or **HTTPS**, if you aren’t sure which address to use pick **HTTPS**. After this you can complete the next step using either the command line (**CMD**) or Github Desktop (Link)[https://github.com/apps/desktop].

![kuva14.png](/pekeohjesivukuvat/kuva14.png)

### Command line 

[https://git-scm.com/downloads]

Ensure that git is installed before following the example. 

Start by opening command line in the folder you want the project to be stored in and run the following command: 

**git clone ‘projectaddress’** 

Replace **‘projectaddress’** with the HTTP or SSH address to your project.

![kuva15.png](/pekeohjesivukuvat/kuva15.png)

If you are cloning from Peke for the first time on your device, you will be asked for your credentials. Simply insert your Peke username and password into the corresponding fields.

![kuva16.png](/pekeohjesivukuvat/kuva16.png)

Note that it may take a moment to copy the project to your computer. 

If everything is successful, the cloned project should now be in the folder 	you specified earlier. 
![kuva17.png](/pekeohjesivukuvat/kuva17.png)

### GitHub Desktop 

[https://github.com/apps/desktop] 

Open GitHub Desktop and click on “**File**” and then “**Clone repository**”
![kuva18.png](/pekeohjesivukuvat/kuva18.png)

Since we are cloning from Peke go to the “**URL**” tab and insert the address you copied earlier. Now select the folder you want the project to be found in. You can either click on the “**Choose**” button or you can copy the path to the desired folder on the “**Local path**” field. Once you have done the required steps you can simply click on the "**Clone**” button.

![kuva19.png](/pekeohjesivukuvat/kuva19.png)

If you are cloning from Peke for the first time on your device you will be asked to login. Simply insert your Peke username and password into the corresponding fields

![kuva20.png](/pekeohjesivukuvat/kuva20.png)

If everything went successfully the project should now be found in the folder, you selected.

![kuva21.png](/pekeohjesivukuvat/kuva21.png)

![kuva22.png](/pekeohjesivukuvat/kuva22.png)

## Issues 

GitLab's Issues are essentially tasks, bug reports, feature requests, or any items that may need attention or action within a repository. 

### Creating an issue 

Go to the projects issue page and on the left side of the page select “Plan” and then “Issues”. Once that is done select “New Issue”

![kuva23.png](/pekeohjesivukuvat/kuva23.png)

![kuva24.png](/pekeohjesivukuvat/kuva24.png)

Now you must determine the type of issue and give it a title. 

You can also give it a description for more clarity about the task. 

You can choose who the task gets assigned to from the **Assignee** section. 

The **Labels** section allows you to give the issue labels to help with sorting. 

The **Milestone** section allows you to set the checkpoint within which the issue belongs. Note that the milestone must be set before creating the issue. 

The **Dates** section lets you set the timeframe for the issue. 

The **Contacts** section allows you to set the contact information of a specific person or group involved with the issue. 

The **confidentiality** tick allows you to limit the issue’s visibility to users with planner or above privileges.

![kuva25.png](/pekeohjesivukuvat/kuva25.png)
![kuva26.png](/pekeohjesivukuvat/kuva26.png)
Once the issue has been created it can be found on the **Plan/Issues** page.

![kuva27.png](/pekeohjesivukuvat/kuva27.png)

## Labels 

Labels allow you to categorize the project's tasks accordingly. Custom labels can be incredibly useful in making the Issues board fit the project. 

### Creating a label 

Go to the project’s page and on the left select “**Manage**” and the “**Labels**”. After this press the “**New label**” button. 
![kuva28.png](/pekeohjesivukuvat/kuva28.png)![kuva29.png](/pekeohjesivukuvat/kuva29.png)

Now you must set the title and if you wish, the description of the label. You should also set the color of the label to help in categorizing. Once you are done simply click on the “**Create label**" button.

![kuva30.png](/pekeohjesivukuvat/kuva30.png)

## Issue Board 

GitLab's Issue Board is a tool designed to help teams manage and track the progress of their work in an organized and collaborative way. It is essentially a kanban-style board that allows users to see, assign, and track issues within a project or repository. 

### Managing the issue board 

Go to the project page and on the left side of said page, click on the “**Plan button**” and then the “**Issue boards**” button.

![kuva31.png](/pekeohjesivukuvat/kuva31.png)
In the basic view you will see the open and closed columns. You can hide them by clicking on the gear icon on the right side of the screen. 

![kuva32.png](/pekeohjesivukuvat/kuva32.png)

In the menu that opens up you can hide the columns with the “**show open list**” and “**show closed list**” tics. You can also change the name of the board or delete it if you want. Save your changes by clicking on the "**Save changes**” button.

![kuva33.png](/pekeohjesivukuvat/kuva33.png)

Creating a new column 

Click on the “**New list**” button on the “**Issue boards**” page.

![kuva34.png](/pekeohjesivukuvat/kuva34.png)

Now select the label you wish to use and press the “**Add to board**” button.
![kuva35.png](/pekeohjesivukuvat/kuva35.png)![kuva36.png](/pekeohjesivukuvat/kuva36.png)
![kuva37.png](/pekeohjesivukuvat/kuva37.png)
When the new column is added you can move it by dragging and dropping. You can also change the order of the columns in the same manner. 

![kuva38.png](/pekeohjesivukuvat/kuva38.png)

Always remember to move the issues to their corresponding column. An example of this would be to move an issue from the “**TODO**” column to the “**Work In Progress**” column once it is started. This way the board stays up to date and following the project's progress becomes significantly easier. 

![kuva39.png](/pekeohjesivukuvat/kuva39.png)
