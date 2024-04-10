# CIS496 Git Activity
This repo contains an activity on all the basic git operations to give you some hands on practice.

Please reference the Week1 folder on this repo for some basic introduction: https://github.com/fmillion-mnsu/cs480-f23/blob/master/week1/README.md
Further explanation and context will be provided in this README. 

# Objectives
- To gain an understanding and practice with the following git commands...
  - fetch
  - commit
  - push
  - pull
  - revert
  - reset
- To practice branching, making pull requests, and merging
- To learn some best practices
- To learn about merge conflicts and how to resolve them

# Pre-Requisites
- A GitHub Account: https://github.com/
- Visual Studio Code installed: https://code.visualstudio.com/download
- GitHub Desktop installed: https://docs.github.com/en/desktop/installing-and-authenticating-to-github-desktop/installing-github-desktop
- Python installed (You can do this in VSCode under extensions if you don't already have it otherwise on Python's website)

# What is GitHub?
GitHub is a version control platform that allows developers to manage their code.

# Why should you care?
Without GitHub or any version control system it would be near impossible for people to collaborate on development projects in an effective manner. Code would have to be emailed back and forth whenever someone makes a change. If you have good experience with GitHub and can showcase that to your potential employers it will give you a good leg up.

# Part 1 - Branching & Commiting 
Now we will get into the sauce. 

**Step 0:** Fork this repository and name it `Activity1-firstname-lastname` but use your actual name.  

**Make sure you uncheck "Copy the `main` branch only".**  

You won't be able to proceed with the assignment if you don't.  

Learn more about Forks here: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo  

**Step 1:** Clone the repository using the nice little green code button and select "Open with GitHub Desktop"  
![image](https://github.com/Madeline-Ellingson/cis496-Activity/assets/93016306/664013d0-49d4-4ec7-adca-473f3960eb27)
![image](https://github.com/Madeline-Ellingson/cis496-Activity/assets/93016306/86432c47-9271-48e6-92f2-6ab583b13843)

You may get a popup saying to open GitHub desktop. Go ahead and click that and click clone. 

**Step 2:** Go ahead and switch into the `part1` branch and create a new branch off of it called..... `firstname_lastname_part1` but obviously replace `firstname` and `lastname` with your actual name. **This will count towards your grade!**
If you don't switch to the `part1` branch BEFORE creating your new branch it will have the wrong head branch and will not be counted. 

**Step 3:** Now that you have sucessfully created a branch go ahead and open up the branch in VSCode. You can easily do this by selecting the "Open in Visual Studio Code" option on GitHub Desktop or going to the Repository dropdown and open it from there.
You may not have VSCode as your default editor. If you don't see it as an option anywhere then go into the settings and switch it to your default editor. 

**Step 4:** Go ahead and create a new file `hello.py` and add a print statement to it that prints... "Hello my name is _________" but add your name instead. 

**Step 5:** If you saved the file you should now see it appear in GitHub Desktop. Go ahead and select that file and commit it. You will need to add a commit message in order to do so. 

**Best Practice:** It is good when working on any project to make smaller more reasonable commits. You don't want to commit a ton of files at once. Maybe 1 or 2 maximum unless they are tiny 1 line changes. This will also be a way to easily save your progress and make it more maneageble if you mess up and decide you need to revert a change.

It IS NOT good practice to commit directly into main. ALWAYS make a feature branch. Many many headaches are created from merging into main. Later on we will learn how to revert commits which will help in any instance that you do things you didn't intend. 

That is it for this part!

# Part 2 - Merging and Pull Requests
In this part we are going to practice merging and creating a nice neat and tidy pull request.

**Pull Request:** A pull request is a proposal to merge a set of changes from one branch into another  

**Step 1:** Switch to the `part2` branch and open er up in VSCode. 

**Step 2:** You should now see a lot more files in your repo. In order to be able to run this little pygame we first need to install all the required packages using the following command. 

`pip install -r requirements.txt`

If you don't have a terminal open then you can select the View dropdown and select Terminal or use ``Ctrl + ` ``

**Pro Tip:** If you have a python project where you have installed a bunch of packages you can generate a requirements.txt file using the following command.

`pip freeze > requirements.txt`

**Where I got this code:** https://github.com/dhhruv/Chrome-Dino-Runner

**Step 3:** Now we can run the Dino Game using the following command.

`python chromedino.py`

# Part 3 - Conflicts, Mistakes, Regrets
