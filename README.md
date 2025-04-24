Problem: 
We need to develop a Web API application that maintains information about different students and courses in a relational database.
Following is the list of API Endpoints that we need to implement in this application:
1. Add a Student [Name, Email, Phone]
2. Assign a Student to one or more Courses
3. List Students [Name, Email, Phone, Course Enrolled (comma separated string)]
4. Create a Login API with any authentication mode. Unless the user hits this API first, others should
not be accessible, giving a 401 UnAuthorized Access response.

Solution:

Database script : to Create Database and Required Tables for the Assignment
![image](https://github.com/user-attachments/assets/23143942-2142-4aef-8007-5e3d345ba8f7)


Initially tables are empty:

![image](https://github.com/user-attachments/assets/765a5505-06ee-4a28-bcf4-ae300c078099)


After running the web application swagger endpoint is shown:

![image](https://github.com/user-attachments/assets/4b0c1ab2-8f64-44bb-9422-e19ca4205e02)


Login Functionality:

Create a Login API with any authentication mode.
Use this endpoint to generate jwt token for authorization.
Default username and password is as per the request body below:

UserName: nikita
Password: test@123

![image](https://github.com/user-attachments/assets/2075f272-23ba-4949-9f5a-2c7e81957e2a)


Unless the user hits this API first, others should not be accessible, giving a 401 Unauthorized Access response.

![image](https://github.com/user-attachments/assets/ad8311f6-f8f5-4000-b167-84b0db242945)


After the login : copy token and paste in the Auth header of request,
It returned the empty list since there is not data into DB.

![image](https://github.com/user-attachments/assets/98807da0-a9d5-4a29-bf09-790a41f7ac61)


Add a Student [Name, Email, Phone]

![image](https://github.com/user-attachments/assets/f0109264-f78b-4d8a-a6f7-8926384a55a3)


Verify in DB:

![image](https://github.com/user-attachments/assets/881e6924-f068-402e-82e8-b2f3002d8a1d)


Add course data manually in database. 

 ![image](https://github.com/user-attachments/assets/28a7e1f6-ef05-4a9f-a3d5-6f67de51630b)


Assign a Student to one or more Courses

![image](https://github.com/user-attachments/assets/d4250090-a175-4266-ab46-6b3475d47a01)

![image](https://github.com/user-attachments/assets/9f7a8056-7b7a-40a6-9828-91945e0fd820)

![image](https://github.com/user-attachments/assets/adccdfc5-40d1-4955-ba32-a248c6cae94f)

![image](https://github.com/user-attachments/assets/26dd3c5f-ebbb-4428-a5de-33c9e67db82f)



List Students [Name, Email, Phone, Course Enrolled (comma separated string)]

![image](https://github.com/user-attachments/assets/956abce6-dc25-4c68-bd76-6e9be21033f3)


