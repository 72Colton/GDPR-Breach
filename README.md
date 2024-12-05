ServiceNow GDPR Demo App (Creator Workflows / App Engine)

How to use this repo:

Fork or import this repo to your own Github account.
![image](https://github.com/user-attachments/assets/3877293b-f975-4639-a636-c291df16c3cf)

Create a Personal Access Token in Github by following the instructions here:
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens
![image](https://github.com/user-attachments/assets/dc02bccc-608c-48f1-b32a-c1d5f69a5880)

The token will look like this: ghp_1234567890abcdefgHIJKLMNOPQRSTUVWXYZ, copy the Token (for example to a textfile).

In your ServiceNow instance, create a Credential from the Connections and Credentials section.
![image](https://github.com/user-attachments/assets/61e1d4da-cbfb-4ea1-987a-418f78cce899)

Use your email address as username and the Github token as password:
![image](https://github.com/user-attachments/assets/05dd8fc2-56b0-4ebf-83f5-5754a6d19b02)



In your ServiceNow instance, go to App Engine Studio, select Import App:
![image](https://github.com/user-attachments/assets/72265c8e-37d2-4568-ba17-38ae7d80f7e9)

Fill out the URL from your own version of the GDPR-Breach repository, select the fork sn_instances/jaspercrwf and select your Github credentials. Then click "Import App".
![image](https://github.com/user-attachments/assets/d775e978-a15b-4323-87fe-5eadcd938015)


Now you should have the App in your instance and you can select to "Open Application". It contains these components:
![image](https://github.com/user-attachments/assets/4b493e8f-64b9-47c7-b95f-a0d9be21e775)

To make it work in your instance, you have to make a few adjustments to three users who are the personas in the demo. Navigate to System Security -> Users:
![image](https://github.com/user-attachments/assets/8fba6b8e-aa7d-414e-921c-0d69755744b4)

Find Billie Cowley, Krystle Stika and Chris Harris and use inline editing to change their emails to your own email:
![image](https://github.com/user-attachments/assets/2d8d26ba-ac87-482c-b810-8e48acb17b84)

Also change their passwords to something, you can remember:
![image](https://github.com/user-attachments/assets/e001cc9b-f781-4f3c-b2a1-c605a139ad9c)

Open Billie Cowley, click Roles and Edit:
![image](https://github.com/user-attachments/assets/481a9775-d3c8-46eb-bc59-4ea43ccf81ee)

Type *gdpr and assign the GDPR user role to Billie, then click Save:
![image](https://github.com/user-attachments/assets/0258b8ff-95ed-4ee8-bc16-bb97dfea9edc)

Do the same for Krystle Stika and Chris Harris and assign the GDPR Manager role to Krystle and the GDPR Admin role to Chris. Also assign the itil role to Chris.

To ensure your instance can send emails, go to Email Properties:
![image](https://github.com/user-attachments/assets/704ca8bd-6505-46e0-842d-288102af01aa)

Change application scope to Global:
![image](https://github.com/user-attachments/assets/fe1bc791-20f6-454c-a078-3d3639bba7d3)

Enable email sending, click Save:
![image](https://github.com/user-attachments/assets/120e09e8-4b63-4be1-9262-c42c52c96f40)


Now you are ready to try the app/demo:

Go to the Employee Service Center. The address for that https://<your-instance-name>.service-now.com/esc.
![image](https://github.com/user-attachments/assets/f276c960-2086-4a62-91bb-fe3767eb919d)

Impersonate Billie Cowley:
![image](https://github.com/user-attachments/assets/45469698-edec-4d28-b679-3c9cf35bca5e)
![image](https://github.com/user-attachments/assets/095abcb6-5907-4d28-a9f7-0be546c01a57)

Search for GDPR and click on the result:
![image](https://github.com/user-attachments/assets/7258da01-9f4a-448c-aee6-ad21723a3279)

Submit a GDPR breach:
![image](https://github.com/user-attachments/assets/15ff518f-e416-43d8-aedd-103699b1e493)

The record has been created:
![image](https://github.com/user-attachments/assets/a7e93bea-950e-4eea-bf64-00ac9193a372)




















Now you should be good to go....

To try it out, first log into the Employee Service Center as Billie Cowley




