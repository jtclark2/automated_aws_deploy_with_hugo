# Hugo Static Website Demo/Tutorial for AWS Deployment
This is a very simple static website built with HUGO. The site is barely more than a "Hello World", but it's being used to configure automated deployment to AWS. The buildspec and config files are needed in this repo, though most of the configuration/setup is in AWS.

# Purpose:
1) Brief exposure to Hugo
2) This repo is being used to explore deployments and automation/devOps tools on AWS. 

# Author's Note about Repo Structure
The structure of this repo is a bit unusual, but recommended in Coursera's **Cloud Computing Foundations** class.

## How was this structure created?
1) [Install hugo](https://github.com/gohugoio/hugo/releases/download/v0.87.0/hugo_extended_0.87.0_Linux-64bit.tar.gz)
2) `hugo new site quickstart` to create a site using the hugo tools in a `quickstart` subdirectory
3) Flatten the directory structure by moving the contents of that subdirectory up a level, and then deleting the `quickstart`. 
4) Create subdirectory `git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke`
5) Configure theme: `echo 'theme = "ananke"' >> config.toml`
6) Start playing with the project, adding posts, etc.
