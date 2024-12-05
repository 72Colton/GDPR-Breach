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

Go to the Employee Service Center. The address for that is https://your-instance-name.service-now.com/esc.
![image](https://github.com/user-attachments/assets/f276c960-2086-4a62-91bb-fe3767eb919d)

Impersonate Billie Cowley:
![image](https://github.com/user-attachments/assets/45469698-edec-4d28-b679-3c9cf35bca5e)
![image](https://github.com/user-attachments/assets/095abcb6-5907-4d28-a9f7-0be546c01a57)

Search for GDPR and click on the result:
![image](https://github.com/user-attachments/assets/7258da01-9f4a-448c-aee6-ad21723a3279)

Submit a GDPR breach:
![image](https://github.com/user-attachments/assets/693f4a6f-841e-4276-8023-7e621188ef0c)

The record has been created:
![image](https://github.com/user-attachments/assets/3c326766-30c1-444e-a46d-e42ffad8dab1)

Billie receives an email:
![image](https://github.com/user-attachments/assets/6741cec1-c3dd-4413-9040-05a2532c7255)

Krystle, his manager, receives an approval request:
![image](https://github.com/user-attachments/assets/de1195ba-6823-4f8d-9000-e323683485c3)

Krystle "Approves" the request, remember to impersonate Krystle or log in as her:
![image](https://github.com/user-attachments/assets/8bec1af5-cf6b-46b1-85a6-9275ad5950ea)

Chris Harris (the CDO) receives notification of the possible breach and is prompted to review:
<img width="1454" alt="image" src="https://github.com/user-attachments/assets/8cbf1367-4116-4858-b337-7a50bd3658b4">

The link takes him to the Breach record. Remember to log in as Chris Harris:
![image](https://github.com/user-attachments/assets/965d95b8-7fb4-4258-83d2-0a298dca86a9)

Review the SLA (the clock is ticking):
![image](https://github.com/user-attachments/assets/b586856d-e0ac-4331-9504-29225459fe88)

His first task is to determine the validity of the breach and whether reporting is required:
![image](https://github.com/user-attachments/assets/03bd7ef9-89f9-43a4-b14c-283805587c9c)

After investigating, he determines that reporting is required so he updates the Breach record:
![image](https://github.com/user-attachments/assets/e376338b-931c-4f62-a0f7-3deb58418db1)

With this, he can now Complete the first task:
![image](https://github.com/user-attachments/assets/fae0985e-3b99-4985-b36c-6927c2fd7d0a)

A new Breach Task (Inform persons) has been created:
![image](https://github.com/user-attachments/assets/acab5db5-98a6-4b06-a1e4-ee8dffc48af2)

So he finds out who was involved in the data leak and informs them of the situation.
When he is done, he can "Complete Task" by clicking the button:
![image](https://github.com/user-attachments/assets/9149e905-5111-43c0-b4d8-26ab9178f956)

The parent record Breach is updated automatically:
![image](https://github.com/user-attachments/assets/3390fb2a-6e18-4cdc-9643-2ecab463af06)

He now has the last Breach Task to complete which is to report the breach to Datatilsynet (Datatilsynet is the Danish authority that handles GDPR violations, you may want or need to edit the app to fit your country).
![image](https://github.com/user-attachments/assets/295e8506-f096-484c-aeb4-3692519d8807)

![image](https://github.com/user-attachments/assets/b26da762-9b2e-4cf5-86bf-699e7c16797b)

The details of this task are beyond the scope of this demo as the demo is focusing on creating a structured workflow for ensuring GDPR compliance.

When he has done that, he can "Complete Task":
![image](https://github.com/user-attachments/assets/1fb7b3c4-0e1b-470b-b2e3-efde4803eb03)

This concludes the Breach handling and closes the Breach Record:
![image](https://github.com/user-attachments/assets/1e96cdc3-113c-4cd5-a502-80ca61fc4546)

And it ends the SLA timer as the tasks have been completed in due time and the company stayed compliant:
![image](https://github.com/user-attachments/assets/0eec61b9-06f0-46fb-9a2f-6259ad00737f)

Finally Billie receives an email:
<img width="1437" alt="image" src="https://github.com/user-attachments/assets/63856bc7-1718-4aa4-9b80-b1b940b2e15a">


The end.

Enjoy!




