
### Introduction

<!-- Our articles have a specific structure. Learn more at https://do.co/style/structure -->
Node.js is a run-time enviroment that allows execution of Javascript outside the browser. It allows you to create automation scripts, build backend web applications and API's, etc. with Javascript. NPM is a JavaScript package manager commonly used for installing packages for Node.js.

In this article, you will learn how to install Node.js and NPM on Windows and verifying the installation.  You will then proceed to learn how to run Node.js code, update Node.js and also, how to uninstall Node.js.

When you're finished, you'll be able to create and run Node.js code on your computer.



## Prerequisites

To follow this tutorial successfully, you'll need the following:

- Internet access to download Node.js.
- A user with admin privileges to install software on Windows. 


## Step 1 — Download Node.js
Open your web browser and visit the [Node installation page](https://nodejs.org/en/download/]). Click on the **Windows Installer** button to download the latest version of Node.js. The installer comes with NPM and it is in 64 bit.

![node.js download page](/assets/images/posts/2020-02-08-template-literals/download-nodejs.jpg)

Next we are going run the Node.js installer

## Step 2 — Install Node.js and NPM
Once the installer has been download. Click on the file to run the installer.

### Node.js Setup Wizard
When the setup wizard dialog opens, click **Next**.

![node.js setup wizard](/assets/images/posts/2020-02-08-template-literals/node-setup.jpg)

### License Agreement
Review the license and then check on the "I accept the terms in the License Agreement" option and then click **Next**.

![license agreement](/assets/images/posts/2020-02-08-template-literals/license-agreement.jpg)

### Choose the Destination Folder

You will be prompted to choose the destination folder  to install Node.js. It is best to just leave the default location and click **Next**. 

![destination folder](/assets/images/posts/2020-02-08-template-literals/destination-folder.jpg)

### Custom Setup
****** COME BACK TO THIS********

Proceed with the default option and click "Next". unless there is a specific reason. Click **Next** to start the installation.


![Custom Setup](/assets/images/posts/2020-02-08-template-literals/custom-setup.jpg)

### Tools for Native Modules
In this step, it's safe to just go with default option and  click **Next** without modifying anything. You can check the option if you need the tools but I don't have a need for them yet. 

![Tools for native modules option](/assets/images/posts/2020-02-08-template-literals/native-tools.jpg)

### Begin Installation
The Node.js Setup Wizard is now ready to install Node.js and NPM. Click **Install** to begin the installation.

![Begin Installation](/assets/images/posts/2020-02-08-template-literals/begin-installation.jpg)

When the User Account Control security prompt pops up, make sure you click **Yes**.


### Finish Installation
After the installation is finished, click **Finish**.
![Finish installation](/assets/images/posts/2020-02-08-template-literals/finish-installation.jpg)


##  Step 2 — Verify Node.js and NPM installation
Let's verifying if the Node.js and NPM were successfully installed.

Open **Powershell** or *Windows Command Prompt* depending on your preferences. It's recommended to use Powershell since it has more features than the Windows Command Prompt. So we will use this in his guide. 

![Open Powershell](/assets/images/posts/2020-02-08-template-literals/search-powershell.jpg)

Once *Powershell* is opened, Enter the following:

```
node -v
```
This command checks the current version of Node installed.

We can check the NPM version installed.

```
npm -v
```

If Node and NPM is successfully installed, it should look the same way as this:

![Node works](/assets/images/posts/2020-02-08-template-literals/node-works.jpg)

Note: your version numbers don't need to match with the ones in the screenshot since you might be reading this article when a newer version of Node or NPM was released.

## Running Node.js Code on Windows
There are two ways to run Node.Js code:
- Node.js REPL  
- Cli executable

### Node.js REPL
REPL stands for Read-Evaluate-Print-Loops. It is a console, just like the browser console that allows you experiment with JavaScript code.

To access the REPL, type `node` in Powershell.

```
node
````
It will open a console you can play around with your JavaScript code.

```
PS C:\Users\<your username> node
Welcome to Node.js v12.15.0.
Type ".help" for more information.
> var name = "stanley";
undefined
> name
'stanley'
> console.log(name);
stanley
undefined
>
```

### Cli executable
This method is the one that is commonly used to run Node. You will write Node.js code in a file with an extension of `.js`.

We can see this clealy by writing our first "hello world" program.

Let's start by creating a folder in the home directory to store our program.

```
mkdir nodejs
```
`mkdir` is a command used for creating directories/folders.

Your output should look as below if you are using Powershell:
```
PS C:\Users\<your username> mkdir nodejs


    Directory: C:\Users\<your username>


Mode                LastWriteTime         Length Name
----                -------------         ------ ----
d-----         2/7/2020   3:12 AM                nodejs
```

Let's now get into the `nodejs` directory.
```
cd nodejs
```
Your prompt should now look like the following:
```
PS C:\Users\<your username>\nodejs>
```
This shows that you are in the `nodejs` directory.

Create a file `first-program.js` in editor of you choice and save it in the directory `nodejs`.

If you have Visual Studio code, you can easily create the file by typing `code first-program.js` which will open Visual Studio Code:
```
code first-program.js
```
Regardless of the option you chose, make sure you enter the following the file `first-program.js`.

```
var name = 'Stanley';

function sayHello(){
    console.log('hello', name);
}

sayHello();
```

Type the following to run the code in `first-program.js`:

```
node first-program.js
```

Your output should look like below.
```
PS C:\Users\<your username>\nodejs> node first-program.js
hello Stanley
```

I hope now you are confident to run Node.js code on your system.

We are not finished yet, let's look at how to update  Node.js and NPM.

## How to Update Node.js and NPM on Windows
To update Node.js and NPM, download the latest version of the Node.js installer on the [Node installation page](https://nodejs.org/en/download/] just we did in step 1 of this tutorial. The Node.js website always displays the latest version when it has been released. 

To update, download the latest installer and run it. It will replace your current Node.js and NPM.

## How to Uninstall Node.js and NPM on Windows
The process of uninstalling Node.js and NPM is the same as how you uninstall any other software in Windows.

On Windows 10, search `apps` and click **Apps & features**. 

![start menu](/assets/images/posts/2020-02-08-template-literals/start-menu.jpg)

When the **Apps & features** window open, search for Node and click it. When the popup dialog opens, click "Uninstall". This will start the **uninstall** wizard.

![start menu](/assets/images/posts/2020-02-08-template-literals/uninstall.jpg)
.

## Conclusion

In this article you learned how to install and update Node.js and NPM on Windows. Now you can run Node.js....

<!-- Speak  to reader benefits of this technique or procedure and optionally provide places for further exploration. -->



<!-- Some examples of how to mark up various things

This is _italics_ and this is **bold**.

Only use italics and bold for specific things. Learn more at https://do.co/style#bold-and-italics

This is `inline code`. Use it for referencing package names and commands.

Here's a command someone types in the Terminal:

```command
sudo nano /etc/nginx/sites-available/default
```

Here's a configuration file. The label on the first line lets you clearly state the file that's being shown or modified:

```nginx
[label /etc/nginx/sites-available/default]
server {
    listen 80 default_server;
    listen [::]:80 default_server ipv6only=on;

    root <^>/usr/share/nginx/html<^>;
    index index.html index.htm;

    server_name localhost;

    location / {
        try_files $uri $uri/ =404;
    }
}
```

Here's output from a command:

```
[secondary_label Output]
Could not connect to Redis at 127.0.0.1:6379: Connection refused
```

Learn about formatting commands and terminal output at https://do.co/style#code

Key presses should be written in ALLCAPS with in-line code formatting: `ENTER`.

Use a plus symbol (+) if keys need to be pressed simultaneously: `CTRL+C`.

This is a <^>variable<^>.

This is an `<^>in-line code variable<^>`

Learn more about how to use variables to highlight important items at https://do.co/style#variables

Use `<^>your_server_ip<^>` when referencing the IP of the server.  Use `111.111.111.111` and `222.222.222.222` if you need other IP addresses in examples.

Learn more about host names and domains at https://do.co/style#users-hostnames-and-domains

<$>[note]
**Note:** This is a note.
<$>

<$>[warning]
**Warning:** This is a warning.
<$>

Learn more about notes at https://do.co/style#notes-and-warnings

Screenshots should be in PNG format and hosted on imgur. Embed them in the article using the following format:

![Alt text for screen readers](/path/to/img.png)

Learn more about images at https://do.co/style#images-and-other-assets
-->