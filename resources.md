---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: archive
layout: single   
title: Software + Resources   
lang: en   
ref: res   
permalink: /resources/   
toc: true
toc_label: "Software + Resources" 
toc_icon: "laptop"  
toc_sticky: true   
read_time: true  
date: 2023-08-01  
last_modified_at: 2023-08-28   

---

<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/lipis/flag-icons@6.11.0/css/flag-icons.min.css"/>

<div class="lang-sidebar">
  {% assign pages=site.pages | where:"ref", page.ref | sort: 'lang' %}
  {% for page in pages %}
    <li class="zoom"><a href="{{ page.url }}" class="{{ page.lang }}"><span class="fi fi-{{ page.lang }}"></span></a></li>
  {% endfor %}
</div>

<div class="top-h1-icon">
  <i class="fas fa-laptop fa-2x"></i>
</div>

A list of stuff we'll be using throughout the course.    

_Be sure to install + test these before you arrive in class._   

## MaxMSP      

_Download + install the current build from:_ <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://cycling74.com/downloads" target="_blank" class="btn btn--primary">MaxMSP</a></span>

Most recent releases should support our work in class, however. 

At the time of this publication, all software for the class was tested up to Max version 8.5.2 (c9ba072623d) (x64 mac rosetta) on macOS version 12.3 (Build 21E230) x86_64 Rosetta.   

### Temporary Max License Keys   

If you don't have your own, <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="mailto:Louis.Goldford@mh-luebeck.de/?subject=[MHL%20Advanced%20CAO]%20Max%20License%20request" target="_blank" class="btn btn--danger">**email me to request a software license key**</a></span>     

We typically have a few licenses available to students enrolled in our courses. 

They are made available on a first-come-first-serve basis. 

If a license key is free, I can make it available to you for the duration of this course and possibly longer, depending on how many other requests I get. Ideally, we would like to ensure you have access to Max for as long as you would need to finish a project.   

## Max Packages + Libraries     

A rolling list of Max packages that we will be using.   
_We may add to this list throughout the semester:_   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	1. <a href="https://www.bachproject.net/dl/" target="_blank" class="btn btn--primary">bach</a> for computer-assisted composition   
	2. <a href="https://forum.ircam.fr/projects/detail/spat/" target="_blank" class="btn btn--primary">IRCAM spat~</a> for multichannel audio spatialization   
	3. <a href="https://forum.ircam.fr/projects/detail/modalys/" target="_blank" class="btn btn--primary">IRCAM Modalys</a> for physical modeling ("modal") synthesis   
	4. <a href="https://github.com/maccallum/x/" target="_blank" class="btn btn--primary">X</a> for random number generation and distribution   
</span>

### Manual Package Installation   

Of the packages listed above, #1 can be installed directly from the [Max Package Manager](#using-the-max-package-manager) _(see description below)_. 

#2 — #4 must be downloaded directly from their websites linked above and then manually installed. 

Download and decompress each installer and place its unzipped folder into your `Max 8/Packages`. 

This folder is located at:

```
/Users/username/Documents/Max 8
```
_Be sure to replace_ `username` _above with the actual user name on your computer._

#### Register for the IRCAM Forum   

To acquire Max packages #2 and #3 above, you must create a **free** account on the [IRCAM Forum website](https://forum.ircam.fr/){:target="_blank"}.  

Once you register, you'll be able to download Modalys and Spat.  

These packages are free and will not incure any additional costs.  

### Using the Max Package Manager   

Some packages can be instantly installed through the [Max Package Manager](https://docs.cycling74.com/max7/vignettes/package_manager){:target="_blank"}, such as #1 above, bypassing the need to manually unzip and move any folders into specific locations. 

To begin, in MaxMSP go to `File > Show Package Manager`.   

In the Package Manager window that pops up, type the name of a package, e.g., `miraweb`, in the search bar at the upper-right, and then click the MiraWeb package at the bottom to install:  

<img src="/assets/images/01.package.manager.png" alt="package manager">

On the next page, click the <span style="font-weight: bold; color: lightblue;">blue</span> `Install` button:

<img src="/assets/images/02.install.png" alt="install">

When finished, you should see a <span style="font-weight: bold; color: lightblue;">blue</span> `Launch` button and a "Successfully installed Miraweb" message:

<img src="/assets/images/03.success.png" alt="install">

From here, you can simply close the Package Manager window.  

Repeat these step to quickly install additional packages.  

_Unfortunately, this method does not work for the IRCAM packages, which must be installed manually from the IRCAM Forum website, as described in [Manual Package Installation](#manual-package-installation) above._  

## Windows: Terminal Emulator   

If your computer runs a Windows operating system, you'll need a program that mimics the behavior of the Unix command line.

<span style="color: red;">_NOTE: macOS + Linux users can ignore this step!_</span>  

Install **one** of these apps:  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://gitforwindows.org/" target="_blank" class="btn btn--primary">Git BASH</a> <a href="https://cmder.net/" target="_blank" class="btn btn--primary">Cmder</a> <a href="https://xshell.en.softonic.com/" target="_blank" class="btn btn--primary">Xshell</a> <a href="https://www.puttygen.com/download-putty" target="_blank" class="btn btn--primary">XPuTTY</a>      
</span>

Of these, the first option (Git Bash) has been the most reliable for my previous students.   

Or, check out some alternatives: [15 Best Terminal Emulators for Windows in 2023](https://www.puttygen.com/windows-terminal-emulators){:target="_blank"}  

## macOS + Linux: Homebrew  

A Package management system to ease installation of other tools and software in the Terminal.    

<span style="color: red;">_NOTE: Windows users can ignore this step!_</span>  

### Install     

Open your Terminal and run:  

```
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```

You may then need to run the following commands to check your installation and update:  

```
brew doctor
```

and 

```
brew update
```

### Verify    

In your Terminal, run this:  

```
brew --version
```

Your console should return a message that looks like this:  

```
Homebrew 2.4.9
```

or

```
Homebrew/homebrew-core (git revision 58437; last commit 2020-08-08)
```

## Version Control with GIT + GitHub   

Git is a very powerful **distributed version control** system for intelligently backing up and tracking changes in your code, or in any set of files.  

It functions alongside **GitHub.com**, which we'll use as a cloud storage platform to keep our files safe, and to submit projects and assignments.   

<span style="color: red;">_NOTE: We installed and used these tools in the previous seminar **Sound Synthesis Techniques**, and we'll continue to use them this semester._</span>  

If you have already taken the time to install these tools, simply **skip this section**. But if you are just joining our class and have not yet worked with these tools, follow the video tutorials below.  

### Register for GitHub.com  

<span style="color: red;">_NOTE: You'll be using GIT (and GitHub.com) to regularly submit class patches and your final projects, so be sure to set this up!_</span>  

Go to [GitHub.com](http://github.com){:target="_blank"} and follow the prompts to set up your **free** account. 

Or visit [this 'How-To' Page for extra support.](https://www.wikihow.com/Create-an-Account-on-GitHub){:target="_blank"}  

#### Verify: Email me!   

Immediately <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="mailto:Louis.Goldford@mh-luebeck.de/?subject=[MHL%20Advanced%20CAO]%20GitHub%20user%20name" target="_blank" class="btn btn--danger">**email me your GitHub user name**</a></span> to receive grades in this class!

### GIT Version Control     

To set up GIT on your computer, follow the video tutorial as a quickstart guide:   

{% include video id="Lw2OgM6tQd8" provider="youtube" %}

Windows Users: install GIT using [Git for Windows](https://gitforwindows.org/){:target="_blank"}  

macOS users: Follow the instructions using Homebrew below...  

#### Install   

Run the following commmand:  

```
brew install git  
```

#### Verify

Run the following commmand:  

```
git --version
```

Your console should return a message that looks like this:   

```
git version 2.20.1 (Apple Git-117)
```

### Large File Storage (LFS)  

Large File Storage (LFS) is a Git **extension** that allows you to verison large binary files — like audio, video, and image files. 

By itself, Git isn't very capable of versioning binary files. Without this extension, your Git folder ("repository") will quickly "blow up" and run out of space. 

Install this valuable extension so that you can safely backup your media files and reserve valuable repository space for your code!     

Download and install the extension here: <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://git-lfs.com/" target="_blank" class="btn btn--primary">Git LFS</a></span>

Altenatively,  macOS users can install via Homebrew:  

```
brew install git-lfs
```

Follow the steps outlined in the video tutorial below to set everything up:  

{% include video id="HLyoH7xfoF8" provider="youtube" %}

<!-- 
## 6. Google Chrome  
_A web browser with great built-in device compatibility tools._  

1. INSTALL:  
	* [Direct from Chrome homepage](https://www.google.com/intl/en/chrome/){:target="_blank"}  
2. VERIFY:  
	* Chrome can be launched from your /Applications folder.  


## 7. Python 3 + pip
_**Python** is an object-oriented, interpreted, and interactive programming language that we'll be introducing alongside JavaScript. It's great for quick prototyping and even better for data visualization._  

_**pip** is the standard package manager for the Python language, allowing you to easily install code packages + modules from the extensive [standard library.](https://docs.python.org/3/py-modindex.html){:target="_blank"}_  

1. INSTALL using these tutorials:  
	* [macOS](https://evansdianga.com/install-pip-osx/){:target="_blank"}  
	* [Windows](https://phoenixnap.com/kb/install-pip-windows){:target="_blank"}  
2. VERIFY:  
	* Verify Python 3:  
		* Open your Terminal and run:  
			`python3 --version`  
		* Your console should return something that looks like this:  
			`Python 3.8.5`
	* Verify pip:  
		* Open your Terminal and run:  
			`pip --version`  
		* Your console should return something that looks like this:  
			`pip 20.2 from /Library/Frameworks/Python.framework/Versions/3.8/lib/python3.8/site-packages/pip (python 3.8)`  
		* or:  
			`pip 18.1 from C:\Python37\lib\site-packages\pip (python 3.7)`  
3. Create an alias so that anytime you run `python` on the command line, you'll be using Python 3 instead of older versions.  
	* When using Python, run this command when you **begin** a Terminal session:  
			`alias python=/usr/local/bin/python3`   -->

## Additional + Optional Resources   

### Software      

#### Text Editor  

Highlight your code, easily find & replace, and a LOT more... 

_Check your operating system for compatibility and install one of these:_  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://code.visualstudio.com/download/" target="_blank" class="btn btn--primary">Visual Studio Code</a> <a href="https://www.sublimetext.com/" target="_blank" class="btn btn--primary">Sublime Text</a> <a href="https://espressoapp.com/" target="_blank" class="btn btn--primary">Espresso</a> <a href="https://brackets.io/" target="_blank" class="btn btn--primary">Brackets.io</a>
</span>

#### Digital Audio Workstations (DAWs)   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://www.reaper.fm/download.php/" target="_blank" class="btn btn--primary">Reaper</a> <a href="https://www.ableton.com/en/trial/" target="_blank" class="btn btn--primary">Ableton Live</a>
</span>

#### Audio Analysis Tools   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://logiciels.pierrecouprie.fr/" target="_blank" class="btn btn--primary">iAnalyse</a> <a href="https://www.izotope.com/en/rx.html?" target="_blank" class="btn btn--primary">iZotope RX</a> <a href="https://www.klingbeil.com/spear/" target="_blank" class="btn btn--primary">SPEAR</a>
</span>

### Free Sample Libraries    

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://freesound.org/" target="_blank" class="btn btn--primary">FreeSound.org</a> <a href="https://archive.org/details/nasaaudiocollection" target="_blank" class="btn btn--primary">NASA Audio Collection</a> <a href="https://www.nps.gov/subjects/sound/gallery.htm" target="_blank" class="btn btn--primary">Natural Sounds Gallery</a> <a href="https://theremin.music.uiowa.edu/MIS.html" target="_blank" class="btn btn--primary">Instrumental Samples</a>
</span>

### Tutorials   

#### MaxMSP   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://music.arts.uci.edu/dobrian/maxcookbook/node/56" target="_blank" class="btn btn--primary">Max Cookbook</a> <a href="https://cycling74.com/forums" target="_blank" class="btn btn--primary">MaxMSP User Forum</a> <a href="https://docs.cycling74.com/max8" target="_blank" class="btn btn--primary">Max 8 Documentation</a> <a href="http://peterelsea.com/maxtutorials.html" target="_blank" class="btn btn--primary">Peter Elsea Tutorials</a> <a href="http://www.maxobjects.com/" target="_blank" class="btn btn--primary">Max Objects Database</a>
</span>


