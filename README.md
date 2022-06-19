# Setting up c++ environment in VS Code for competitive Programming  on MacOS

## Step 1 :
Install xcode and command line tools for xcode in your machine .

## Step 2 :

Install homebrew in your machine . It's a package manager for MacOS

## Step 3 :
Install gcc compiler using "homebrew"
 <pre>brew install gcc</pre>

## Step 4 :
Now open your Vs Code and add an extension named **Code Runner** . 

## Step 5 :
Now , open the folder where you want to create c++ files and then create a c++ file .
<br>
Now press ,
**ctrl+alt+N** <br>
to run the c++ file and see the desired result . 
<br>

## Step 6
But still you can not use the header **#include <bits/stdc++.h>** . Because this line will throw an error saying bits/stdc++.h not found . So, To resolve this ,

- Go to **Finder**
- then go to **Desktop**
- press **cmd+shift+G** . It will open a dialog named **Go to folder** . In this dialog type **/Library/Developer/CommandLineTools/usr/include/c++/v1** .
- create a folder **bits** and inside the folder create a file **stdc++.h** . 
- in **stdc++.h** copy paste the code from this [link](https://raw.githubusercontent.com/gcc-mirror/gcc/master/libstdc%2B%2B-v3/include/precompiled/stdc%2B%2B.h)

Now that should be enough to avoid the error we discusssed earlier .

## Step 7

Still your code can not take input from user . So , to resolve this ,

- Go to **Code** in top right corner and click it .
- then click **Preferences** . after that click **Settings** . 
- search **run in terminal** . Now scroll down and you will find a option **Code-runner: Run In Terminal** with a box which is not checked  . Check the box . make sure you are making the changes only for your current workspace rather than for all the projects . So between **User** and **Workspace** choose **Workspace**

<br><br>

## Extra : If you want to use a code snippet for your cpp environment

<br>

1 . Go to **Code** -> **Preferences** -> **Configure User Snippets** <br>
2. select **cpp.json** file <br>
3. copy paste the code from [file](snippet/cpp.json)

Now if you type **jagonmoy** and press **Enter** then the snippet will load . You can customize your snippet according to your need .