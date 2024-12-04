ServiceNow GDPR Demo App (Creator Workflows / App Engine)

How to use this repo:

Fork or import this repo to your own Github account.

Go to App Engine Studio, select Import App:
![image](https://github.com/user-attachments/assets/abeb7163-2cf4-4e48-ac79-21b0522d546d)

Fill out the information about your own version of the GDPR-Breach repository. Credentials are mandatory and should be configured in "Credentials" in ServiceNow. The type is Basic Auth Credential, the username is your email address and the password is an API Key that you create in settings here on Github. It looks something like this: ghp_1234567890abcdefgHIJKLMNOPQRSTUVWXYZ.
![image](https://github.com/user-attachments/assets/fcecd5b2-b2fa-4940-875c-2ac8b101ff81)

Now you should have the App in your instance and you can select to Open App. It contains these components:
![image](https://github.com/user-attachments/assets/da4424a9-f26e-43ca-b95a-63c779bc9bad)

To make it work in your instance, you have to make a few adjustments:
1)  Open the GDPR Breach Reported email
    Click on the link in the email content that says ${number} and edit the link to your own instance name:
![image](https://github.com/user-attachments/assets/d1ae1409-40d6-4040-a4d1-ba01ced735dd)

2)  Edit the users who are personas in this demo context. Set their emails to your own email address and change their password to something you can remember. The personas are Billie Cowley, Krystle Stika and Chris Harris.
    You use filtering and inline editing to change the emails and passwords:
![image](https://github.com/user-attachments/assets/57879d45-d7de-40de-8512-014beea7ed31)

Now you should be good to go....

To try it out, first log into the Employee Service Center as Billie Cowley




