# class 14

## Access Controls

as a i user sure you want to keep your data safe and not every one have the control of it but when you face problem and you want to have remotely solution you want another user to have access to your device here the access control concept come which is allow some user and deinie othe untel you give the permission for that user so he will be aloow to have access

## Application Flow and Access Control

if you are work on company you want to keep your data safe but you also want workers to work and some of them add data and some of them read data and of curse you want to have full access to yur work the type of access:

Allow admin users to create categories, content, manage user accounts, and run reports
Allow editor users to create, edit and delete existing content, but not see or manage user accounts
Allow guest users to access (read) content
Allow user users (logged in users) to access (read) content and apply a thumbs-up/down to content, but not change the actual content

to have this work done you need the back anf front end work as following

### Back End (API Layer)

Manage the login cycle with the front-end application
Maintain the User’s database
Maintain roles for each user
Authenticate users (basic and bearer)
Create, manage, and apply Role Based Access Controls
Maintain and reference their capabilities, based on their role
Restrict access to features (like routes) based on capabilities
Express Middleware could be used to restrict access to routes
Mongoose Middleware/Hooks could be use to restrict access to business logic

### Front End (Client Layer)

Initiate the login process
Store login tokens as cookies
Manage login state, capabilities
Control physical & visual access (hide/show/alter) to components based on RBAC rules
Alter behaviors based on RBAC rules