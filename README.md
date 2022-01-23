## Create-DotNet-Standard-Library
This repository contains information about creating .Net standard library to publish as NuGet package.

# How to create .Net Standard Library

1. Launch new instance of __Visual Studio__ > Click __Create a New Project__
![](images/1-create-new-proj.png)

2. Search for Class Library to select **.NET Standard Library**.
![](images/2-dotnet-standard-library.png)

3. Fill in the required fields > Set **Name** to **HelperLibrary** > **Solution** Name to **NuGetDemo** and Click **Next**
![](images/3-configure-new-project.png)

4. Select **.NET Core 3.1** as Target Framework and Click **Create**
![](images/4-dotnet-core-target-framework.png)

5. Once we click on **Create**, we are going to delete the Class1 that creates by default. **Right Click** (or press Del) to delete the class.
![](images/5-delete-default-class.png)

Now we will set the namespace for our project. You can leave the default value as it is but I'm going to change it to "**ACloudTechie.Artifact**" so it looks little bit different. It means, every class from now on will get the "**ACloudTechie.Artifact**" as a namespace.

1. Now, Right Click on Project (**HelperLibrary**) file and Select **Properties**.
![](images/6-project-properties.png)

7. Set Default namespace as **ACloudTechie.Artifact** and Click **Save**.
![](images/7-set-default-namespace.png)

8. Right Click on Project node and add new **Folder**. Set the name to **Calculate**
![](images/8-add-new-folder.png)
   
9. Add new **Class** as this will be very standard class library to demo something.
![](images/9-add-new-class.png)

10. Set Class name to **Calculate** and click on **Add**
![](images/10-class-calculate.png)

---
### Let's Start some coding 👨‍💻

This class will contain two super helpful methods. One method *adds two number* together and other *subtracts* one number from the other.

### Code Snippet

```dotnet
using System;
using System.Collections.Generic;
using System.Text;

namespace ACloudTechie.Artifact.Calculate
{
    public class Calculator
    {
        public static double Add(double numOne, double numTwo)
        {
            return numOne + numTwo;
        }

        public static double Subtract(double numOne, double numTwo)
        {
            return numOne - numTwo;
        }
    }
}
```

11. Now, foundation of our library has been setup.
![](images/11-foundation-calculate-library.png)

---

## Conclusion
In this post, we went through step-by-step to see how we can create a .Net Standard Library that can be used as a NuGet Package and publish to feed in [Azure Artifacts](https://acloudtechie.com/how-to-use-azure-pipelines-and-artifacts-for-package-management).

## Thank You
Thank you for reading!

Follow me for more content at https://acloudtechie.com
Let's Grow together! [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/bukotsunikki.svg?style=social&label=Follow%20%40zeeshanmcp12)](https://twitter.com/zeeshanmcp12)
