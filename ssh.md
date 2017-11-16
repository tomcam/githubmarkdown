

See [https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

## What "The authenticity of host 'github.com (192.30.253.113)' can't be established" means

Suppose you wish to clone a project from GitHub. You run this command:

```
git clone git@github.com:tomcam/deleteme.git
```

Then a bunch of text appears, and it doesn't look good:

```
Cloning into 'deleteme'...
The authenticity of host 'github.com (192.30.253.113)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no)? 
```

You should type `yes` (the full word).

```
Please type 'yes' or 'no': **yes**
```

This ominous-looking message appears:

```
Warning: Permanently added 'github.com,192.30.253.113' (RSA) to the list of known hosts.
Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```
