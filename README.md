# Create a Quiz app using AWS Amplify and Cognito (with CI/CD)
## Prerequisites
Ensure you have the following before starting:
AWS Account with necessary permissions
Node.js installed
GitHub account
AWS Amplify CLI installed
## steps to reproduce it
  I Followed this steps to achieve the the output. To do this Project we need to have following things
1.Setup Environment
2. Create React app
3.Add authentication with Cognito
4. Add Functionality and staying quiz
5 push local in Github
6  Host the front end in amplify via github(CI/CD)
7  Merge it works!

## command I used this handson
 1. npm install -g @aws-amplify/cli – Installs AWS Amplify CLI globally.
 2. amplify configure – Configures Amplify with AWS credentials.
 3. npx create-react-app <app-name> – Creates a new React app.
 4. cd <app-name> – Navigates into the app directory.
 5. amplify init – Initializes Amplify in the project.
 6. amplify add auth – Adds authentication (Cognito) to the app.
 7. amplify push – Deploys Amplify changes to AWS. After this step you can see the user pool is created in the aws conginto console
 8. npm install aws-amplify @aws-amplify/ui-react – Installs Amplify libraries for React. Run this command inside the project directory
 9. npm start – Runs the React app in development mode.it will start your application you can see login page
 10. Now i am using CICD pipeline to push this code to github and amplify will connect to github to do: git init – Initializes a Git repository.
 11. git add . – Stages all changes for commit.
 12. git commit -m "Initial commit" – Saves changes with a message.
 13. git branch -M main – Renames the main branch to "main."
 14. git remote add origin <repository URL> – Links the repo to GitHub.
 15. git push -u origin main – Pushes the project to GitHub.

After this, go to the AWS Amplify Console. You will see the app name that was created during step 8 (amplify init). Click on it and navigate to the "Deploy" section. Select "GitHub" as the deployment source and follow the configuration steps to connect your repository. Once connected, confirm the setup and start the deployment. After the deployment is complete, you will receive a subdomain link. Clicking on it will take you to your application's homepage.

