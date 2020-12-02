# Test your Android App UI using Firebase TestLab easily

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*ryOMNAQb2slGr3MvrOh5Cg.jpeg)

Firebase Test Lab is a cloud-based app-testing infrastructure. With one operation, you can test your Android or iOS app across a wide variety of devices and device configurations, and see the results including logs, videos, and screenshots in the Firebase console.
In this article, you will learn how to test your Android apps on the Firebase Test Lab cloud platform. you will see how easy it is to test your app’s UI and also get quality feedback from the test-lab.

> Note: I assume you know how to walk around/navigate the Firebase platform, if you are new to Firebase please follow the below link to get started with Firebase
https://developers.google.com/learn/topics/firebase

## Steps to test your android app using Firebase Test Lab:

kindly follow the below steps to test your Android app.
**Step 1:** go to https://console.firebase.google.com/

Sign in to your dashboard and click Test lab

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*CaSpnexit-G2-o6gTC2mIw.png)

**Step 2:** Build a debug-app in Android studio and upload in the “ Android Robo Test”

Robo test is a testing tool that is integrated with the Firebase Test Lab. Robo test analyzes the structure of your app’s UI and then explores it methodically, automatically simulating user activities. Robo test captures log files, saves a series of annotated screenshots, and then creates a video from those screenshots to show you the simulated user operations that it performed. These logs, screenshots, and videos can help you to determine the root cause if your app crashes, and can also help you to find issues with your app’s UI.
for more about Robo Test https://firebase.google.com/docs/test-lab/android/robo-ux-test

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*QTfdQ4OMmG8sWOw5mnFIyQ.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*J7NtU53aolKIIcJAnopJwg.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*7pPOmP_CoG2OTNsP0FP4bA.png)

**Step 3:** Click on the Device that performed the test ( Pixel API Level 26 )

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*1vS8sSeFJqBbrEWJiB3MAA.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*XJZ00BxebmieAss1LYndSg.png)

From the above image, you can see the Test Passed and also the time it took the Firebase test Lab crawler to crawl your Android app UI, you can see the craw graph of your app, logs, screenshots, video, performance, and accessibility results.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*lwOj9nA-S5jwC3a27oLXkQ.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*LawyzYGzGfnTNAD5BpnGUw.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*sWYePLBEfXM01AreHySrAw.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*a-X6fvKfm1WDb157mipVCw.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*7Beee_or4edEY0dSF3T24A.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*vkodMUAJSz53oMpS1aEivg.png)

Thanks for taking the time to read my article and I hope it helps you optimize your next Android app.
I will advise you to always use Firebase Test Lab to test your app and watch how you will get the best feedback to improve your next Android /IOS app.