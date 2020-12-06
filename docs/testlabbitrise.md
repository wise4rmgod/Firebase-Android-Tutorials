# Continuous Unit Testing in Android Development Using Bitrise

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*a7fnh0qKujgvkZQSD0tMeQ.png)

Unit tests are typically automated tests written and run by software developers to ensure that a section of an application (known as the “unit”) meets its design and behaves as intended.

In this tutorial, you will learn how about unit testing, its benefits, its types, unit testing tools, how to write a simple unit test in Android studio, and automating the testing processing using Bitrise.

## What is Unit Testing?
Unit Testing is a type of software testing where individual units or components of a software are tested. The purpose is to validate that each unit of the software code performs as expected. Unit Testing is done during the development (coding phase) of an application by the developers. Unit Tests isolate a section of code and verify its correctness. A unit may be an individual function, method, procedure, module, or object.

## Types of Unit Testing
In software engineering we have two types of unit testing which are:
- Manual
- Automated

## Benefits of Unit Testing?
- Unit testing will help the developer to fix/catch bugs early in the software development.
- It helps the developers to understand the codebase.
- unit-testing your project will help the developer structure the codebase and use an architecture
- you can test individual part of your code
- it saves time and cost in testing because you are using the JVM to run your test

## Unit Testing Tools
There are lots of free tools that will assist a developer to test his code, below are a few of them:

**Junit:** Unit is a unit testing framework for the Java programming language. JUnit has been important in the development of test-driven development and is one of a family of unit testing frameworks which is collectively known as xUnit that originated with SUnit. learn more https://junit.org/junit5/

**Robolectric:** Robolectric lets you run your tests on your workstation, or on your continuous integration environment in a regular JVM, without an emulator. learn more http://robolectric.org/

**Mockito:** Mockito is a mocking framework that tastes really good. It lets you write beautiful tests with a clean & simple API. learn more https://site.mockito.org/

**Truth:** Truth is a fluent and flexible open-source testing framework designed to make test assertions and failure messages more readable. learn more https://truth.dev/

**Hamcrest:** Hamcrest is a framework for writing matcher objects allowing ‘match’ rules to be defined declaratively. learn more http://hamcrest.org/JavaHamcrest/tutorial

## How to do Unit Testing

Let's follow the step by step guide below in creating your first Unit test:

**Step 1:** Add the necessary dependency for Truth/Hamcrest
but in this tutorial, we will make use of Truth

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*iYpnGrTHCQBA4CbAB2Iczw.png)

```

repositories {
  mavenCentral()
}
dependencies {
  testImplementation "com.google.truth:truth:1.1"
}

```

**Step 2:** Create a Unit test class

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*i9aXvBq9t1doegl--fkIIg.png)

**Step 3:** Write your Unit test

This entirely depends on what you want to test, if you check the image below you will see what I am trying to test for.
What I did was to create a function that does a specific task and returns a value, so I am checking for an “@” in the return value.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1332/1*KU3GOVz7uLBCeK5ptYksRQ.png)
![Welcome to jetpackcompose.com](https://miro.medium.com/max/670/1*5vowSFUHG8npjJ-VSvY8sA.png)


you will see I am getting a failed test because it didn't meet the requirement now lemme fix the bug by adding an “@” sign

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*iMvIST1IorOVFJk5xmv67g.png)

**Step 4:** Add the Firebase Android Unit Test Step

To add it, go to the dashboard -> Click on the App then select the project you want to automate the testing process.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*ML8wtq7ybX9H4B2W.png)

After selecting the app It will open the image below, then you Click on “Workflow”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*cR4zSiE6d7WUAfLA.png)

The image below will show

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*l93GThRCb5QHFykL.png)

Now to add a new Step, you will click on the plus sign in the Workflow

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*mhyHDuPdCjGL7vxJ.png)

When you click the plus sign you will see many Steps to choose from, but in this tutorial, you need to select a Firebase Android Unit Test Step.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*x6XaTztstYjsp_TB.png)

When you select the Firebase Android Unit Test Step the Image below will show.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*_CXGPiFacKOtYjTu3MvMWw.png)

> Make sure you have the Deploy to Bitrise.io Step in your Workflow, Once the build is finished, you will be able to view your test reports.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*1GjnIEjqQzn6qPT4.png)

Then click save(X+S) and push your new changes to your preferred source code management(Github, Gitlab, Bitbucket, etc)
After a successful Build goto your dashboard and click on the build.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*DrXvJgtsxc6jzS3P.png)

After clicking on the Build the below Image will open

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*nhhXU-7zz-s1kb9l6UYSEw.png)

To see your Android Unit Test report click on the **“Test reports”** button to get the below image.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*nVYOEdrmKKSvMUYJXkzk1A.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*a7fnh0qKujgvkZQSD0tMeQ.png)

Click on the “Test Case” button and the image below will show the test class names and duration

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*TE6Wnuv5EocCXnC3bzoDww.png)

That’s how easy it is to automate unit testing in Android development using Bitrise.