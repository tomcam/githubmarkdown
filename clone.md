# Clone the repository to your work machine

Now let's make a copy of the repository on your work machine.

## Install Git (and Xcode if you're an Apple developer)

* First, [install Git](https://help.github.com/articles/set-up-git/) if you haven't done so already.

On Macintosh systems, you may be required to download XCode if you haven't already. And before you download XCode, you need to create a free account with the Apple Developer Program.

* Follow those instructions and sign up as needed. 

Do not be distracted by what seems like a requirement to pay
for the account. That's only if you're going to list a product in the App Store.

* To ensure you have Git, open your terminal and enter `git` at the command line.

The result should be several pages of explanatory text looking something like this:

```
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
```

That shows you Git has been installed. If you see something like this, it means you don't have Git yet:

```
-bash: git: command not found
```

## Create a Git working directory

You need a place to work. Althought it's not necessary for you to think this way, I like to think
of my working directory as only being around for one session. That's because it reminds me that
my work is meant to be kept up to date on GitHub, not my local machine.

Suppose you're doing the documentation for something called MyAwesomeProduct. 

### Move to your home (or Documents) directory

* Go to your home directory (Using bash on Macintosh or Linux):

```
cd ~
```

OR

* Go to your home directory using Windows:

```
cd /d %USERPROFILE%
```

### Create the working directory

* Create a working directory (Using bash on Macintosh or Linux):

```
mkdir  ~/myawesomeproduct
```

OR

* Go to your home directory using Windows:

```
md %USERPROFILE%/myawesomeproduct
```

## Run git clone to make a local copy

You're going to run `git clone` from the terminal. That means a lot of typing to get the address of the repository correct.  GitHub makes it easy to construct the right command line by giving you the full path interactively and pasting it right
to our system's clipboard.

* Find the repository you're interested in, for example, `https://github.com/tomcam/deleteme`, and look for the big green `Clone or download` button on its home page:

![Green Clone or download button](images/github-clone-download-button.png)

There two ways to perform the download: Using `ssh` or using HTTPS. GitHub [recommends the latter](https://help.github.com/articles/which-remote-url-should-i-use/) for many reasons, including proper functioning from behind firewalls.

You'll probably see an option to use SSH:
![Green Clone or download button](images/clone-download-button-ssh.png)


clone-download-button-https

https://github.com/tomcam/deleteme.git

* Clone it like this:

```
git clone git@github.com:tomcam/deleteme.git
Cloning into 'deleteme'...
The authenticity of host 'github.com (192.30.253.113)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)? y 
Please type 'yes' or 'no': yes
Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
Permission denied (publickey).
fatal: Could not read from remote repository.
```

See [ssh](ssh.md) to learn how to create your 

Please make sure you have the correct access rights
and the repository exists.




