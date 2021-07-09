# LifeWorks Backend Developer Assessment

This assessment is designed to be simple and its primary aim is to assess how you approach and solve software 
development problems holistically. 
It contains only [three tasks](#tasks) which involve transforming user and company data.

Please be aware this isn't a test, and you will not be solely accepted or rejected based on your answers, 
but your answers may give us some idea about your code culture and technical capabilities.  
All candidates asked to complete the assessment will be invited to a technical interview where the assessment 
will be discussed along with their general technical knowledge and experience.

## How to Complete the Assessment

You will be advised by your recruitment contact which software language to complete this assessment in, 
but it will be either PHP, Python or Node JS.

Please clone this repository, complete the [tasks defined below](#tasks) and push the finished code to a private 
GitHub repository. Once this is done inform your relevant recruitment contact and we will advise on which GitHub users 
need access to review the assessment.

Please be aware the assessment should be completed 24 hours before your scheduled technical interview. If you have 
any issues with this please inform your relevant recruitment contact. 

### Completion Time 

We expect this assessment to take **2-4 hours** to complete dependent on experience. Please do not spend more 
than 4 hours on this assessment. We'd prefer you submit an assessment which is well done but half complete, 
rather than an assessment which is complete but poorly done.

You can complete this assessment in any way you see fit, but we expect you will have to complete the work in three 
basic steps:

- **Domain Warmup (30-60 mins)** consider the problem and gather information.
- **Environment Setup (30-60 mins)** create and configure your environment.
- **Task Completion (60-120 mins)** solve the individual tasks and push the code.

## Tips and Advice

Each of the tasks are relatively simple in that they represent common problems which have well documented solutions. 
So our main focus will not be assessing the specifics of how you solve each task.

To complete this assessment well you should consider carefully what steps you'd need to take to make this repo and code 
production and team ready. What features would the code and repo require so it can be safely pushed to production 
and another developer can easily edit and extend it.

## Tasks

The three tasks are based around user and company JSON data stored in the `./assets/user.json` 
and `./assets/company.json` files. Please review each collection of data before working on the tasks.

Be aware we do not care how you output the results of the data transformations, that is entirely up to you.

### Task 1

Transform the user collection so each record contains a new `full_name` field as shown in the example below.

```js
{
    "forename": "Jane",
    "surname": "Smith",
    "full_name": "Jane Smith",
    "date_of_birth": "2001/10/12",
    "location": "London",
    "company_id": 3
}
```

### Task 2

Transform the user collection so it only contains records where the user is 30 years in age or older.

### Task 3

Transform the user collection so each record contains a new `company` field which contains the company object 
and replaces the `company_id` field as shown in the example below.

This should be based on the relationship defined by the `company_id` field contained in the user collection 
and the `id` field contained in the company collection.

```js
{
    "forename": "Jane",
    "surname": "Smith",
    "date_of_birth": "2001/10/12",
    "location": "London",
    "company": {
        "id": 3,
        "name": "Solomon Sisters Bank",
        "headquarters": "London",
        "industry": "Finance"
    }
}
```
