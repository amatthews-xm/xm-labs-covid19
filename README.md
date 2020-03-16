# covid19workflow
This file is divided up into two parts, the first is instructions on creating the repo and cloning the template, the second part is the template for the `README.md` file that will serve as the home page and installation instructions for the integration. 

Some examples to emulate:
* [Logz.io](https://github.com/xmatters/xm-labs-logz.io-elk)
* [StatusPage](https://github.com/xmatters/xm-labs-statuspage)

## 1. Create the repo
[Create the repo](https://help.github.com/articles/create-a-repo/) using your own GitHub account. Please prefix the name of the repo with `xm-labs-` and all in lower case. When you create the repo don't add a README or LICENSE; this will make sure to initialize an empty repo. 

## 2. Clone the template
*Note*: These instructions use git in the terminal. The GitHub desktop client is rather limited and likely won't save you any headaches. 

Open a command line and do the following. Where `MY_NEW_REPO_NAME_HERE` is the name of your GitHub repo and `MY_NEW_REPO_URL` is the url generated when you create the new repo. 

```bash
# Clone the template repo to the local file system. 
git clone https://github.com/xmatters/xm-labs-template.git
# Change the directory name to avoid confusion, then cd into it
mv xm-labs-template MY_NEW_REPO_NAME_HERE
cd MY_NEW_REPO_NAME_HERE
# Remove the template git history
rm -Rf .git/
# Initialize the new git repo
git init
# Point this repo to the one on GitHub
git remote add origin https://github.com/MY_NEW_REPO_URL.git
# Add all files in the current directory and commit to staging
git add .
git commit -m "initial commit"
# Push to cloud!
git push origin master
```

## 3. Make updates
Then, make the updates to the `README.md` file and add any other files necessary. `README.md` files are written in GitHub-flavored markdown, see [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for a quick reference. 


## 4. Push to GitHub
Periodically, you will want to do a `git commit` to stash the changes locally. Then, when you are ready or need to step away, do a `git push origin master` to push the local changes to github.com. 

## 5. Request to add to xM Labs
Once you are all finished, let Travis know and he will then fork it to the xMatters account and update the necessary links in the xM Labs main page. From there if you update your repo, those changes can be merged into the xMatters account repo and everything will be kept up to date!

