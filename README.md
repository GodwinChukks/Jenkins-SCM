## Jenkins Job

### In Jenkins, a job is a unit of work or a task that can be executed by the Jenkins automation server.

### A Jenkins job represents a specific task or set of tasks that needs to be performed as part of a build or deployment process. Jobs in Jenkins are created to automate the execution of various steps such as compiling code, running tests, packaging applications, and deploying them to servers. Each Jenkins job is configured with a series of build steps, post-build actions, and other settings that define how the job should be executed.

## Creating a Freestyle Project

### 1.  From the dasboard on the left side, click on new

![image](screenshot/1.PNG)

### 2. Creating a freestyle project with name  "my-first-job"

![image](screenshot/2.PNG)

## Connecting Jenkins To Our Source Code Management


### Now that we have created a freestyle project, let connect jenkins with github.

### 1. Create a new github repository called jenkins-scm with a README.md file

![image](screenshot/3.PNG)

### 2. Connecting jenkins to jenkins-scm repository by pasting the repository url in the area selected below, and ensuring  current branch is set to main

![image](screenshot/4.PNG)

![image](screenshot/5.PNG)

![image](screenshot/6.PNG)

### 3. Save configuration and run "build now" to connect jenkins to our repository

### Jenkins successfully connects to Github repository (Jenkins-SCM) and built freestyle job

![image](screenshot/7.PNG)


## Configuring Build Trigger

### As an engineer, we need to be able to automate things and make our work easier in possible ways. We have connected jenkins to jenkins-scm, but we cannot run a new build with clicking on Build Now. To eliminate this, we need to configure a build trigger to our jenkins job. With this, jenkins will run a new build anytime a change is made to our github repository

### 1. Clicking on "Configure" your job and add this configurations

![image](screenshot/8.PNG)

### 2. configuring build trigger to configure triggering the job from GitHub webhook

![image](screenshot/9.PNG)

### 3. Creating Github webhook

![image](screenshot/10.PNG)

### Github webhook configured

![image](screenshot/11.PNG)

### Successfully configured Github webhook

![image](screenshot/12.PNG)

### After change was made on the Github file and pushed to Github. A new build was triggered automatical

![image](screenshot/13.PNG)


