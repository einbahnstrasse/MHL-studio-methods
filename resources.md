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
show_date: true  
date_format: "%Y-%m-%d"  
date: 2023-08-01  
last_modified_at: 2023-08-28   

---

<!-- <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/lipis/flag-icons@6.11.0/css/flag-icons.min.css"/>

<div class="lang-sidebar">
  {% assign pages=site.pages | where:"ref", page.ref | sort: 'lang' %}
  {% for page in pages %}
    <li class="zoom"><a href="{{ page.url }}" class="{{ page.lang }}"><span class="fi fi-{{ page.lang }}"></span></a></li>
  {% endfor %}
</div>

<div class="top-h1-icon">
  <i class="fas fa-laptop fa-2x"></i>
</div> -->

A list of stuff we'll be using throughout the course.    

_Be sure to install + test these before you arrive in class._   

_For all software below, be sure sure to choose the version that matches your computer’s operating system (e.g., Windows, macOS, Linux, etc.)._  


## Reaper   

Reaper is a Digital Audio Workstation (DAW), which we will be using to _sequence_ and _edit_ our audio throughout the semester. 

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://www.reaper.fm/download.php" target="_blank" class="btn btn--primary">Install Reaper from this link.</a></span>   

<img src="/MHL-studio-methods/assets/images/Reaper-DAW-software-1.png" alt="Reaper interface">  

### Extra Packages for Reaper  

To make Reaper more useful, we may occasionally install extra software libraries for use with Reaper.  

_At the moment, there are no libraries to install, but we may include a list of them below throughout the semester:_   

* * *  

## SpatGRIS  

SpatGRIS is an audio spatialization tool that we will use to make our final pieces for the semester.  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://sourceforge.net/projects/spatgris3/files/" target="_blank" class="btn btn--primary">Download SpatGRIS here.</a></span>   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://gris.musique.umontreal.ca/" target="_blank" class="btn btn--primary">Informational page about SpatGRIS</a></span>   

<img src="/MHL-studio-methods/assets/images/spatGRIS.png" alt="spatGRIS interface">  

### BlackHole or JACK  

To route multi-channel audio signals from our DAW (Reaper) into SpatGRIS, we need another program.  

If you are a macOS user, download and install     

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://existential.audio/blackhole/" target="_blank" class="btn btn--primary">BlackHole</a></span>   

If you are a Windows user, download and install   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://jackaudio.org/downloads/" target="_blank" class="btn btn--primary">JACK</a></span>   

Windows users: watch this instructional video for using SpatGRIS with JACK:   

{% include video id="hrX9ZdK2DPM" provider="youtube" %}



* * *   

## SPEAR    

SPEAR is an application for audio analysis/resynthesis. We use SPEAR to “dissect” a sound into its component frequencies and to represent that sound on an interactive spectrographical editor.  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://www.klingbeil.com/spear/downloads/" target="_blank" class="btn btn--primary">Download SPEAR here.</a></span>   

<img src="/MHL-studio-methods/assets/images/spear_screen_bigsur.png" alt="SPEAR interface">  

* * *   

## MaxMSP      

_Download + install the current build from:_ <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://cycling74.com/downloads" target="_blank" class="btn btn--primary">MaxMSP</a></span>  

Most recent releases should support our work in class, however.  

At the time of this publication, all software for the class was tested up to Max version 8.5.2 (c9ba072623d) (x64 mac rosetta) on macOS version 12.3 (Build 21E230) x86_64 Rosetta.   

<img src="/MHL-studio-methods/assets/images/maxmsp_interface.png" alt="MaxMSP interface">  

### Temporary Max License Keys   

If you don't have your own, <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="mailto:Louis.Goldford@mh-luebeck.de/?subject=[MHL%20Advanced%20CAO]%20Max%20License%20request" target="_blank" class="btn btn--danger">**email me to request a software license key**</a></span>     

We typically have a few licenses available to students enrolled in our courses. 

They are made available on a first-come-first-serve basis. 

If a license key is free, I can make it available to you for the duration of this course and possibly longer, depending on how many other requests I get. Ideally, we would like to ensure you have access to Max for as long as you would need to finish a project.   

## Max Packages + Libraries     

To make MaxMSP more useful, we may occasionally install extra software libraries for use with MaxMSP.  

_At the moment, there are no libraries to install, but we may include a list of them below throughout the semester:_   

<!-- <span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	1. <a href="https://www.bachproject.net/dl/" target="_blank" class="btn btn--primary">bach</a> for computer-assisted composition   
	2. <a href="https://forum.ircam.fr/projects/detail/spat/" target="_blank" class="btn btn--primary">IRCAM spat~</a> for multichannel audio spatialization   
	3. <a href="https://forum.ircam.fr/projects/detail/modalys/" target="_blank" class="btn btn--primary">IRCAM Modalys</a> for physical modeling ("modal") synthesis   
	4. <a href="https://github.com/maccallum/x/" target="_blank" class="btn btn--primary">X</a> for random number generation and distribution   
</span> -->

<!-- ### Manual Package Installation   

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

These packages are free and will not incure any additional costs.   -->

### Using the Max Package Manager   

Some packages can be instantly installed through the [Max Package Manager](https://docs.cycling74.com/max7/vignettes/package_manager){:target="_blank"}, bypassing the need to manually unzip and move any folders into specific locations.  

To begin, in MaxMSP go to `File > Show Package Manager`.   

In the Package Manager window that pops up, type the name of a package, e.g., `miraweb`, in the search bar at the upper-right, and then click the MiraWeb package at the bottom to install:  

<img src="/MHL-studio-methods/assets/images/01.package.manager.png" alt="package manager">

On the next page, click the <span style="font-weight: bold; color: lightblue;">blue</span> `Install` button:

<img src="/MHL-studio-methods/assets/images/02.install.png" alt="install">

When finished, you should see a <span style="font-weight: bold; color: lightblue;">blue</span> `Launch` button and a "Successfully installed Miraweb" message:

<img src="/MHL-studio-methods/assets/images/03.success.png" alt="install">

From here, you can simply close the Package Manager window.  

Repeat these step to quickly install additional packages.  

<!-- ## Windows: Terminal Emulator   

If your computer runs a Windows operating system, you'll need a program that mimics the behavior of the Unix command line.

<span style="color: red;">_NOTE: macOS + Linux users can ignore this step!_</span>  

Install **one** of these apps:  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://gitforwindows.org/" target="_blank" class="btn btn--primary">Git BASH</a> <a href="https://cmder.net/" target="_blank" class="btn btn--primary">Cmder</a> <a href="https://xshell.en.softonic.com/" target="_blank" class="btn btn--primary">Xshell</a> <a href="https://www.puttygen.com/download-putty" target="_blank" class="btn btn--primary">XPuTTY</a>      
</span>

Of these, the first option (Git Bash) has been the most reliable for my previous students.   

Or, check out some alternatives: [15 Best Terminal Emulators for Windows in 2023](https://www.puttygen.com/windows-terminal-emulators){:target="_blank"}  

## Additional + Optional Resources   

### Software      

<!-- #### Text Editor  

Highlight your code, easily find & replace, and a LOT more... 

_Check your operating system for compatibility and install one of these:_  

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://code.visualstudio.com/download/" target="_blank" class="btn btn--primary">Visual Studio Code</a> <a href="https://www.sublimetext.com/" target="_blank" class="btn btn--primary">Sublime Text</a> <a href="https://espressoapp.com/" target="_blank" class="btn btn--primary">Espresso</a> <a href="https://brackets.io/" target="_blank" class="btn btn--primary">Brackets.io</a>
</span> -->

<!-- #### Digital Audio Workstations (DAWs)   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://www.reaper.fm/download.php/" target="_blank" class="btn btn--primary">Reaper</a> <a href="https://www.ableton.com/en/trial/" target="_blank" class="btn btn--primary">Ableton Live</a>
</span> -->

## VCV Rack      

_for virtual modular synthesis_  
<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;"><a href="https://vcvrack.com/Rack#get" target="_blank" class="btn btn--primary">VCV Rack</a></span>  

<img src="/MHL-studio-methods/assets/images/VCVrack.png" alt="VCVrack.png">

* * *   

## Additional + Optional Resources   

### YouTube: Electroacoustic + Acousmatic Music   

<iframe width="560" height="315" src="https://www.youtube.com/embed/videoseries?si=dGmT6dvsMcJbrF1u&amp;list=PLJiSOq8uc1_-jrDCDCAqAhAECYbwWrqr_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Audio Analysis Tools   

<a href="https://logiciels.pierrecouprie.fr/" target="_blank" class="btn btn--primary">iAnalyse</a>  

<img src="/MHL-studio-methods/assets/images/ianalyse_interface.v01.png" alt="iAnalyse interface">  

### Free Sample Libraries    

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://freesound.org/" target="_blank" class="btn btn--primary">FreeSound.org</a> <a href="https://archive.org/details/nasaaudiocollection" target="_blank" class="btn btn--primary">NASA Audio Collection</a> <a href="https://www.nps.gov/subjects/sound/gallery.htm" target="_blank" class="btn btn--primary">Natural Sounds Gallery</a> <a href="https://theremin.music.uiowa.edu/MIS.html" target="_blank" class="btn btn--primary">Instrumental Samples</a>
</span>

### Field Recording On Your Phone   

_You can request a Zoom device or field recorder from the studio, but it is sometimes even more convenient to record high-quality audio on your phone using a free app! 2 apps are listed below._    

_The challenge with mobile recording apps that don't require a microphone is this: they use your phone's built-in microphone, which is usually a very ambient **omni-directional microphone**. It is therefore crucial that you **carefully point your phone towards the sound source you want to record** in order to minimize indirect and ambient sound when field recording._    

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://apps.apple.com/us/app/apogee-metarecorder/id965930387" target="_blank" class="btn btn--primary">Apogee MetaRecorder (iPhone app)</a> <a href="https://play.google.com/store/apps/details?id=com.dolby.dolby234&hl=en&gl=US" target="_blank" class="btn btn--primary">Dolby On (Android app)</a>
</span>

_Other phone apps are also available. Whichever app you choose, be sure to set the app's preferences to record at our studio's standard **sampling rate (48kHz) and bit rate (24 bit)**. Unfortunately, Dolby On may only allow you to record in 16-bit, but you might find another app that can do better. Dolby On also has a lots of great audio editing features._  

#### Apogee MetaRecorder Quickstart Video Guide   

{% include video id="QoD4OQey4m4" provider="youtube" %}  

#### Dolby On – Full Walkthrough Tutorial   

{% include video id="n6UVVpXc8Og" provider="youtube" %}  

### Tutorials   

#### MaxMSP   

<span style="font-size: smaller; text-transform: uppercase; font-weight: bold;">
	<a href="https://music.arts.uci.edu/dobrian/maxcookbook/node/56" target="_blank" class="btn btn--primary">Max Cookbook</a> <a href="https://cycling74.com/forums" target="_blank" class="btn btn--primary">MaxMSP User Forum</a> <a href="https://docs.cycling74.com/max8" target="_blank" class="btn btn--primary">Max 8 Documentation</a> <a href="http://peterelsea.com/maxtutorials.html" target="_blank" class="btn btn--primary">Peter Elsea Tutorials</a> <a href="http://www.maxobjects.com/" target="_blank" class="btn btn--primary">Max Objects Database</a>
</span>


