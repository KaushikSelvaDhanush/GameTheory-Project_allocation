# GameTheory-Project_allocation
This project is developed by 3 students who took up the course "Introduction to Game Theory" 2020

# Introduction

The “Introduction to Game Theory” course has attracted a large number of students. This high level of interest in the course makes it difficult to assign and manage project topics to all the students. Moreover, the current Covid-19 situation has not made things any easier. Each student taking this course needs to work in a team on a specific topic that is to be submitted for being graded. The topics are open, and students are given freedom to come up with their own topic to work on. The requirement of the course is to work in a team of 3-5 students on a topic. 

# Problem

The distribution of the topics to all the students was done by creating a google sheet. Where students can propose a topic of their own and try to gather students interested in their topic. Once number of students in a topic was between 3-5, they formed a group. If there is a team of 2 students who are interested in one topic, they would be forcefully be put in other random topic, which may or may not be there topic of preference. Thus, this will lead to formation of unstable groups.
Lack of communication with the fellow students made the matching problem complicated. A student was not able to make preference for the topics he/she wanted to work on. 

# Video
The video is an example of the 2 sided problem. It can be viewed in :https://app.animaker.com/video?e=ESX4K158OI927CL7

# In the Code
## Group Formation - Topic Preference

In this code an input file of the list of class students is given with top 3 preferences with the topic that they would like to work on. The code tries to form group with the top preferences. If this is not acheived then it checks for 2nd preference. Groups are tried to form by adding a student with second preference that can fulfil a Teamless of 2 students in their 1st preference. This is just an initial try and needs more work


## Splitting groups

There could be cases where the number of students in an internal group can be more than 4. This code is used to split students into teams of specific sizes. It suggests the number of students in each group and also number of groups to be formed.

It is the team formed when the more than 2 Topic Taker are part of a topic, but without the presence of TOPIC OWNER. This is similar to the 1 sided topic with topic preference. The group is formed randomly with respect to the number of students. The following method is used to determine the number of groups and number of students in each group.

Let the number of students interested in a topic be ‘n’. 

Let q be the quotient when n is divided by n and 

let r be remainder when n is divided by 4

The result is presented in the following table:


| Value of r        | Number of teams with 3 students           | Number of teams with 4 students  | Number of students with 5 students | Total Number of Teams |
| ------------- |:-------------:| :-----:|:-----:| :-----:| 
| r = 0  | 0 | q | 0 | q |
| r = 1  | 0 | q-1 | 1 | q |
| r = 2  | 2 | q-1 | 0 | q+1 |
| r = 3  | 1 | q | 0 | q+1 |
