An end-to-end application a Game with a Continuous Deployment Pipeline from GitHub to S3
Introduction:
Code for a game is hosted in GitHub. We create an S3 bucket for static website hosting, then create a continuous deployment pipeline (using AWS Code Pipeline) to automatically deploy the code whenever changes are made.
About the Game:
A simple memory matching game. The user clicks two cards (images of memes) to try to match them. If there's a match, the cards disappear from the board. If there's no match, the cards are flipped back to their blank side so the user can try again.
The game consists of HTML, CSS and JavaScript.
Ideas for additional features:
A scoring mechanism
A timer
Add additional cards
Multi-player capabilities so you can compare scores

Process to Create the Project:
Step 1. A high-level look at the pipeline we’re building
Step 2. How much will this cost me?
Step 3. Forking the GitHub repository to get the game code
Step 4. Creating and configuring an S3 bucket for static website hosting
Step 5. Creating a new pipeline in AWS CodePipeline
Step 6. Connecting to GitHub from CodePipeline
Step 7. Monitoring the progress of the source and deploy stages of CodePipeline
Step 8. Testing that the static website is working on S3
Step 9. Committing a code change in GitHub and triggering CodePipeline
Step 10. IMPORTANT!! Delete your resources!



Step1:A high-level look at the pipeline we’re building
Write or update your code. This is the first step in the pipeline. You can write your code locally or in a cloud-based repository like GitHub.
Check your code into a repository. This is where you store your code so that it can be tracked and shared with others.
Code pipeline runs the pipeline. This means that it will automatically build, test, and deploy your code.
Code pipeline builds your code. This means that it will compile your code into a format that can be run on a server.
Code pipeline runs your tests. This means that it will execute the tests that you have written to make sure your code is working correctly.
Code pipeline deploys your code. This means that it will push your code to the S3 bucket.
In the case of the pipeline that we are discussing, the code pipeline will not need to build or test the code because we are not writing any code. However, in the real world, you would need to build and test your code before deploying it.
