📌 Project Objective :-
=
The main objective of this project is to automate the deployment of a web application hosted on GitHub to AWS Elastic Beanstalk using AWS CodePipeline. This ensures continuous integration and continuous delivery (CI/CD), improving deployment speed, reducing manual errors, and providing a scalable, highly available environment for the application.

📌 Project Description:-
=
This project sets up a CI/CD pipeline that automatically deploys a web application from a GitHub repository into AWS Elastic Beanstalk.

 Developers commit and push changes to GitHub.

 AWS CodePipeline detects the changes and triggers the pipeline.

 CodePipeline integrates with AWS CodeBuild (if build/testing is required).

 After build success, the updated application version is deployed to Elastic Beanstalk.

 Elastic Beanstalk manages the environment, scaling, and load balancing automatically.

This setup ensures seamless delivery of application updates with minimal downtime and provides developers with an automated workflow from code to deployment.

📌 Architecture Flow :-
=
Here’s the step-by-step flow of the architecture:

Developer Commit → A developer pushes code changes to GitHub repository.

Source Stage (CodePipeline) → CodePipeline automatically detects the commit (via GitHub webhook or polling).

Build Stage (Optional) → CodeBuild compiles, runs tests, and packages the application.

Deploy Stage (Elastic Beanstalk) → CodePipeline deploys the latest build to the Elastic Beanstalk environment.

Elastic Beanstalk Environment →

Manages EC2 instances, load balancer, auto-scaling group, and environment health.

Deploys the web application across multiple instances for high availability.

User Access → End-users access the web application via the Elastic Beanstalk environment’s endpoint.

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/1df10b1f-6d5e-4ba4-a9a5-3d1b0e2bc48b" />

📌 Benefits of This Setup:-
=

✅ Automation – Reduces manual deployment steps, ensuring faster releases.

✅ Continuous Delivery – Every commit automatically flows through testing and deployment.

✅ Scalability – Elastic Beanstalk automatically handles scaling up/down based on traffic.

✅ High Availability – Built-in load balancing and monitoring ensure the app is always accessible.

✅ Developer Productivity – Developers focus on coding; deployment is handled by pipeline.

✅ Integration with GitHub – Seamless sync between source code changes and deployment.

✅ Error Reduction – Automated testing & build steps minimize human mistakes.

✅ Cost Efficiency – Pay only for the resources used, no need for managing infrastructure manually.

