#### Creating Your Project
To begin, click on the **Dashboard** tab in the console frame of this browser window. This will open the web console link in another tab or window of your browser.

You should see an **OpenShift Origin** window with **Username** and **Password** forms.

For this scenario, start by entering the following:

**Username:** `developer`

**Password:** `developer`

After logging in to the web console, you'll see a button labeled: **New Project**. Click this to get started.

You should now see a page for creating your first project in web console. Fill it in with the following:
>New project

>** *Name **

>`MeowWorld`

The rest is optional, but fill it in if it helps you.

After your project is created, you'll be taken to a screen where you can begin adding content to your project.

#### Deploying .NET Core S2I

The first thing that we'll need to add is the [.NET Core source-to-image (s2i)](https://raw.githubusercontent.com/redhat-developer/s2i-dotnetcore/master/dotnet_imagestreams.json). The quickest way to do that will be by navigating to the link, and copying all from the JSON file. Next, select the **Import YAML / JSON** tab, and paste the code from the JSON into the form. Click **Create**.

After you receive a message that says "Creating resources in project..." click **Add to Project** to return to the **Browse Catalog** view. Now, you should see .NET as an option. You're on your way!
