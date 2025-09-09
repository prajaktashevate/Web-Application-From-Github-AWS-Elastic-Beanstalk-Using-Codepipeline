⚙️ Setup Guide
=

 Step 1. Prepare Your Application
=
Add your application code to this repository.
Ensure dependencies are listed (requirements.txt, package.json, or build file depending on language).

Step 2. Create Elastic Beanstalk Environment
   =
In the AWS Management Console, go to Elastic Beanstalk.
Create a new application and environment (ElasticBeanstalk-project-env).
Select the correct platform (Node.js, Python, Java, etc.).
Note the Web-deploy and Web-deploy-env.
<img width="1903" height="852" alt="image" src="https://github.com/user-attachments/assets/31b3d989-fcfb-4fd9-aa92-7b981dba1820" />

<img width="940" height="481" alt="image" src="https://github.com/user-attachments/assets/645ef050-430a-4a00-b61f-dace652c93ac" />

step 3. Configure IAM Role
=
Open **IAM Role ** in the console.
Create Role (EB-Codepipeline-Project ).
Add policies in the Role.
<img width="940" height="414" alt="image" src="https://github.com/user-attachments/assets/91f5b0ec-4ed1-403e-ad11-da7c239dc672" />

step 4. Configure CodePipeline
=
Open AWS CodePipeline in the console.
Create connection to github.
Create a new pipeline and give it a name.
Source Stage: Choose GitHub and connect to this repository.
Build Stage (Optional): You can add a build step with AWS CodeBuild if your app needs compiling or testing.
Deploy Stage: Choose Elastic Beanstalk and select your application and environment.
Save and create the pipeline.

<img width="940" height="293" alt="image" src="https://github.com/user-attachments/assets/11ed6b26-d508-4f16-8adf-130dbfbb0c96" />
<img width="940" height="525" alt="image" src="https://github.com/user-attachments/assets/5062efd4-4e50-449d-8cf9-5d8c5b78a61d" />
<img width="940" height="363" alt="image" src="https://github.com/user-attachments/assets/993f0e35-b8ba-4598-8cc4-344a852bbbaf" />
<img width="940" height="355" alt="image" src="https://github.com/user-attachments/assets/7737c762-e152-4e68-b222-6492a23524c5" />

step 5. Check final output
=
Refresh the page of Elastic Beanstalk.

<img width="940" height="446" alt="image" src="https://github.com/user-attachments/assets/564fc69b-8238-4f22-b2ea-99d5b057746c" />








