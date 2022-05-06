# **Lab Report 4; Week 6**
---

Hello, today I will be showing you the process that I used to implement the three Group Choice Options including:
* **Streamlining ssh Configuration (Short Username)**
* **Setting Up GitHUb Access from ieng6**
* **Copying Whole Directories Using `scp -r`**

---

## **CHAPTER 1:** Streamlining ssh Configuration (Short Username)

Setting up a custom alias or username will allow a user to login to their ieng6 account without having to type `ssh cs15lsp22zzz@ieng6.ucsd.edu`. The the custom alias, when combined with the ssh key makes logging in to the ieng6 servers so much easier, and a lot faster. **Lets get started.**

Assuming you have already set up the ssh key, open up the .ssh folder located on your personal computer onto Visual Studio Code.

![Image](./images4Lab3/opening%20.ssh.PNG)

Once open, you should have the following files in your folder:

![Image](./images4Lab3/files%20in%20.ssh.PNG)

Next, simply create a new file, make sure to call it `config`

once you have created the file, copy and paste the following lines

```
Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lsp22zzz (use your username)
```

You can change the `ieng6` after Host to whatever you want your login name to be. Here is how my file looks after I have made the changes. 

![Image](./images4Lab3/configFileIn.ssh.PNG)

And you are all set, now test it out in the terminal! Here is what a successful login should look like. 

![Image](./images4Lab3/aliasLogin.PNG)

Once you are in your account you can go about your day as normal, here is a screen shot of me copying a cool picture onto my ieng6 server account using my new login alias. 

![Image](./images4Lab3/pictureCopied.PNG)

As you can see after logging in and running the `ls` command the file I copied (drippychopper.PNG) is now there.

Here is the file in question: 

![Image](./images4Lab2/drippychopper.PNG)

Pretty cool huh?

---
## **CHAPTER 2:** * Setting Up GitHUb Access from ieng6


