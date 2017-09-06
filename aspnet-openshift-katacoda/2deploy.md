#### Add to Project

Now that **.NET** is a language option, select that. Click on the dropdown and select the appropriate version. If you made your project in Visual Studio 2017 or Visual Studio Code, then you'll probably be using 1.1. If you made your project in Visual Studio Community 2015, then select 1.0. Go ahead and use **1.0** for the example.

![screenshot](/assets/catalog.png)
![screenshot](/assets/dotnet.png)

You are ready to build and run your .NET application. Enter a name for it, which will be used to label pieces created in your project. (It can be the same name as your project.) Paste a GitHub repository URL for your application here, then click **Create**. Here is the URL for the example project again: https://github.com/openshift-evangelists/MeowWorld

#### Deploying

You can now click **Continue to overview**, and watch in real time as your project is automatically built and deployed. You'll see an animated cycling icon and a message that says **Running**. You can click **View Log** to check out what's happening during this process. Click on **Overview** in the upper left menu to return to the original view.

If for some reason your app is not building and deploying automatically, you can click on the **Builds > Builds** button in the left-side menu, then your app name, and find the link to manually **Start Build** in the upper right. You can also check on the status of individual past builds here by clicking the build number in the list.

Similarly, you can do a manual deployment by visiting **Applications > Deployments** in the left-side menu, then selecting the app name, and then clicking the link to manually **Deploy** in the upper right.

This should not be necessary if your build is automatically working; however, feel free to poke around in this area while you wait on your app to get up and running, and see what information you can view about your build and deployment.
