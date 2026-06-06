Set Up GitHub Repository:

The first step in our CI journey is to set up a GitHub repository to store our Python application's source code.
Go to github.com and sign in to your account.
Click on the "+" button in the top-right corner and select "New repository."
Give your repository a name and an optional description.
Choose the appropriate visibility option based on your needs.
Initialize the repository with a README file.
Click on the "Create repository" button to create your new GitHub repository.


Create an AWS CodePipeline

In this step, we'll create an AWS CodePipeline to automate the continuous integration process for our Python application. AWS CodePipeline will orchestrate the flow of changes from our GitHub repository to the deployment of our application. Let's go ahead and set it up:

Go to the AWS Management Console and navigate to the AWS CodePipeline service.
Click on the "Create pipeline" button.
Provide a name for your pipeline and click on the "Next" button.
For the source stage, select "GitHub" as the source provider.
Connect your GitHub account to AWS CodePipeline and select your repository.
Choose the branch you want to use for your pipeline.
In the build stage, select "AWS CodeBuild" as the build provider.
Create a new CodeBuild project by clicking on the "Create project" button.
Configure the CodeBuild project with the necessary settings for your Python application, such as the build environment, build commands, and artifacts.
Save the CodeBuild project and go back to CodePipeline.
Continue configuring the pipeline stages, such as deploying your application using AWS Elastic Beanstalk or any other suitable deployment option.
Review the pipeline configuration and click on the "Create pipeline" button to create your AWS CodePipeline.
Awesome job! We now have our pipeline ready to roll. Let's move on to the next step to set up AWS CodeBuild.



Configure AWS CodeBuild

In this step, we'll configure AWS CodeBuild to build our Python application based on the specifications we define. CodeBuild will take care of building and packaging our application for deployment. Follow these steps:

In the AWS Management Console, navigate to the AWS CodeBuild service.
Click on the "Create build project" button.
Provide a name for your build project.
For the source provider, choose "AWS CodePipeline."
Select the pipeline you created in the previous step.
Configure the build environment, such as the operating system, runtime, and compute resources required for your Python application.
Specify the build commands, such as installing dependencies and running tests. Customize this based on your application's requirements.
Set up the artifacts configuration to generate the build output required for deployment.
Review the build project settings and click on the "Create build project" button to create your AWS CodeBuild project.
Fantastic! With AWS CodeBuild all set up, we're now ready to witness the magic of continuous integration in action.

<img width="944" height="440" alt="image" src="https://github.com/user-attachments/assets/defc2c6d-5530-4516-9fc9-970af00b93a1" />

<img width="932" height="360" alt="image" src="https://github.com/user-attachments/assets/0cadb42f-7e47-4f76-9216-8078fe5a0da1" />


<img width="944" height="440" alt="image" src="https://github.com/user-attachments/assets/da18bbf4-50c2-4ae3-b4ba-6a142a2299ec" />



<img width="949" height="386" alt="image" src="https://github.com/user-attachments/assets/c1a50ee5-9592-40b2-b8cf-73f8709609b1" />

<img width="959" height="146" alt="image" src="https://github.com/user-attachments/assets/d8b3b3b1-c9bf-46a4-8beb-ec6116ecc558" />
<img width="959" height="146" alt="image" src="https://github.com/user-attachments/assets/8b90cf5f-357b-44a8-ab22-62ab3b51792f" />


<img width="958" height="410" alt="image" src="https://github.com/user-attachments/assets/ef5d95bb-2f04-4a96-b8da-14fc29fe4ccb" />
