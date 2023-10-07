---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

# layout: archive
layout: single   
title: Schedule   
lang: en   
ref: sched   
permalink: /schedule/   
# sidebar:
#   nav: "schedule-toc"   
toc: true  
toc_label: "Schedule" # default: Content
toc_icon: "bell"  # corr esponding Font Awesome icon name without the "fa" prefix
toc_sticky: true   # enables sticky toc 
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
  <i class="fas fa-bell fa-2x"></i>
</div>

<!-- <img src="/Goldford-MTEC1003/assets/organized.gif" alt="organized" width="400" align="right"> -->

<!-- # Schedule -->
_This page will be updated frequently with examples, video tutorials, links to new resources, and occasional updates to LAB ASSIGNMENTS. Our schedule follows the [Current MHL Academic Calendar]({{ site.MHL-calendar }}){:target="_blank"}. The following topics and their precise order may change. Check here for updates!_  

* * *

## Week 1: {{ site.week-01 }}  

<!-- ### [Week #1 Survey/Quiz — Personal Info, Syllabus Elements](https://forms.gle/HeYNxzVSuG67M3Nb8){:target="_blank"}   -->
<!-- * _Complete the quizlet above as part of today's participation._   -->

#### Start-of-Semester Business  

* Review [Syllabus + course policies](/MHL-studio-methods/){:target="_blank"}  
* Review [Detailed Breakdown of Grading](/MHL-studio-methods/grading.html){:target="_blank"}  
<!-- * Review [Keys for Success in MTEC1003](/Goldford-MTEC1003/resources/week.01/keys.for.success.html){:target="_blank"}   -->

#### Tutorials
* [Let's Learn About Waveforms _(Interactive Guide)_](https://pudding.cool/2018/02/waveforms/){:target="_blank"}  

<!-- #### Video Tutorial
##### Stepping Through Week 1 Slides + Labs    

<div class="video">
    <figure>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/O617zAPuNng" frameborder="0" allowfullscreen></iframe>
    </figure>
</div>
_Normally we won't record our classes but sometimes we may in order to clarify complex topics. This video is archived from a previous version of this class, but the directions are all the same. For the 2 labs (below) this week, enter your respones in the text files and then save your changes directly on GitHub (i.e. "commit" your changes), as demonstrated and described in class and in this video. The slides above will help guide you to these answers, so be sure to study them and use to your advantage. Don't forget to study the slides for Week 2 before next class!_   

##### Lab Assignments

<div class="instructornote"><p markdown="span"><em>{{ site.weekly-deadline-statement }}</em></p></div>  
* [Setting Up GitHub for Submitting Labs](/Goldford-MTEC1003/labs/01/how.to.submit.1st.week.labs.html){:target="_blank"}  
* [Lab 1 / Part 1: Commands + Navigation](https://github.com/einbahnstrasse/mtec1003-week1-labs/blob/master/lab.01.part1.commands.navigation.txt){:target="_blank"}  
* [Lab 1 / Part 2: Download + (Un)Compress](https://github.com/einbahnstrasse/mtec1003-week1-labs/blob/master/lab.01.part2.download.compress.txt){:target="_blank"}   -->

<!-- * * * -->

<!-- <a id="w2"></a> -->
<!-- <h3 class="schedule-page-date">Week 2: {{ site.week-02 }}</h3> -->
## Week 2: {{ site.week-02 }}  

<!-- ### File System: Shell Scripting, Permissions, Date/Time, Editing Files  

### [Week 2 Quizlet](https://forms.gle/vFneHmAUaNeTaHo4A){:target="_blank"}  
* _Complete the quizlet above as part of today's attendance + participation._  

<h5 style="color:Tomato;"><b>SLIDES</b></h5>  
* [Review](/Goldford-MTEC1003/labs/03/review.html#1.0){:target="_blank"}  
* [Working With Files](/Goldford-MTEC1003/labs/03/working-with-files.html){:target="_blank"}  
* [File Permissions, Editing, Date + Time, Shell Scripting](/Goldford-MTEC1003/labs/03/permissions-editing-date-time.html){:target="_blank"}  
* [Shell Scripting: Some Odds and Ends](/Goldford-MTEC1003/labs/04/shell-scripting.html#1.0){:target="_blank"}  

<h5 style="color:Tomato;"><b>LAB ASSIGNMENTS</b></h5>
* [Submitting Week 2 Labs](/Goldford-MTEC1003/labs/02/how.to.submit.2nd.week.labs.html){:target="_blank"}  
* Lab 2 / Part 1 has been removed: We'll only complete the following 2 labs this week!    
* [Lab 2 / Part 2: Working with Files](/Goldford-MTEC1003/labs/02/lab.02.part2.working.with.files.txt){:target="_blank"}  
* [Lab 2 / Part 3: Shell Scripting, Permissions, Editing Text, Date + Time](/Goldford-MTEC1003/labs/02/lab.02.part3.shell.scripting.txt){:target="_blank"}   -->

* * *

## Week 3: {{ site.week-03 }}  
<!-- ### Version Control: Introduction to GIT, Concepts + Basic Commands   -->

* * *

## Week 4: {{ site.week-04 }}  
<!-- ### Version Control: Local/Remote Repositories + Collaboration Via _GitHub_   -->

* * *

## Week 5: {{ site.week-05 }}  
<!-- ### JavaScript + Python: Introduction, Variables, Types, Input/Output -->

* * *

## Week 6: {{ site.week-06 }}  
<!-- ### Review: Version Control + Basic JavaScript/Python   -->


* * *

## Week 7: {{ site.week-07 }}  
<!-- ### Javascript + Python: Conditionals -->
<!-- <p class="redish"><i>Spring Recess 3/27-4/4. See <a href="https://www.citytech.cuny.edu/registrar/docs/spring_2021.pdf" target="_blank">CityTech Spring 2021 Schedule.</a></i></p> -->  

* * *

## Week 8: {{ site.week-08 }}  
<!-- ### JavaScript + Python: For Loops   -->

### [Week 8 Quiz](https://forms.gle/h5XMi7Gy1UDLAGta6){:target="_blank"}  


* * *

## Week 9: {{ site.week-09 }}  
<!-- ### Javascript + Python: Function Definitions + Function Calls -->

* * *

## Week 10: {{ site.week-10 }}  
<!-- ### Introduction to Python Data Visualization + Mapping -->
<!-- ### Review Week   -->

* * *

## Week 11: {{ site.week-11 }}  
<!-- ### Javascript + Python: More Kinds of Loops    -->


* * *

## Week 12: {{ site.week-12 }}  
<!-- ### HTML/CSS: Introduction   -->

* * *

## Week 13: {{ site.week-13 }}  
<!-- ### HTML/CSS: Drawing on Web Pages (Using JavaScript + HTML Canvas) -->


* * *

## Week 14: {{ site.week-14 }}  
<!-- ### _GitHub Pages_, Advanced Web Design + Layout -->

* * *

## Week 15: {{ site.week-15 }}  
<!-- ### Complete + Present Final Assignments -->

* * *

## Week 16: {{ site.week-16 }}  
<!-- ### Complete + Present Final Assignments -->

* * *

## Week 17: {{ site.week-17 }}  
<!-- ### Complete + Present Final Assignments -->

* * *

