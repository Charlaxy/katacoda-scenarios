#### Manually Create a route

While waiting, go ahead and manually set up a route. Routes work by exposing an OpenShift services through an URL, giving a handy link to your page. One may be automatically crated, but it will go to a default ASP.NET path, such as /api/values. This isn't currently being used in the example app, and will just show a generic "value 1" and "value 2" if viewed. We'll need to make an additional route to a path being used in the application.

Navigate to **Applications > Routes** in the left sidebar.

Pick a **Name** for your route. This should be something that will be suitable for a URL, as this will be appended to your app's web address. Leave **Hostname** blank, and for **Path**, enter `/cat/bill` (one of the objects in the example). Select your app's name (the one that you picked when you added the build) from **Service** if it's not there by default, and the **Target Port** should be `8080`. Click **Create** when done.

Now, your new route will show up in **Overview**. Be patient, as it may take some time to finish deploying the project.

#### Check Your App Using the Terminal

At this point, you probably can't yet follow your route to check to see if your cat objects are there yet. Although everything is working with your app, you may still see a message like "Application not available" until everything is done.

This is fine! The message is ambiguous, but it doesn't indicate a problem. Your app should still be working behind the scenes. You can check to make sure by poking around in the terminal.

From the **Overview** page, you can click on "**1 pod**" (middle of the blue circle) and be taken to the Pods page. Click on the name of the pod, and then select the **Terminal** tab.

In the terminal, enter:

`curl http://localhost:8080/cat/bill`

You should get an answering `Meow!` if it's working. Soon after, following your **route** that you created should also work for displaying the same message in a browser window.

#### Congratulations!

The app should be working at this point! If not, you have learned some clues for troubleshooting.

Next, we'll go over some of the features that make OpenShift a nice choice for your future ASP.NET apps.
