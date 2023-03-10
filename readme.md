# Host a Resume on GitHub Pages

## Purpose  
This document will teach people how to host and format a resume online.  

## Prerequisites  
### Resume
We need a formatted resume in Markdown.

### Software

There are something we need to install on computer before we get start to host and format our resume.  
* Find a Markdown editor and install it
* Download GitHub desktop and install it
* Install a static site generater(We will use Jekyll as an example)  
	* We need install [ruby](https://rubyinstaller.org/downloads/) before we start install Jekyll
	* Don't install latest version of ruby, it may not compatible with Jekyll(rubyinstaller-devkit-2.7.0-1 is recommended)
<center><img src="ruby.gif" width = "" height = ""></center>


### More Resources  
* We should know how to use Markdown to write a file, here is a good resource to learn: [good markdown tutorial](https://www.markdowntutorial.com/)
* We should have a GitHub account. If you don't have one, go to [GitHub](https://github.com/) to create one.  


## Instruction  
### Make Local Static Site  
1. Create a folder and open a terminal on your computer
2. Run this command "jekyll new [your site name]"
3. Use "cd [your site name]" to change to that directory
4. run "bundle exec jekyll serve" to generate the site at first time, you only need to run "jekyll serve" after first time.
5. Then copy and paste the url at Serve address to our browser, you can see our site locally.  
(Note: don't close the terminal when we run our local site)
<center><img src="run_local_site.gif" width = "" height = ""></center>
<center><img src="run_site_browser.gif" width = "" height = ""></center>

6. Move our resume into this root folder  
7. Delete the default "index.md"  
8. Add "---  
&emsp; &ensp; &ensp;layout: home  
&emsp; &emsp; ---"  
in our resume  
<center><img src="add_layout.gif" width = "" height = ""></center>  
9. Rename the resume to "index.md"  
10. Delete ererything in "_config.yml" except theme and plugins  
<center><img src="modify_config.gif" width = "" height = ""></center>  
Now our resume should at the home page.  

### Put Static Site In GitHub Pages  
1. Go to [GitHub](https://github.com/) and login your account
2. Create a new repository by click the "+" at top right corner
3. Set repository name in this format: [your account name].github.io
(Note: don't add readme file by default)  
<center><img src="repo_name.gif" width = "" height = ""></center>  
4. Open GitHub Desktop and clone the repository that we just created  
5. create a new brank called "gh-pages"  
6. copy every file that in our local site folder and paste to the repository folder  
7. Commit these files and push to GitHub  
