# Building a Personal Research Website with Github and Hugo
A tutorial for making a personal research website with Github and Hugo. Hugo provides static website themes (ex: with stable content that doesn't change unless you update). 


Acknowledgements: This repo was adapted from [Hansen Johnson's Hugo Demo page](https://github.com/hansenjohnson/hugo-demo) with supplementation from  [4BES.NL](https://4bes.nl/2021/08/29/create-a-website-with-hugo-and-github-pages/). 

# Why make a research website as an academic?
- share your work
- connect with others
- aggregate your projects, publications, and other information in one place


# How?
Make use of one of Hugo’s free templates and insert your content (contact information, project links, blogs)
Host on Github Pages and push updates as needed

# Example: My Hugo Website via [Avicennia theme(https://github.com/hadisinaee/avicenna)

[alburycatalina.github.io/me](alburycatalina.github.io/me)

# Let's Get Started. You will need:
- Internet connection
- Github account and git
- Hugo
- VSCode
- A browser to view your site in construction



# Step 1: Setup
1. Install git on your machine: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

Git is a kind of SCM (source code management) software. You can use it to track and finalize changes in code. Github is a place to store this version control information on the internet. Git is installed by default on most Mac and Linux machines. 




2. Install hugo : https://gohugo.io/getting-started/installing/. This can be done in a few ways, but an easy way is via homebrew if using a mac. 
  
  With homebrew: https://brew.sh/ (if work with python or ruby this may be familiar. Homebrew is a package manager)
  
  
  Install homebrew: `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` in terminal
  
  `brew install hugo`
  
  You will then be prompted to enter a few more commands to add HomeBrew to your PATH. This makes them available in your terminal. These are slighlty different per computer, so copy and paste the ones that you are prompted with. 
  
  
3. Install VS code: https://code.visualstudio.com/

VS code is an IDE (interactive development environment) that has lots of cool tools to help you manage your website. 



# Step 2: Make a Site and choose a Theme

Make a folder for your website and change the terminal directory to it.

`cd ~/Website`

Then, make a new site with hugo in a new directory:

`hugo new site personal_website`

Themes: https://themes.gohugo.io/

Try: https://themes.gohugo.io/themes/hugo-theme-jane/




# Step 2: Make a new github repo 

Make a github repo (main.github.io or main/thing.github.io)



# 


# Step 

Edit config.toml for website address. Static folder usually holds pictures etc. 


`Hugo server -D`




