# Git

## Useful Commands

### Intallation

```
sudo apt intall git
```

### First Time Config

```
git config --global init.defaultBranch main
git config --global user.name "Sebastián García Viera"
git config --global user.email "email@gmail.com"
```

### Initialize Repository

```
cd my-project
git init 
```

### Select a File to be tracked in version control

```
git add my-file.txt
```

### See the files that are ready to be committed (staged)

```
git status
```

### Commit Staged Files

```
git commit -m "message"
```
## Remote GitHub Repository

### Generate public and private keys for GitHub
**This enables my local computer to push to GitHub**

```
ssh-keygen -t ed25519 -C "email@gmail.com"
cat /home/sebastian/.ssh/id_ed25519.pub
```


And paste the public key [here](https://github.com/settings/ssh/new)


### Connect Local Repository with a remote one in GitHub

**First initialize an empty remote repository on GitHub**
```
git remote add origin git@github.com:sgviera/my-project.git
git branch -M main
git push -u origin main
```

### Push other commits

```
git add otherfile.txt
git commit -m "another message"
git push
```

### Adding all the files and folder inside the project to staged

```
git add .
```
