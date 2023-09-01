# Devops challenges

Show off your skills with one of the challenges below, each estimated at roughly 2-3 hours if you’re already familiar with the subject, or less if you’re an expert.

## Challenge #1: Github actions

This task assumes basic skill with git and github actions and at least some familiarity with node.js.

1. Make sure you have [node.js](https://nodejs.org/en/download) installed.
2. Copy/clone the tiny `hello/` node.js project from this repo to your local computer.
3. Verify local project by running `npm i`, `npm start` and `npm test`.
4. Publish to a public github repo of your choice.
5. Make a github action script that runs on every push to remote repo. It should perform the following steps.
    - Install the package dependencies on the task runner using `npm i``.
    - Run test script using `npm test` and report failure if it returns anything but 0.
6. Make some trivial changes to the repo, e.g. increase the version number by running “npm version minor”. Commit+push and verify that the action reports success.
7. Change the test script in package.json to fail rather than succed. Commit+push and verify that the commit action reports the failure.
8. Send the link to us so we can view your repo. Don’t worry about your repo history. Just make sure the last two commits have one success and one failed action.

## Challenge #2: Cloud infrastructure deployment

This task assumes some basic skills for deploying cloud resources programmatically.

1. Make sure you have an account with one of the major cloud service providers that allows you to create basic resources for free. We currently use Microsoft Azure but pick the one you feel more comfortable with.
2. Make a script/program that will automatically create at least two different kinds of cloud resources, such as a VM, a web application, a storage account or anything that’s free on that platform. The deployment script may be a terraform app or a script in a language of your choice. It must take at least the following inputs:
    - Authentication. It’s okay to use `az login`` or similar, to manually pre-authenticate, but credentials must not be hardcoded in any way.
    - Subscription ID, tenant, or whatever term is used to describe how to deploy these resources into the control/custody of customers who insist on a deployment of our solution in their private cloud.
3. Prepare to demonstrate how the script/program works either by recording a video or showing us live in chat or in person. Ensure that things work flawlessly the first time.

## Challenge #3 Filesystem scripting

This task assumes some basic skills in scripting, json and archives.

1. Clone the `scripting` directory from this repo.
2. Make a script or program in the language of your choice to do the following:
    - Read and parse the `manifest.json` file.
    - Delete all the files in the directory that are NOT part of the manifest.
    - Move the files that are left into an archive file, like zip or tar.
3.	When the script is done there should just be two files left: `manifest.json` and whatever archive that contains the files listed therein.
4.	Send us the script file/program (with source code if compiled) for review.

