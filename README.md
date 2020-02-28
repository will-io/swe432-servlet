[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
# A pretty Simple Servlet/JSP using Heroku

This tutorial will show you how to deploy a Heroku app that allows running Servlets and JSPs.

# Create GitHub and Heroku accounts

You can create accounts for free in both platforms (do not provide any payment info). Also, use your personal email so you can keep your accounts after you graduate:

## GitHub

Go to https://github.com/join: Use your personal email address (you can add your academic email later to access student benefits), provide your info and proceed, use the individual plan, and create your account.

## Heroku

Go to https://signup.heroku.com: Provide your info and proceed to create your account.

Optional: You can use GitHub student package found at https://www.heroku.com/github-students. 

# Create a Git repo(sitory) and and link it to a Heroku app 

If you have not install Git before, you can get it here: https://git-scm.com/downloads.

Now, follow these steps to bring this repo into your Github account:

## 1. Create an empty repo in your Github:

a. Go to github.com, login into your account, select the "repositories" tab, click on "New".

b. Once in the "Crew a new repository" page: give a name to your repo, make it private and let other options as is, and click on "create repository".

c. This will take you to your new repository's page, here copy the url to access your repo in the quick setup section.
It should look like this:

``` "https://github.com/<your_username>/<newly_created_repo_name>.git"```

## 2. Get this repo locally in your machine:

```
git clone https://github.com/luminaxster/swe432tomcat.git
```

## 3. Redirect the local repo to your own repo and save the changes:

Remember to replace the url template "https://github.com/<your_username>/<newly_created_repo_name>.git" with your repo's.

```
cd swe432
git init
git remote set-url origin "https://github.com/<your_username>/<newly_created_repo_name>.git"
git add .
git commit -m "Initial commit: cloned repo"
git push
```

## 4. Create a Heroku app

Go to https://dashboard.heroku.com/apps: click on "New" > "Create New App", provide a name to it, and click on "create app".

## 5. Link repo and deploy 

Once in your app's web page, select the "deploy" tab:

 a. set the deploy method to "Github",
 
 b. authorize Heroku to access your GitHub repositories,
 
 c. select the recently created one,
 
 d. click on "connect",
 
 e. activate automatic deploys,
 
 f. click on deploy the "master" branch (only this time so you can see the changes immediately),
 
 g. and finally, once your deploy is processed, click on "View".
 
## Updating your repo and redeploying

You only have to push your changes on your repo and they will cause a redeploy automatically.


## Follow the Original Guide
For more details about how to create a Tomcat setup from scratch, go to the Dev Center guide on how to [Create a Java Web Application using Embedded Tomcat](https://devcenter.heroku.com/articles/create-a-java-web-application-using-embedded-tomcat).

## Resources: 

https://kbroman.org/github_tutorial/pages/init.html  


