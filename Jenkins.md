CI (Continuous Integration)
CD- Continuous Delivery or Continuous Deployment


Workflow:
1. GitHub
Code changes are pushed

2. Jenkins
Detects the change and starts a job

3. Maven
Compiles code and runs configured build steps

4. Automated tests
Verify expected behaviour

5. Jenkins reports
Results, logs, errors and build status


Installation and configuration:
Component	Why Jenkins needs it
Java JDK-	Runs Jenkins and/or compiles your Java project. The JDK required depends on your Jenkins and project versions.
Git-	Allows Jenkins to retrieve source code from GitHub.
Maven- Builds Java projects and executes configured tests.
Plugins-	Add features such as Git integration, Pipeline jobs and test-result publishing.
Workspace-	The directory where Jenkins checks out code and runs build commands.

Freestyle jobs:
A Freestyle job is a Jenkins job configured mostly through the web interface. You specify the repository, build triggers, build commands and post-build actions.

Jenkinsfile:
A Jenkinsfile is a text file containing your pipeline definition. Instead of configuring every step separately in the Jenkins UI, you write the stages in code and store the file in source control alongside the project.
This approach is called Pipeline as Code. It makes the pipeline reviewable, reusable and version-controlled.

Git integration:
Git integration means Jenkins can retrieve code from a Git repository, build a particular revision and associate the results with that version of the code.
