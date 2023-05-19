# **My Notes**

![Banner](./banner.png)

<hr>

## Generating SSH keys

```sh
ssh-keygen
# press enter, enter ...
```

> **NOTE:** 
> `id_rsa` (private key), `ida_rsa.pub` (public key)

After this: 
* Go to the github settings page.
* Navigate through **SSH and GPG keys** section.
* Click `Add new SSH key` (or like) button.
* Then paste contents of `ida_rsa.pub` file.

> **NOTE:** 
> You can get it by `cat ~/.ssh/id_rsa.pub`

* Then save, and clone your repositories.

## Cloning git repo

```sh
git clone username/repository
# via SSH
git clone git@github.com:sanjarzayniev/git-demo.git
```

## Useful Git Commands

See what files added/modified and deleted.
```sh
git status 
```

Add changes, e.g You created file named `main.cpp` and you wanna add it.

```sh
git add main.cpp
```

Or you made some changes on `README.md`, and you wanna update it.

```sh
git add README.md
```

Or you want to add ALL FILES.

```sh
git add .
```

Then, I may prepare your changes to PUSH github.

```sh
git commit -m "what kind of updates you made" 
# -m message
```

> **WARNING**
> Do not write commit messages like "Update, Add, Some ...". Write meaningful commit messages, it helps you to move through your changes.


Then **PUSH** all of your changes:

```sh
git push
```