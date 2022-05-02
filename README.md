# Building a Personal Research Website with Github and Hugo
This repository contains a tutorial for making a personal research website with Github and Hugo. Hugo is a framwork that provides static [^1] website themes. 

[^1]: Static websites host stable content that doesn't change unless you update it.


# Acknowledgements: 
This repository was adapted from [Hansen Johnson's Hugo Demo repo](https://github.com/hansenjohnson/hugo-demo) with supplementation from  [4BES.NL](https://4bes.nl/2021/08/29/create-a-website-with-hugo-and-github-pages/). 


# Why make a research website as an academic?
- Share your work
- Connect with potential collaborators
- Aggregate information (publications, resources, contact info) in one place


# How?
Make use of one of Hugo’s free templates and insert your content (contact information, project links, blogs). Then, host your newly-minted site on Github Pages and push updates with Git as needed. 


# Example: My Hugo Website via the [Avicennia theme](https://github.com/hadisinaee/avicenna)

[alburycatalina.github.io/me](alburycatalina.github.io/me)


# Let's Get Started. You will need:
- Internet connection
- [Github account](https://github.com/) and git
- Hugo
- VSCode IDE
- A browser to view your site in construction


# Step 1: Setup
1. [Install git on your machine](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Git is a kind of SCM (source code management) software. You can use it to track and finalize changes in code. Github is a place to store this version control information on the internet. Git is installed by default on most Mac and Linux machines. 

2. [Install hugo](https://gohugo.io/getting-started/installing/). This can be done in a few ways, but an easy way is via homebrew if using a mac. 
  
  With homebrew: https://brew.sh/. If you have experience working with python or ruby, Homebrew may be familiar. It's a package manager used to help out when installing software. 
  
  Install homebrew by pasting `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"` in the terminal.
  
  Then, use:`brew install hugo`
  
  You will then be prompted to enter a few more commands to add HomeBrew to your PATH. This makes them available in your terminal. These are slighlty different per computer, so copy and paste the commands that you are prompted with. 
  
  
3. [Install VS code](https://code.visualstudio.com/)

VS code is an IDE (interactive development environment) that has lots of cool tools to help you manage your website. You can navigate files and push directly to Github if you like. 


# Step 2: Make a new github repo 

1. Make a github repo to host your site

You have two options for the URL that your website will be hosted under: either (your username).github.io or (your username).github.io/(repository name). Either is great depending on your usage, but let's try out hosting via your main URL for now. 
  
 Name the new repository (your username).github.io. You should tick the "add a README file" box and select whether your repository will be public or private (private repos are restricted to Github pro, which available at no cost to students). 
 
2. Clone the Repo

Once you've created the repository, you can [clone it to your computer](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) with command line. This creates a local copy of the repo on your computer. 
 
 Hit the green code button in the top right corner of the github repository and copy the link to clone with HTTPS.
 
 Make a folder for your website (ex: a folder called "Personal_Website" and change the terminal directory to it.
 
 In terminal, type `cd ~/Personal_Website`
 
 Type `git clone` and paste in the copied URL from before. 
 
 For example: `$ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`
 
 If you open the folder that you cloned your repo to, you should see the README file. 
  
  
  
 # Step 3: Make a Site and choose a Theme

Still in your "Personal_Website" folder, make a new site with Hugo. 

In terminal, paste `hugo new site .\ --force`. You will see that hugo creates a file structure with folders named things like "static", "layout" and more. There will also be a file named `config.toml` which will be important soon. 



Hugo has a wealth of user created website themes that you can browse [here](https://themes.gohugo.io/). Most come with great guides on how to use them. 

Let's try out the [Cactus theme](https://themes.gohugo.io/themes/hugo-theme-cactus/) as an example. Head to the link, click the yellow download button. This will take you to the theme's github page with instructions. 

From Cactus' info page, we can use the following code to add the theme to our website:

`git clone https://github.com/monkeyWzr/hugo-theme-cactus.git themes/cactus`



# Step 4: Edit Theme & Preview

Most sites will allow most changes to be done on the `config.toml` file. It is at least mandatory that you change the base URL to the URL of your site (ex: (your username).github.io). 

Let's update this in the `config.toml` file, along with changing the main page title and description. Save the `config.toml` when your changes are complete. 

Note: The "static" folder usually holds photos and files for uploading. 

Tip: For quick editing, identify which aspect of text you'd like to change and cmd+F the text in the config.toml file to identify it and change it. 

You can see what the site looks like locally by running  `Hugo server -D`

The return will be a localhost URL, which you can preview in your browser. 

# Step 5: Commit & Publish

When the website is complete, host it on your Github page and share the link to your friends, family, colleagues, and mortal enemies. 

In the Github repo, go to Settings > Pages > Change "Source" to "Main." If done correctly, you should get a message along the lines of "Your site is ready to be published at https://username.github.io. Successs!

Finalize the page by simply running `hugo` in your website directory. 

It can take 5-10 minutes for published changes in your Github repo to be reflected in the live page. 

In the future, edit website files and use the follwoing commands to push and commit website edits to the directory. 

`git commit -A`
`git push -u origin master`









