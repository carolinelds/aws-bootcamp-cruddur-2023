# Week 0 — Billing and Architecture

## 0 - Stakeholder Meeting

I took some notes while watching the [live stream](https://www.youtube.com/live/SG8blanhAOg?feature=share):

### 0.0 Project Scenario

I am responsible for the cloud infrasctructure of an application called Cruddr, which is an ephemeral microblogging website. The goal is to build an architecture around microservices considering the the 3 application layers: UI, Business Logic and Data Access. Also I should keep in mind the [Iron Triangle](https://www.mindtools.com/aa9j1zc/the-iron-triangle-of-project-management) concept when balancing cost, time and features. 

### 0.1 Involved people

Tony is my direct manager on the startup, we have the web development team working on our side, the investors - who mostly care about cost and timing - and our fractional CTO, with whom I can discuss about the technical requirements.


### 0.2 To do

I need to present a technical report for the investors detailing the proposed architecture, a budget and ongoing cost estimate.

## 1 - Homework Hard Assignments

### 2.0 Basic AWS Account configuration

I added MFA to my root account, then created a user group with AdministratorAccess policy attached. Then I added a new IAM user in this group to use along the bootcamp and added MFA to this user as well. 

### 2.1 Budget and billing

At first I had trouble configuring Billing and Budget access to my IAM user. Then I discovered that giving the permissions with policies is not enough: one also needs to [activate user access to Billing and Cost Management directly on root Account page](https://docs.aws.amazon.com/IAM/latest/UserGuide/tutorial_billing.html?icmpid=docs_iam_console#tutorial-billing-step1). And finally I discovered I did it "wrong", because Budget and Billing should ideally be kept on root account only, for security reasons. So I had to undo the previous permissions for my IAM user.

On my root account, I created two budgets: a zero spending budget to try to keep myself in free tier as much as possible, and a montly cost budget of U$ 5.00 to watch for my credits.


### 2.2 AWS CLI 

### 2.3 CloudShell

### 2.4 Conceptual architecture diagram 


## 2 - Homework Stretch Assignments

### 2.0 More AWS Account Configuration



