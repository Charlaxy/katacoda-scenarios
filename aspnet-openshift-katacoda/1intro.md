#### Using ASP.NET in OpenShift

So, you want to try out ASP.NET on OpenShift? You'll see just how easy it is in the next few minutes.

This scenario was written specifically to introduce you to putting your ASP.NET project in OpenShift, and to go over some of the advantages of using OpenShift for ASP.NET.

If you are completely new to OpenShift, then please check out the [beginning OpenShift for developers scenario](https://openshift.katacoda.com/introduction/getting-started/).

#### Using OpenShift

This scenario will run an OpenShift cluster for you inside of Katacoda. If you'd like to try OpenShift outside of this scenario, then check out [OpenShift Online](http://openshift.com), and sign up for free. You can play around more with the tools that you'll be learning in this scenario. If you'd like to run OpenShift locally for further experimentation, then take a look at [OpenShift Origin](http://openshift.org).

If you're new to using ASP.NET and want to learn how to make the simple app that's used in this scenario, then check out my blog series on [Getting Started in ASP.NET on OpenShift](https://blog.openshift.com/asp-net-on-openshift-getting-started-in-asp-net/).

This scenario will work with the web console. However, OpenShift also has a CLI called [OpenShift Origin Tools](https://github.com/openshift/origin/releases/tag/v1.5.1), or OC Tools, that you can use through the terminal in Katacoda. You can also download it for your own use with OpenShift Origin or when running OpenShift locally.

#### Why OpenShift for .NET?

If you're looking at this scenario, you probably already know why you're using ASP.NET Core, such as how simple its [Razer syntax makes embedding C# code into your pages](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/razor).

What may be new to you is how good OpenShift is for your ASP.NET code. To explore that, we'll upload the project that's created for the Getting Started blogs ([found here](https://github.com/openshift-evangelists/MeowWorld) if you want to take a look at the code) and go over a few cool things that you can do with your project in OpenShift, such as vertical and horizontal scaling.
