# Mensa App Würzburg

Some time ago, we came up with the idea that a homescreen widget for the canteen we usually go to while on University-Campus, that displays todays meals would be cool. The initial idea evolved into a bigger concept for a whole app, that can show you information about the cafeterias and canteens of the Studentenwerk Würzburg. Currently, the project is **still under development**.

> **!  Important Note:** This is no official application of the Studentenwerk Würzburg! We are just two computer-science students doing this for fun. :D


## Setup
Our apps are build on top of the Google Cloud Platform using Firebase.

Since the Studentenwerk offers no API, we wrote a fetcher (see Repository [Data-Fetcher](https://github.com/mensa-app-wuerzburg/Data-Fetcher), that retrieves the data from the website and stores them using Firestore (via Firebase Admin SDK). This fetcher runs as a Cloud Function three times a day to update the database. We then access the data on the client side using the Firebase SDK.

The iOS (maintened by @TimoReusch) and Android (maintained by @erikspall) versions are two standalone products written in Swift and Kotlin. Our goal is to offer roughly the same functionality on both plattforms, however, since we want to achieve a native look and feel on both operating systems, the apps differ a bit when it comes to structure and design. 

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
