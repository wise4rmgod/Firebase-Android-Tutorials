# Building a Joke App with Cloud Firestore using Kotlin 

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*rRs5kgidBosSGeRlv0LxvA.jpeg)

Cloud Firestore is a flexible, scalable database for mobile, web, and server development from Firebase and Google Cloud Platform.

**Note:** I will not be covering the benefits, capabilities, and features of Cloud Firestore, if you want to know more kindly visit this link: https://firebase.google.com/docs/firestore

In this tutorials, you will learn how to build a simple joke android app with Cloud Firestore using Kotlin in Android Studio. Just follow the simple steps and you will be a Cloud Firestore Expert

> This is part one of this article covering the integration of Cloud in your Android project

**Step 1:** Connect to Firebase Firestore

Goto Tools -> click you will see the dropdown in the image below then click on “Firebase”.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*vLm3iWOq3BVweOF3F1lWwA.png)

It will open the image below, you will all the Firebase packages available in Android Studio but you only need Firestore for these tutorials. so click on “Firestore”.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*RuPOkQORgVnpv4PF62twMQ.png)

It will open the below image, you have two important steps to follow
- Connect your app to Firebase
- Add Cloud Firestore to your app
**NOTE:** login your Gmail details in your Android Studio first before proceeding to the next step.
Click “Connect to Firebase”, it will open the firebase console in your browser

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*11jaPWyTekm2tcm_9Xv45Q.png)

The below image is giving you two options
- Create a new project
- Continue with an existing project
In this part, you will select “Add project”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*Lkvtx0aA1j0TKijoZUDQwQ.png)

The image below will give you an option to change the name of the project, then click **“Continue”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*DYKfNtCjogIBpU2FiBdSEw.png)

The image below just click “Continue”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*kK3KU_viQepC6pkNop2hnw.png)

Tick the checkboxes in this part

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*hgfJcNXxpOCPzCeJBpaE_Q.png)

Just click **“Continue”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*b41i5skgqUy8ZGWzdDZ32g.png)

It's creating your project

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*9JfmKc_LpUV-bxYiADoTvw.png)

your project is fully set up and ready for use, click **“Continue”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*DoQsMUnYJlOuITFJ3rVHdg.png)

Firebase is setting up your project

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*OX4jPgHxSiAiDgbokHqWvA.png)

Now your project has been created in Firebase, click **“Continue”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*YZXej8YO9KvGIWZAJZ5K0g.png)

Now your Android Studio project is connected to Firebase

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*MuSXxuLH03KDYScBHmi1SQ.png)

at this stage the project doesn't support Cloud Firestore yet, you will need to configure it.
Click your newly created project (JokeFirestoreExample)

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*2FAzmY7MHydrzpXbNyH8xQ.png)

Then click **“Cloud Firestore”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*d0AXeNCdgbypSFJF__ACNg.png)

Now click **“Create database”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*mYV0l6qRA3XQh5lrH3VScg.png)

Then select **“Start in test mode”**, the reason is that we are only testing it and not building for production.

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*M3syZpOW7ccgi3W1K9ooIw.png)

Click **“Enable”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*gvtmSQpiZBieIj6cpmv_PQ.png)

Your Cloud Firestore project is creating

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*XKxpD_mZH9D4ciOX9rzB8g.png)

you now have your Cloud Firestore database all setup

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*oaTMwzCviNkUL95G62XrRA.png)

Your project is ready to use the Cloud Firestore. you can see that your android studio project is connected, now click “ Add Cloud Firestore to your app”

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*X4R9jnrTyugpwoN-gZm0NA.png)

It will open the below Image, Click **“Accept Changes”**

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*jtw15_wo6k5jqdM4a04E5A.png)

Congratulation you have successfully configured your Android project with Cloud Firestore

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*mhFsJOxvo4-HXftOPFHTRw.png)

Now you are ready to send data and receive data from the Cloud Firestore database.

Follow the steps below to save and retrieve data from Cloud firestore

**Step 1:** Add the required dependencies and client libraries to your app.
```

implementation 'com.google.firebase:firebase-firestore-ktx:21.6.0'

```

**Step 2:** Initialize an instance of Cloud Firestore

```
val db = Firebase.firestore

```

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*V-RgUPCSQs8wlKDXpyrD8Q.png)

**Step 3:** Add data from android app to Cloud Firestore

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*TnT8PmzjxY_tbpmyqAsw5g.png)

```

val user = hashMapOf(
    "joke" to jokename,
)

db.collection("Jokes").add(user)
    .addOnSuccessListener {

        Toast.makeText(application, "Saved Successfully", Toast.LENGTH_SHORT).show()
    }
    .addOnFailureListener {
        Toast.makeText(application, "Not Successful", Toast.LENGTH_SHORT).show()
    }

```

**Step 4:** Retrieve data from Cloud Firestore

you will create a class with the field names that will correspond to the Cloud Firestore field names

Joke Model Class

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*nXakP-dMnmiTjmbmJ2wPRw.png)

```
class JokesModel(
    var joke: String? = null
)

```
![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*GgTPZ3t_GHaKsmNzyTXyQg.png)

```
db.collection("Jokes").addSnapshotListener  { snapshot, e ->

    val getjokes = ArrayList<JokesModel?>()

    for (document in snapshot!!){

            getjokes.add(
                JokesModel(
                    document.getString("joke")
                )
            )
            val ty = Adapter(getjokes, applicationContext)
            recy.adapter = ty
            ty.notifyDataSetChanged()

    }

```

Create an Adapter Class

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*6PxG18VyZKEj0L74nwuAkw.png)

```


class Adapter(
    private var dataList: ArrayList<JokesModel?>,
    private val context: Context
) :
    RecyclerView.Adapter<Adapter.ViewHolder>() {

    override fun onCreateViewHolder(parent: ViewGroup, viewType: Int): ViewHolder {
        return ViewHolder(
            LayoutInflater.from(context).inflate(
                R.layout.list_of_jokes,
                parent,
                false
            )
        )

    }

    override fun getItemCount(): Int {
        return dataList.size
    }

    override fun onBindViewHolder(holder: ViewHolder, position: Int) {
        val dataModel = dataList.get(position)
        holder.listj.text = dataModel?.joke

    }

    class ViewHolder(itemLayoutView: View) : RecyclerView.ViewHolder(itemLayoutView) {
        var listj: TextView = itemLayoutView.findViewById(R.id.listjoke)

    }


}



```

Finally, you can test your joke app now

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*s1VEDg9CMa6PfpzDQkLATw.png)

Cloud Firestore database

![Welcome to jetpackcompose.com](https://miro.medium.com/max/1400/1*qY4dqyzHC6NKLLrxaCGNoQ.png)

With Cloud Firestore you can build awesome projects not only for Android, but it also covers so many platforms like IOS, Web, Cross-platform( Flutter, React Native), and more.
Thanks for reading and I hope it will help you with your next project.
Github: https://github.com/wise4rmgod/JokeFirestoreExample