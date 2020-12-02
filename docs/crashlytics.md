# How to Integrate Firebase Crashlytics to Android project in Android studio

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*oXc49-L319DTt3LEXr-k_w.png)

Firebase Crashlytics is a lightweight, real-time crash reporter that helps you track, prioritize, and fix stability issues that erode your app quality. Crashlytics saves you troubleshooting time by intelligently grouping crashes and highlighting the circumstances that lead up to them.
In these tutorials, you will learn how to easily add Firebase Crashlytics to your Android project. Follow the guide below to start seeing crashes in your Firebase Crashlytics platform.

> To learn more about Firebase Crashlytics https://firebase.google.com/docs/crashlytics/get-started?platform=android

**Step 1:** Connect your app to Firebase
To connect your Android project to Firebase follow this link: https://wise4rmgodadmob.medium.com/how-to-connect-your-android-studio-project-to-firebase-a5f5c4d67e87
**Step 2:** Add Firebase Crashlytics SDK to your Project
Click on the button **“Add Firebase Crashlytics SDK to your app”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*P1F4kbyhDyRlWtsXp3YPVA.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*GGvaqXSzvHXoSyiq1-icbA.png)

Click on the “Accept Changes” to add it to your project
Now you can check your build.gradle to see the added dependencies

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*QbCcU-EP76m9AfNho80c1w.png)

After these, goto Firebase console

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*T-s2QatuoP4VkiVsl4WXCA.png)

Click “Crashlytics” in the menu it will show the image below

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*xAeONvwiHyOjn2P_g2aVLQ.png)

Then click the **“Enable Crashlytics”** button to enable it on your project.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*bQwO2o0ASvOlsCLGrqoaFQ.png)

Then cause a crash in your Android project to get the report on the Firebase Crashlytics dashboard

```
throw  RuntimeException("Test Crash")

```

Add the above to your main activity Oncreate method. you will see the crash below

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*Md_5ry7d1mdrk572l8DUYg.png)

Congratulations 😍😍😍😍😍❤️❤️❤️ you just added crashlytics to your android project.