# Implementation of sharing Android apps using Firebase App Distribution + Bitrise easily

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*QHtxermMtweBtORRkLxXDg.png)

Firebase App distribution makes it easy to share android apps easily and securely to testers, but many people will ask the question” how will I automate the process of building the APK and automatically the app will be sent to the testers email address, without going to firebase to upload the APK manually? that is where Bitrise comes to play.

> I will not explain how to set up Firebase App Distribution in this tutorial, you can check it out here

Bitrise automates the process for the developer using the Firebase App Distribution Step, which has fields where you can create a Test Group, Release Note, Release Note File, Testers, etc.
In this tutorial, I will show you the simple steps to integrate Firebase App distribution in Bitrise and how to share your APK easily with the testers through their email addresses from the Bitrise platform.

> I will assume you know the basics of how to set up a Bitrise Android pipeline if you don't, visit this link https://medium.com/swlh/setting-up-a-bitrise-ci-pipeline-for-android-2f9996095377

## What is Firebase App Distribution Step

Firebase App Distribution step in Bitrise lets you upload app binaries to Firebase, attach release notes and specify testers you’d like to notify through email.

## Set up Bitrise Pipeline for Android development
Setting up Bitrise pipeline for Android is very easy and simple to do, I have already written about that in another tutorial just check this https://medium.com/swlh/setting-up-a-bitrise-ci-pipeline-for-android-2f9996095377  then proceed to the next step

## Add Firebase App Distribution Step
To add it, goto dashboard -> Click on the App

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*a9sX9alzs01B4ZlUaKCQzg.png)

It will open the image below, then you Click on **“Workflow”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*KsGcOZS1HszrcFTPCSJI9A.png)

## What is Bitrise Workflow?

A Bitrise Workflow is a collection of Steps. When a build of an app is running, the Steps will be executed in the order that is defined in the Workflow.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*q8wpYWkGajb5QbxNiK-ATQ.png)

the “Git Clone Repository”, “Android Lint”, “Android build” are all Bitrise steps.

## What is a Bitrise Step?
A Step is a build task: for example, the Git Clone Step clones your Git repository at the start of a build, A Step contains the code that performs the build task.
Now to add a new Step, you will click on the plus sign in the Workflow

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*ttR1C4NwoL9PoB4UEd8i1w.png)

When you click the plus sign you will see many Steps to choose from, but in this tutorial, you need to select a Firebase App Distribution Step.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*UTxpQLVCnL7g6p7ttMz8vg.png)

You can see it's still in the BETA stage of development, so select the Firebase App Distributions.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*uiUUNYkM1l1id_3IkWpV6A.png)

The WorkFlow we have is looking good, but in this tutorial, we don't need some steps, let's remove the “ Do anything with Script step” and maintain the order of the step.

> these steps need to be before “Firebase App Distribution” please follow the order below.
1: Install missing Android SDK

2: Android Lint

3: Android Build

4: Firebase App Distribution

Click on the “Firebase App Distribution” step to configure it

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*_SSWh1J9jZNbEDCJWbQfzA.png)

There are three important things here
1: Firebase Token

2: App Path

3: Firebase App ID

## 1: Firebase Token
Install the Firebase CLI if you haven’t got it on your machine already.
```

// auto install script for Mac OS or Linux users> curl -sL firebase.tools | bash
```

To Use the CLI with CI systems login into the Firebase and get a token.
```
> firebase login:ci
```

Once the authentication process is completed, your token is printed out on the terminal. (Example token: 1/a1gqPSI3ryNcsDiZnCaHnY-hg9u9nJeosz3iNPe-S-RLdmqdypiJMOjoeOhOGsWK)
you will be taken to the Firebase dashboard to login with your preferred email address. then the below image shows you are good to go.