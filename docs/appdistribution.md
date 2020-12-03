# Implementation of Firebase App Distribution in Android Development

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*2H2wzDBa6mzBaPN5DpcQ_g.jpeg)

Firebase App Distribution makes distributing your apps to trusted testers painless. By getting your apps onto testers’ devices quickly, you can get feedback early and often. And if you use Crashlytics in your apps, you’ll automatically get stability metrics for all your builds, so you know when you’re ready to ship.

> Firebase App Distribution is a beta release. This means that the functionality might change in backward-incompatible ways. A beta release is not subject to any SLA or deprecation policy and may receive limited or no support.

## Get Started

In this article, you will learn how to distribute your Android app to users/testers using Firebase App Distribution.
From the IOS background, they have been using test flight to distribute their apps to testers, it has really made it easy to test an IOS app and distribute it.
All Thanks to the Firebase Team to add this feature to Firebase, it's now easy to distribute Android apps to tester securely.

## Set Up Firebase App Distribution

**Step 1:** go to https://console.firebase.google.com/
Sign in to your dashboard and click App Distribution

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*vlzSIezBQLubi7msJQr_iw.png)

Click the check box to accept the Firebase Crashlytics and App Distribution Terms of Service.
Then Click **Get started**

**Step 2:** Drag an Apk or browse on your computer

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*3I70THkM-zrRqe-Ahzd-Qw.png)

in the **Release Tab**, you can drag an APK file to begin the upload process or you browse your PC to locate the saved location of you Signed APK.
In the **Invite links Tab**, you will be able to create an invite link for your tester.
In the **Tester & Groups Tab**, you will be able to create a group for each tester, see the list of testers in each group, and delete testers.
**Step 3:** Navigate to Tester & Groups Tab

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*iRhgFyub-T4z-1R8Bx7Ytg.png)

Create a group for your app testers, so click on “ Add group”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*wWspBgBdEQwVR7_kbsFRvw.png)

give your group a name and proceed

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*pgzbf2JeSYwPVJObclt4ag.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*9wBpVVwFDT7aU3mOY6hTwg.png)

The App Tester group is empty because it has no tester in it.
**Step 4:** Navigate to Invite Links Tab
Click on **“New invite link”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*4nF5-k3P76g61Ns3_WkQqA.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*rKDcjvvcAGZ90gT3blUH6w.png)

When you click on “New invite link” it will open this dialog box having your package name, a section to choose your tester group, and add restriction to the email domain.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*GGQRnfjdh1Yy4dftKK-QSA.png)

Click on “ Create Link” it will generate a dedicated link for your tester, you can now copy and share with your testers.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*bMsXc_gu0MDAJ4YUsv3zHg.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*0VLS6cjzDKf-6N-cd-FXcA.png)

when you try the links in your browser you will see the below screen

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*YjgOzcYo7mZFbHRHBlwfYA.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*jj01iNUTAQHmOaRU2opy2A.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*hgeCwWP2Bp_pZnJdGbKXAw.png)

**Step 5:** Upload a Signed APK

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*UMPvuT7-pHiFn56NS3RrAg.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*vg0YQIg-X3bn-COBhvr4bg.png)

Firstly, Click on “ Add testers or group ” to select the tester group you have created.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*boT-Zmo8EWAsViMCRVuvxw.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*WL9f2adQXuUt8b1VVxrnpw.png)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*Texr8fy4xcETywlzeqz4KQ.png)

At this point, you will have to refresh your browser so that the tester email you sent will reflect.
Then click on the “ Next” button to proceed to add release note.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*rY1Q4Z7iD9u5xR1pFqfJeA.png)

Click the “ Distribute to 1 tester”, the reason for having one tester is because only one tester has applied to test the project

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*qZo90Ks3G4aVZsnImnrzXw.png)

It has been sent to only one tester, the tester has not accepted it at the moment neither has he downloaded the app.
An invite email will be sent to the developer to accept and download for testing.

**Step 6:** Check your email address for an invite

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*MR6h4YIGGu4Xdpukg1dGmw.png)

Click on the “ Get setup” button
if you open it with your PC you will get the following message below

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*7GGj5P6tTzRN0qUDtxhsiQ.png)

**Step 7** Open the mail on an Android device

In this section, you will open the mail on an Android device and proceed

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*XkOgc1LH7Fzd_-uwbSeFUg.jpeg)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*Z0M_ZPR71nxi-t5GTA6SDA.jpeg)

Click the **“Allow”** button to proceed

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*I73Hd_iP6pe6aqf-MnoWdQ.jpeg)

Choose an email to sign in to Firebase using your mobile device

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*87p_YJr4gi1xgvYeuVPUAQ.jpeg)

Click the **“Sign in with Google”** and sign in with the email address you used in applying for App testing.

**Step 2:** Download Firebase App Tester

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*YqKMTDVjFYh9m3Ih8zy6yw.jpeg)

Click the check box to give Firebase consent and click the **“Accept Invitation”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*Ypau0fIXyQAE6G04z4wZBQ.jpeg)

Click the **Accept invitation** button it will take you to the screen where you can download Firebase App Tester to your Android device

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*KlwzmpNVk6w5FGCOf0rRPQ.jpeg)

Click the **Download** button to download the Firebase App Tester to your Android device

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*iL-qbgBLoF5tkqC9MBLUzA.jpeg)

Click **“OK”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*_7nAai6SqRh1I0ypMJk_mw.jpeg)

Check your notification for the downloaded app or search in the file explorer and locate the download folder. install it

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*grYUozyVGB9ldpCKYuA6mg.jpeg)

Click the **INSTALL BUTTON**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*rmEnYv5eIRBAh2PuRkh5aQ.jpeg)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*_nhDrqS5NwVUCaVPLNRDww.jpeg)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*Z0M_ZPR71nxi-t5GTA6SDA.jpeg)

Click the **Allow** button to accept the terms of service of the Firebase App Distribution

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1214/1*-EGzMYbgviTyN_UPHxla0w.jpeg)