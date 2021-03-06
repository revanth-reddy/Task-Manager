[![Build Status](https://travis-ci.com/revanth-reddy/Task-Manager.svg?branch=master)](https://travis-ci.com/revanth-reddy/Task-Manager)

## Prerequisites

After cloning the repo, install the dependencies present in requirements.txt file using the following command :

```
pip3 -r install requirements.txt
```
## Running the Application
I have used a virtual environment called **myvenv**. 
```
To activate virtual environment use following command in the homedirectory:

> source myvenv/bin/activate
```

There's already a database included in the repo ( db.sqlite3 ). So, there's no need of migrations. You can directly run the server using :
```
> python3 manage.py runserver
```

If you get any errors, probably your system is still using the default inbuilt python3.
You can use the below command which serves the same purpose as above :
```
> myvenv/bin/python3 manage.py runserver
```

## About the Application :

### Team Model : -
-   Any authenticated user can create any nunmber of teams and add other authenticated users to them
-   Only Team creator can edit Team details and its member.
-   Every Team creator is a member of that team also.
### Task Model : -
-   A Task is created in a team and Task creator can assign task to no user or other users.
-   If a single user tries to create Task then he is assigned to that task always.
-   Task creator **only** can update the task and other members of same team to which the task belongs can view it.
- Every Task has comments part, where Team members can comment.

###  Comments Model : -
-  Every Comment is associated to a task and has an author and creation date
- Comments creator a.k.a author **only** can edit or delete the comment.

##  Built With
- Python 3.6.7
- [Django](https://www.djangoproject.com/)  - The web framework used
- HTML, CSS, Js, jQuery
- [Bootstrap 4](https://getbootstrap.com/)  - Responsiveness reloaded
- Ajax
```
No third party apps used 😉
```

##  Additional Features are also added :
- Edit and Update a Team
- Edit Delete and Update a Task
- Edit Delete and Update a Comment
