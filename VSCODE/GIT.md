# Using Git with VSCode
Microsoft Virtual Studio Code is a popular IDE used for programmers to create and compile code. It's one of the programs that any beginning coder will stumble upon or be directed to. It's easy to use, has a large community to support you, and is often found to be user friendly (in most cases). Personally, as someone who's very new to coding, I find it to be very helpful as it provides the ability work on code, tie in source control using Git (which is what these notes will cover), and find help when I need it due to its popularity. <br />

As someone who's new to GitHub who also uses windows, VSCode is an efficient way to dive into the world of coding. There's other tools out there that make jumping in easier however, VSCode is used by novices and professionals alike which makes it important to have as a foundation for IDE's. VSCode allows users to push and pull repositories while interfacing with GitHub. This allows you to work on projects straight in your IDE without ever having to pull up the web version of GitHub. For instance, in this project I created this repository and pulled it straight into VSCode to work on. When I'm finished, I can push it straight back into the repository without ever having to look at the web interface. <br />

Instead of using GitHub for Desktop I use GitBash. GitBash allows you to use GitHub in it's respective CLI capacity. If you're not a stranger to the BASH emulation environment, then GitBash might be good for you. Additionally, you could install Ubuntu for Desktop in the Windows store and use that. You could even generate your key-pair in the command prompt. Feel free to generate your keys however you feel comfortable with. As a fan of BASH, I chose the GitBash route. <br />

You can find the program here: https://gitforwindows.org/. Git for Windows provides a BASH emulation used to run Git from the command line. *NIX users should feel right at home, as the BASH emulation behaves just like the "git" command in LINUX and UNIX environments. I'm sure there's other ways to do the exact same thing but, this is how I've learned to do it. You can find a descriptive tutorial on how to install GitBash here: https://www.toolsqa.com/git/install-git-on-windows/. <br />

So, we have our BASH, ideas, and IDE. How do we start working? <br /> 

The first step to working on your project is generating an SSH key-pair in order to remotely connect to your repository. <br /> 

# Where'd I put my keys again?
Thankfully, GitHub has already provided a step by step process for Mac/Windows/Linux users located here: https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent.

Windows (GitBash, Command prompt, etc.) <br />

$ ssh-keygen -t rsa -b 4096 -C "my_email@example.com" <br />
The output will look like this: <br />
Generating public/private rsa key pair. <br />
Enter file in which to save the key (/c/Users/JohnDoe/.ssh/id_rsa): <br />

Pay close attention to where you're putting your keys so you can copy and paste them later. Enter a password for your key and you're good to go! <br />

At this point, login to your GitHub account and head to your profile settings. You'll see a tab labeled 'SSH and GPG Keys'. Click on that tab and you'll be able to view a list of your keys. Click 'New SSH Key' and find your public key file (DO NOT USE YOUR PRIVATE KEY). It'll be the file with the .pub file extension. Copy and paste the entire key into the box provided and give it a name. Now, you're ready to go. <br />

# Creating a Repository
https://help.github.com/en/github/getting-started-with-github/create-a-repo <br />
The link above is the instruction page on how to create a repository. If you don't want to visit it, I'll list how it's done here. I'll explain how to do it the web route and locally in VSCode. <br />

GitHub (Web Route) <br />
- Head over to your account and click on the Repositories tab. <br />
- In the top right-hand corner you'll see a button that says 'new' (https://github.com/new) <br />
- Now you can fill in the desired information about your project. You can make your project public or private. You also have the ability to initialize your project with a README. This is a great way to let people know what your project is about. Many programmers and coders use this file to demonstrate how to use the program or how to install it. <br />
- In case you're wondering what the add .gitignore option is: gitignore files specify intentionally untracked files that Git should ignore. Files already tracked by git are not affected. For example, if you have files and folders you don't want to share on git, .gitignore files allow you to block that file (or extension) from being accessed. You can read more about it here: https://git-scm.com/docs/gitignore. <br />
- You can also add licenses to add trademark, copyright, and patents to your repository. To do that, you can select what license you want in the drop down box or if you don't know what those do, you can click the small info button next to the drop down. You'll be taken to https://choosealicense.com/ where you can pick a license based off of the scope of your project. You can copy and paste the license and add it to a LICENSE file in your repo (no file extension). Youtuber Thomas Bradley, has an excellent explanation video on how to write README files and what license files do. You can watch that here: https://www.youtube.com/watch?v=RZ5vduluea4. <br />

# Cloning a Repository
1.	Get the URL for the desired repository <br />
2.	Open VSCode <br />
3.	Press F1 <br />
4.	Type Git: Clone and hit enter <br />
5.	You will then be prompted to add the URL; copy, and paste the URL when prompted <br />
6.	Save the file to your desired location (I have a folder dedicated to coding projects and information <br />
7.	VSCode will then ask if you want to open the source repo, select “Open” <br />
8.	You will then see your repo! <br />
 
