# to-do-list
**Overview**:
This is an API for a to-do-list web application. We have designed it using FastAPI framework in python language.
In our application, a user can register with his email and password, and then a user can do any CRUD operation on tasks by passing
"title" and "content" of the task when it's needed.

**Features**:
This API can register a user in the applicaation and then each user can create/read/update/delete any task he wants.
our API is able to return us the list of all tasks created by a user and also the number of tasks that each user has created.
For security measures, Each user is able to only read/update/delete his own tasks. but he can see the "number of tasks"
that other users have created.
We have used sqlalchemy as an ORM to talk to the Postgresql database. also we have made the use of "Pydantic" library to check
the validity of different requests in our API. it should be also noted that we have used JWT method for user authentication
and protecting desired API resources.


**How to Use**:
we can run the application using command below:
uvicorn app.main:app --reload

In this task, we used "requests" library to check the different endpoints, just to keep all things in one directory.
but any other application or platform could be used to do this, for example: Postman, Swagger UI, etc.
So, we can test different endpoints using files in app\requests directory. we have to just choose the endpoint we want to
send an HTTP request to, and comment out other endpoints, according to the comments explanations.
To use swagger UI, we can simply put URL below into our browser(defualt port is 8000):
127.0.0.1:port/docs
All environment variables have been defined in ".env" file.

**Requirements**:
All needed libraries and dependencies can be found and installed from requirements.txt file.
