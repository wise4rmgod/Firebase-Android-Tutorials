#Implementation of Firebase In-App Messaging in Android development

 ![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*s5lUbq98byx1f-9u0kjRLA.jpeg)

Firebase In-App Messaging helps you engage your app’s active users by sending them targeted, contextual messages that encourage them to use key app features. For example, you could send an in-app message to get users to subscribe, watch a video, complete a level, or buy an item. You can customize messages as cards, banners, modals, or images, and set up triggers so that they appear exactly when they’d benefit your users most.

In this article, you will learn how to create an In-App Updater using a card that will notify your users to update their app and give them a button or text to click using Firebase In App Messaging in android development.
In-App messaging is a dream come true, do you know why? If you want to implement it on your own, you will have to write lots of code to achieve it, but you don't have to even write a single code 🥳🤯😳 to make it work using In-App Messaging.

###**Examples of In App messaging format(Card, Image)**
In this section, you will see how your messages are been shown to the users in a Card,banner,modal or image form below

###**Card Layout**
This display your message using a card that can contain an image, a text and a button too another fun part about it is that the button can trigger an action or just close the card.

 ![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*JSwCJj7TbuOf2izmNkzDQA.png)

###**Modal Layout**
This will display your message in a modal form having an “X” button to close the modal after reading the message, it can contain an image, a text and the x button to close it.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*DvJRXaEEQ9YfxKgWPVmUVw.png)

###**Image Only Layout**
This will just display the message using an image, it can contain an image and also have an x button that will enable the users to close it.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*P5vVQfrW6PsSSQ0-esf7VQ.png)

###**Top Banner Layout**
This will display the message at the top of the Android device, it can contain an image, a text? to close it just click any where on the screen it will close.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*vyRikPWbH9aVCYaIEhLykg.png)

###**Step by step guide to setup Firebase In-App Message**

Step 1: Connect Android project to Firebase

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1212/1*oCEzZHwNsZ0QN_HKwW7mCA.png)

Click on “Firebase” in the list and the below image will showup

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*zzU2yj8AtnOxwe8Tzkpy3A.png)

To connect your Android project to firebase in Android studio check this link: https://wise4rmgodadmob.medium.com/how-to-connect-your-android-studio-project-to-firebase-a5f5c4d67e87

###**Step 2:** Add Firebase In-App Messaging dependency

click on the **“Add Firebase In-App Messaging to you app”** button to add the dependency to your project as seen in the image below

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*NfiBlInkzleDYkkDDlBs4Q.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*JoIFqfJfPKrlkLmx5RcXKQ.png)

###**Step 3:** Create a campaigne in firebase console

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*xQksf1RJiZB_cpQ-DUzP2Q.png)

At this point, you will decide which of the layout will fit what you want to display to the users, for this article we want the users to click a button that will take them to a playstore where they will update the app. So, you will have to choose the “Card Layout” because with it you can add a button/Text with an action.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*B8151uQOYzi7a6bzYsZsVA.png)

Its time to modify the fields to suit your taste, you will have to add a **“message title”** , the **“body message”**, add an **“Image”** if you want to and also add the button with or without an action. you should notice that the phone image beside changes as you modify the fields.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*XkCg-H5oeXRcM5HUBD9kGg.png)

Click the **“Next”** button that will take you to the next screen

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*moyjut4ORTVRepJhb8Yi5g.png)

In this section, you will give your campaigne a name, a description and select the device you want to receive this campaigne and fill other fields too then click the **“Next”** button.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*6ey3-HSrmiSwaKgIryLemg.png)

In this section, you decide if you want the device to receive the campaigne immediately or schedule a date for that, secondly you will choose the event you want to take place before showing the campaigne and lastly, select per device frequency and click the **“Next”** button or click the **Review** button because the two other sections are optional.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*GOb0FXkkr0gUt4SwHgTGWA.png)

In this section, you will **“select conversion event”** and click on the **“Next”** button.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*MHU2eABiF4_0tuCl1vnHZg.png)

In this section, add a custom data key and value or leave it blank(this section is optional) then click **“Review”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*jY8c3NdGIYz4bR2LVU3DrA.png)

In this section, you can go over and modify them or proceed to click the publish button if everything looks okay and good.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*pz9jpZW_fl_ec01ma-u9Pg.png)

Then head over to your device, restart it and you will see the result 😍

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*NhMWhzxiZ4f3G7GGm-3WAw.png)

Viola you have it live on your device, at this point you can click on the Update button and it will take you to google play store to update the app.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*rRtrcsrJCh7Vn-ubi-N-Kg.png)

You don't need coding to set up Firebase In-App Messaging on Android studio.