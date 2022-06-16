# Coding challenge

This coding challenge is designed to test your ability to break down a problem into smaller components, and craft a solution that is readable, maintainable and modular.

The task you have been assigned is to build a role manager - very similar to Github.

You can build full functionality like Github, but this is not expected. We expect you to complete Level 1. If you want to go the extra mile and really showcase your skills, then complete level 1 and level 2.

>If you really want to show off, then build level 3 and full functionality. This is overkill and we do not expect this for any applicants.

# The assignment
You are to build a role manager for projects. This role manager should have the following abilities.
1. CRUD projects, users (and groups)
2. Add users to a project with given role
3. (optional) Add users to a group
4. Add groups to a project (with a set role)

The logic should be almost identical to how github assigns users and groups to repositories. This functionality gives you a good solid frame of reference.

The following roles should be available for each user and group.
1. Owner
2. Admin
3. Manager
4. Employee

# Interacting with your solution
> When executing the program, a input should be expected which listens to the users commands. 

There are three levels for this task. 
1. A basic solution to add users to a project. This is acceptable to display your basic python skills.
2. Add group functionality and showcase your ability to design solutions to complicated problems.
3. If you want to go the extra mile, add the ability to unassign user and groups from projects, change roles e.t.c. Extend the softwares functionality to be fully functional in every way you can come up with. This will take a long time, so don't bother unless you really want to.

## Level 1
> Add the ability to create users and assign them to projects

**CRUD users**
```
user add elon       -> Add the user elon
user delete elon    -> Delete the user elon
user show elon      -> Show elon, his projects (and his groups)
user show           -> Show all user names
```

**CRUD projects**
```
project add model3    -> Add the project model3
project delete model3 -> Delete the project model3
project show model3   -> Show model3, its users (and groups)
project show          -> Show all project names
```

**Add users or groups to projects**
Assignment should follow the following format:
```
assign user <name> project <name> <role>
```
Some commands can look like this:
```
assign user elon project model3 owner
assign user musk project model3 employee
```

## Level 2
> Add additional functionality with groups

It should be possible to users to groups, and entire groups can be assigned to a project. This is the additional functionality for groups and assigning groups/users to projects.

**CRUD groups**
```
group add tesla     -> Add the group tesla 
group delete tesla  -> Delete the group tesla
group show tesla    -> Show tesla, its users and projects
group show          -> Show all group names
```

**Add users or groups to projects**
Assignment should follow the following format:
```
assign user|group <name> project|group <name> <?role>
```
Some commands can look like this:
```
assign user elon group tesla
assign user elon project model3 owner
assign group tesla project model3 employee
```

## Level 3
Add additional functionality to unassign, change roles e.t.c. How you do this is up to you. Please add documentation how to do this, if you decide to build additional functionality.

# Time for solution
We estimate that the time required to solve the assignment is the following:
|   Level  |   Estimated time |
| :------  |  :-------------- |
|   1      |    1-2 hours     |
|   2      |    3-4 hours     |
|   3      |    6-8 hours     |

We expect everyone to solve level 1. The additional levels are not mandatory, but optional if you want to showcase your skills more.

# What we will be looking at

We will be evaluating your solution in three categories:
1. Functionality - does your code work?
2. Maintainable - is your code easy to maintain and adjust
3. Readability - How do you name variables, comment code, use types e.t.c
