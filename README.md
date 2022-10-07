## AS a collaborator
If you’re a collaborator, go to the Github Repo page, Git Clone the project with the following command or simply cd into your work repository(Desktop) on your machine and paste the following command:
## $ git clone https://github.com/vincey101/admin_dashboard.git

then:
## $ cd admin_dashboard

### COLLABORATION
When you’re using git to work on the same project with multiple people, there’s one central rule you must follow:
## THE MASTER BRANCH SHOULD ALWAYS BE DEPLOYABLE
The way to keep Master deployable is to create new branches for new features and merge them into Master when they’re completed. Here’s how that works.

To start, branches should always represent features. For example, if you want to add the ability for a user to login you should probably create a branch called “user_auth” and in that branch you should only update what you need to to enable a user to login.

So let’s say you want to create the User model. In your terminal create a new branch:
## $ git co -b user_auth

You’re now in your new branch and can start coding away.

## Note: As a general rule, you should git add frequently and git commit when you finish something that allows your code to work (ends up being a couple times an hour). For example, when you finish a method and the code base works, git commit like so:
 ## $ git commit -m "Added function to allow Users sign in"

### Submitting Pull Requests

Your team spent all day and night working on their separate features in their various branches. They come back the next day with their completed features and want to merge them back into Master to be deployed.

Determining your Git Flow is a huge part of working in a team, but here’s one Git Flow you could adopt for now:

## Next, everyone git push their branches:
## $ git push

Now go to the Github Repo page. You should see the branch you pushed up in a yellow bar at the top of the page with a button to “Compare & pull request”.

Click “Compare & pull request”. 
This will take you to the “Open a pull request” page. From here, you should write a brief description of what you actually changed. And you should click the “Reviewers” tab and select whoever your team decided would be the “Merge Master”. When you’re done, click “Create pull request”.

## Rinse and Repeat
And that’s pretty much it! Keep adding new branches for new features and then coming together as a team to merge them into master. Keep master clean and deployable and don’t try to merge more than one branch at a time and you should be good to go.