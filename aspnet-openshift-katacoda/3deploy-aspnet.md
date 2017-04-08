In this lab, you are going to deploy an ASP.NET application on OpenShift. If you don't have one already prepared, then use [this example one]. If you'd like to make your own ASP.NET application, then see [this blog series](https://blog.openshift.com/asp-net-on-openshift-getting-started-in-asp-net/) for a tutorial on getting started.

# Exercise: Deploying Your ASP.NET Image

Using the OpenShift web console, we're going to import a new ASP.NET Source-to-Image (S2I), so ensure you have the OpenShift web console open in the dashboard to the right, and that you are in the project called ``myproject``.

The OpenShift web console provides various options to deploy an application to a project. For this lab, we are going to use the **Import YAML/JSON** method. As we just created a project, the *Add to Project* view should be displayed. If not, the *Overview* page should display a prominent *Add to Project* button; otherwise you can also find an *Add to Project* button in the top menu bar for the project.

![Add to Project](https://blog.openshift.com/wp-content/uploads/OpenShift-Web-Console-0-300x177.png)

After selecting *Add to Project*, you should be presented with the options of *Browse Catalog*, *Deploy Image* and *Import YAML/JSON*. Choose the *Import YAML/JSON* tab.

![Add to Project Options](../../assets/intro-openshift/getting-started/3add-to-project-options.png)

Within the *Import YAML/JSON* tab, you can either upload or copy & paste the contents of a YAML/JSON file. We recommend that you use the following ASP.NET S2I:

https://raw.githubusercontent.com/redhat-developer/s2i-dotnetcore/master/dotnet_imagestreams.json

You can either download it from [this link](https://github.com/redhat-developer/s2i-dotnetcore/blob/master/dotnet_imagestreams.json), or copy & paste the contents of the raw file linked above. Click **Create**.

![Import S2I](https://blog.openshift.com/wp-content/uploads/OpenShift-Web-Console-3-300x268.png)

Once finished, you should see a "Creating resources in project..." message. Click on the **Add to Project** button below it. Now, it's time to upload your code.

![Add to Project](https://blog.openshift.com/wp-content/uploads/OpenShift-Web-Console-4-300x229.png)

**.NET** should now be an option in the Languages menu. Click on the dropdown and select the appropriate version. If you made your project in Visual Studio 2017 or Visual Studio Code, then you'll probably be using **1.1**. If you made your project in Visual Studio Community 2015 as I did with the example, then select **1.0**.

![Select .NET version](https://blog.openshift.com/wp-content/uploads/OpenShift-Web-Console-5-300x221.png)

You are ready to build and run your .NET application. Enter a name for it (it can be the same name as your project), and paste your a GitHub repository URL for your application here, then click **Create**.

You can now continue to the Overview.
