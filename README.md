# Setting up c++ environment in VS Code for competitive Programming  on MacOS

## Step 1 :
 Make sure  you have homebrew installed in your machine . It's a package manager for MacOS. Then run the following command 

<br>

 <pre>brew install gcc</pre>a
 If you are facing error running this command then probably you don't have Xcode installed in your machine . So make sure you have installed Xcode in your machine .

 <br>

 ## Step 2 :


  Now open your Vs Code and add a extension named **Code Runner** . 

   <br>

## Step 3 :
  Now , open the folder where you want to create C++ files and create a c++ file .
Now press , <br>
**ctrl+alt+N** <br>
to run the c++ file and see the desired result . 
<br>

## Step 4
But still you can not use the **#include <bits/stdc++.h>** line because it will throw an error saying bits/stdc++.h not found . So, To resolve this ,

- Go to **Finder**
- then go to **Desktop**
- press **cmd+shift+G** . it will open a dialog named "Go to folder" . In this dialog type **/usr/local/include** .
- create a folder named **bits** and inside the folder create a file named **stdc++.h** . 
- in **stdc++.h** copy paste the code in this [link](https://raw.githubusercontent.com/gcc-mirror/gcc/master/libstdc%2B%2B-v3/include/precompiled/stdc%2B%2B.h)

Now that should be enough to avoid the mentioned error above 

## Step 5

Still your code can not take input from user . So , to resolve this ,

- Go to **Code** in top right corner and click it .
- then click **Preferences** . after that click **Settings** . 
- search **run in terminal** . Now scroll down and you will find a option **Code-runner: Run In Terminal** with a box which is not checked  . Check the box . make sure you are making the changes only for your current workspace rather than for all the projects . So between **User** and **Workspace** choose **Workspace**
