# Intro
This project is an introduction to CI/CD using Github Action that will continually translate issues written in other languages into English.
# CI/CD
Continuous Integration/Continuous Deployment focuses on automating and streamlining the process of building, testing, and deploying applications. It allows development teams to continuously integrate code changes, automatically test them, and deploy updated versions of the application quickly and safely.

# GithubAccion
GitHub Actions is a tool that allows you to deploy CI/CD to GitHub repositories. <br>
GitHub Actions, provides a framework  to allow you to automate varios tasks, susch as :
- automate,
- build, 
- test, and 
- deployment pipeline or process.

Workflows are defined in the .github/workflows directory of a repository and can perform a different set of tasks.<br>
You can create workflows that build and test every pull request to the  repository, or deploy merged pull requests to production. 


More about GitHub Actions:
- Understanding GitHub Actions - GitHub Docs. https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions.
- Introduction to GitHub Actions - GeeksforGeeks. https://www.geeksforgeeks.org/introduction-to-github-actions/.


## What we need
1. event
2. job
3. step
4. action
5. runners
   
<br>

**Event** is an action that triggers a workflow. Example creating a change request, submitting a comment, or creating a tag.

**Job**, sequence of steps that are executed in parallel or series. This project only has one job and it is called **bluid**

**Runners** are the instances on which GitHub Actions workflows run. They can be virtual machines hosted by GitHub or physical or virtual machines configured by the user. Runners execute the steps defined in the workflows and provide the environment in which the actions are executed.

**Step** specific action that is performed as part of the workflow, such as building a project, running tests, or deploying an application in sequential order.

**Action** is a reusable component in GitHub Actions that encapsulates a set of steps and can be used in various workflows. This can be a [GitHub-provided action](https://github.com/marketplace?type=actions) or a user-defined custom action.<br><br>

This repository uses an action called ["Issues Translator"]( https://github.com/marketplace/actions/issues-translator). This action is responsible for translating the problems (issues) and associated comments into new languages.

## How to do it?

1. create a new repositorio.
2. create a folder called .github/workflows
3. create a file with the extension **.yml** inside and describe the [workflow](https://github.com/BeatrizBravo/githubAccion/blob/main/.github/workflows/issue-translator.yml).

### Hand on action to see the result:
1. Create a new issue from the tab called Issues.
2. go to the tab called Acctions to visualize the actions are happening in the repository.
Example: 
![alt Example that shows the result after each "issue" written in a language that is not English](https://github.com/BeatrizBravo/githubAccion/blob/main/issueBot.PNG)
![alt Example of actions"](https://github.com/BeatrizBravo/githubAccion/blob/main/actions.PNG)
