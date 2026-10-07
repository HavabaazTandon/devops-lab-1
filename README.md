# DevOps Lab 1 - Foundations & Continuous Integration

## Objective
To implement a basic DevOps workflow using Git, GitHub, and Jenkins for version control, continuous integration, and automated deployment.

## Tools Used
- Ubuntu 24.04 LTS
- Git
- GitHub
- Jenkins
- Java 21
- Visual Studio Code

## Project Files
- `app.sh` - Sample application shell script
- `Jenkinsfile` - Jenkins CI/CD pipeline configuration

## Git Workflow
The project demonstrates:
- Git repository initialization
- Staging and committing changes
- GitHub remote repository integration
- Feature branch creation
- Branch merging
- Pushing changes to GitHub
- Maintaining commit history

## CI/CD Pipeline
Jenkins retrieves the source code from this GitHub repository and executes an automated CI/CD pipeline.

The pipeline contains the following stages:

1. **Checkout SCM** - Retrieves source code from GitHub
2. **Build** - Makes the application executable and runs it
3. **Test** - Verifies that the application file exists
4. **Deploy** - Copies the application into the deployment directory
5. **Post Actions** - Reports pipeline success or failure

## Automated Build Trigger
Jenkins is configured using **Poll SCM** to periodically check the GitHub repository for changes.

Schedule:

`H/5 * * * *`

When a new change is detected, Jenkins automatically starts the pipeline.

## Pipeline Result
The Jenkins pipeline successfully completed all stages:

**Checkout SCM → Build → Test → Deploy → Post Actions**

Final Status: **SUCCESS**

## Branching
A `feature-update` branch was created to demonstrate the Git branching workflow. The changes were committed and successfully merged into the `main` branch.

## Conclusion
This lab demonstrates a complete foundational DevOps workflow using Git for version control, GitHub for remote source-code management, and Jenkins for Continuous Integration and automated deployment.
