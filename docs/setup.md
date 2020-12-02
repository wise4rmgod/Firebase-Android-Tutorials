# Set-Up

In this tutorial, you will learn how to connect your Android project in Android studio to firebase so you can be able to integrate Firebase features like Authentication, Cloud Firestore, App distributions, Test Lab, Cloud storage, etc.

# Getting started
Follow the guide below to set up your project in Android studio
Goto Tools -> click you will see the dropdown in the image below then click on “Firebase”.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*wvdBgbfbApbNL86_.png)

It will open the image below, you will see all the Firebase packages available in Android Studio and select the one you want to work with.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*cGrb7RnIEjW7Vo3m.png)

It will open the below image, you have two important steps to follow
1: Connect your app to Firebase
2: Add Cloud Firestore to your app
NOTE: login your Gmail details in your Android Studio first before proceeding to the next step.
Click “Connect to Firebase”, it will open the firebase console in your browser

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*TVhf1enpng4LdWuF.png)

The below image is giving you two options
1: Create a new project
2: Continue with an existing project
In this part, you will select “Add project”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*m0WzhAAtChgU5Aht.png)

The image below will give you an option to change the name of the project, then click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*S-blDbQUw09IsDx_.png)

For the image below just click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*RIKiyayqPtjre9-1.png)

Tick the checkboxes in this part

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*SgmmjcaPz6uLrn2B.png)

Just click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*1wLiN4Ug0o9QGNnv.png)

It’s creating your project

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*pG3nYO00_-ubKSNQ.png)

your project is fully set up and ready for use, click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*xTu4XHPDVpvUvVet.png)

Firebase is setting up your project

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*p46MnGkYhzJrPoqh.png)

Now your project has been created in Firebase, click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*tUVN8tKrQuYAN3YS.png)

Now your Android Studio project is connected to Firebase

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/0*unDz-_aDpKf2Mw5x.png)

at this stage the project doesn’t support any Firebase package yet, you will need to configure it later.

# Add the Latest dependencies using Firebase BoM

Firebase Android BoM enables u to manage all ur Firebase library versions by specifying only one version — the BoM's version.
BoM automatically pulls in the individual library versions mapped to BoM's version. All the individual library versions will be compatible.

```
dependencies {
    // Import the BoM for the Firebase platform
    implementation platform('com.google.firebase:firebase-bom:26.1.0')

    // Declare the dependency for the Cloud Firestore library
    // When using the BoM, you don't specify versions in Firebase library dependencies
    implementation 'com.google.firebase:firebase-firestore-ktx'
}

```