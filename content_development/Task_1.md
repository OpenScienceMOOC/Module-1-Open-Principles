---
output:
  html_document: default
  pdf_document: default
---
# Task 1: Defining how Open Science affects you

This task is designed for, well, everyone!

Estimated time to complete: 30-90 minutes.

Don't forget you can join in the discussions over at our open [**Slack channel**](https://openmooc-ers-slackin.herokuapp.com/). Please do introduce yourself at #module1principles, and tell us a bit about who you are, your background, and how you ended up here!


## Table of contents

* [Getting started up](#Getting_started)
* [Learning the basics of markdown syntax](#markdown)
* [Putting this into practice](#draft)
* [BONUS STEP](#bonus)


## Getting started up <a name="Getting_started"></a>

Welcome to your first task, probably, of the Open Science MOOC! What we *don't* want here is to create something where you sit in front of a screen, basically being lectured like you do at high school or university. We want you to create, to learn, to build, both as an individual and as part of a boundless community. We want to help you to sculpt your own path in research, and tell your own story and use that story to inspire and guide others.

In order to help this, we are going to try something that hasn't really been done before in this space. This [MOOC](https://opensciencemooc.eu/) is entirely built on a dynamic 'open source' process, with everything in the open and available to contribution from everyone. We would like you to be part of that.

During the tasks throughout the MOOC modules, we will help you, as a community, to directly create and edit content that becomes part of the overall course and its companion website. What you do from here on out will help to influence the learning of all individuals who come here in the future. Our job is to guide you in this process, and help you to realise that what you are doing is valuable, to yourself and others.

**IMPOSTER SYNDROME KLAXON**

Scholarly researchers represent the highest density of Imposter Syndrome that has ever been known to exist in the history of virtually anything, ever. [Jacquelyn Gill](https://twitter.com/JacquelynGill) wrote an excellent [post](https://contemplativemammoth.com/2012/04/25/how-i-cured-my-imposter-syndrome/) on this issue several years back now, and is well worth reading if you have a few minutes to spare before moving on.

> "While imposter syndrome can be alienating and the source of unhealthy emotional turmoil, I do think it’s worth drawing a clear line between feeling inadequate and recognizing areas for improvement. Being immobilized by anxiety because you don’t have a background in math is one thing; identifying a gap in your skill set and setting out to work on that is another. This takes time, a lot of self-reflection, and is best done with a good mentor or three." - Jacquelyn Gill.

We want to remind you at the beginning that if you find any part of this MOOC complicated, frustrating, or difficult, that is totally okay. The whole point of having this more of a peer-to-peer community is foster a culture of mutual understanding and learning so that we all grow together. The fact that you are here, demonstrating a willingness to learn more, is what is most important at this stage. We all have gaps in our knowledge and understanding, and this MOOC is just one small way to fill some of those gaps. So, we **thank you** for being here!

<br/>

## Learning the basics of markdown syntax <a name="markdown"></a>

A lot of people think [RStudio](https://www.rstudio.com/) (covered more in [Module 5](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/MAIN.md)) is just for writing complex scripts for statistical analysis. Wrooooong. It can also be used to write nicely formatted text documents, using something called [markdown](https://en.wikipedia.org/wiki/Markdown). Much of this MOOC was written in markdown in RStudio, and then converted from that into PDF, HTML, and Jupyter notebook formats, and look how nice it all looks!

Markdown is really a plain writing style that gives you full control over the format of text. If you're used to using something like Microsoft Word, it's kind of similar and gives you the same control over simple things like header style and text format. But in a way that is readable by more software, and can also be easily easily rendered as a webpage and many other useful output formats.

It is because markdown is so flexible in reading, writing, and conversion, that we are going to be learning a bit about it to get things started here. A collection of all things markdown-related can also be found [here](https://github.com/mundimark/awesome-markdown) for the adventurous types.

Here is just some of the basic markdown syntax that you might find handy for now (based largely on this [cheatsheet from Adam Pritchard](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)):

```markdown

  # Header one
  
  ## Header two
  
  ### Header three
  
  #### Header four
  
  Header with an underline
  ========================

  *one asterisk pair for italics*
  
  **two asterisk pairs for bold**
  
  1. For a numbered list
  2. Just use numbers
  3. Like this
  
  * For an unordered list
  * Just use asterisks
  * Like this
  
```
 
  # Header one
  
  ## Header two
  
  ### Header three
  
  #### Header four
  
  Header with an underline
  ========================

  *one asterisk pair for italics*
  
  **two asterisk pairs for bold**
  
  1. For a numbered list
  2. Just use numbers
  3. Like this
  
  * For an unordered list
  * Just use asterisks
  * Like this
  
For automatic links use [square brackets](https://www.google.com) and then insert the target URL in normal brackets after.

`[square brackets](https://www.google.com)`
  
For images, use an exclamation to indicate this and then a link to the image location:

`![image](https://github.com/OpenScienceMOOC/Module-1-Open-Principles/blob/master/content_development/images/logo.png)`
  
Some times you can also add in bits of HTML here if you want to be a bit fancier, which can help with display issues too some times:
  
<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-1-Open-Principles/blob/master/content_development/images/Logo.png?raw=true" width="500" /></p>

<p align="center"><i>The Open Science MOOC logo!</i></p>

```markdown
<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-1-Open-Principles/blob/master/content_development/images/Logo.png?raw=true" width="500" /></p>

<p align="center"><i>The Open Science MOOC logo!</i></p>
```
Some times, you might want to add in little snippets of code, like we have done above. For this, use simple back ticks, these little things: `

`some code with back-ticks around it`

For code blocks or chunks, you can use three back-ticks to indicate these:

```python
s = "Python syntax highlighting"
print s
```

Another handy point for highlighting text is to use block quotes, especially if you want to add a direct quote from someone (like we did for Jacquelyn above). For this, just use a right line break: >

`> This is a quote (Person, 2018)`

> This is a quote (Person, 2018)

For simplicity, line breaks are best added using the simple html code: `<br/>` as this helps to keep it much more visible where they are or need adding.

One of the last little things we might want to do is add tables, as these can look quite nifty in markdown. Let's sketch out a simple one here and see what it looks like.

```markdown

| Column 1     | Column 2      | Column 3  |
| -------------|:-------------:| ---------:|
| Tyrannosaurus| Meat          | Angry     |
| Velociraptor | Meat          | Relaxed   |
| Triceratops  | Veggiesaurus  | Hungry    |

```
Notice how the colons are used to align the text in the columns to either the centre or right hand side?

| Column 1     | Column 2      | Column 3  |
| -------------|:-------------:| ---------:|
| Tyrannosaurus| Meat          | Angry     |
| Velociraptor | Meat          | Relaxed   |
| Triceratops  | Veggiesaurus  | Hungry    |

<br/>

## Putting this into practise<a name="draft"></a>

Consider this task a bit like a mini research project to help increase your personal knowledge about Open Science. Here, what we are going to do is write a brief summary article about Open Science either about your research discipline and/or in your country.

We are going to use the simple markdown syntax we just learned about above here. For this, you can use a simple text editor like Notepad, or others that are a little more complex like [Atom](https://atom.io/), depending on whatever you are comfortable with.

As such, try and include a bit of formating variation in your work, including different headers, highlights, and maybe an image or two or a table. This will give you some nice experience using basic markdown while also doing some cool Open Science research.

There are several choices you have here for this part:

1. Write about the state of Open Access in your research community or lab group. This can include things like what proportion of articles are OA, whether there is an OA policy, or a summary of how your colleagues and you view OA. For this, it would be good to think about whether existing data are available, and if were they easy to acquire? Make  note of which sources you used, and whether you think these are appropriate to answer the questions.

2. Look at the status of Open Science in your research group or lab. Make a note of who is doing what, using what tools and services, and what their views are. What do you think could be improved?

3. Define clearly what Open Science means to you. Here, we want to make it a little challenging, by having a conversation about it with a colleague. Then, find someone from a different country, and have another conversation about Open Science. How do these view points all differ?

4. Time to investigate! Find out whether policies exist for your research group or institute regarding:

  * Career progression and assessment.

  * Publishing and Open Access.

  * Data sharing.

  * Intellectual Property (IP).
    
Write a brief summary for one of these, and about how it might influence your own research.

5. Identify any repositories for research articles or data for your discipline, as well as any tools and services that are widely used. Make a little table illustrating the key traits for these - you can decide what they are! (e.g., are they Open Source, are they owned by a for-profit company, are the data openly licensed etc.)

That's it! You can keep this as simple or detailed as you like, and depending on what information is available for you. If you don't like any of these options, feel free just to write something about your experiences as a researcher, and what drew you to be here.

<br/>

## BONUS STEP <a name="bonus"></a>

Hopefully, you just wrote something pretty awesome and useful, that you are proud of and want to share with others. I mean, after all that effort, why would you not want to? If you do want to do so, then let's make this a reality.

There are two ways to go about this. If you have an existing website or blog, post it there. That was easy!

For the second route, let's make this a real contribution to the main Open Science MOOC website!

Format your file like this:

`DD-MM-YYYY-your_name.md`

Replacing `your_name` with your_name. Your actual name.

Now, go to [this folder]() and upload your new blog post. Click 'Commit' and simply add a little message describing what you have done. For now, don't worry too much about using GitHub, as we address that in other modules.

What this will do is notify the people who are part of the core MOOC team that a new file has been uploaded. As soon as we 'accept' the new file, just like magic, it will automatically render [here] on the main Open Science MOOC website! How cool is that?

Now, all you have to do is share it. If you use Facebook, Twitter, LinkedIn, GooglePlus, Instagram or whatever, make sure to share your work widely. Let people know what Open Science means to you!

<br/>

## Checklist <a name="Checklist"></a>

Hopefully now, you will have a greater understanding of just some of the different ways in which Open Science influences you and your research. 

- [ ] You are now familiar with some basic markdown syntax and can use these to draft simple blog posts.
- [ ] You can now describe some of the Open Science policies that influence you, your colleagues, and your research discipline.
- [ ] You have written and shared a blog post illustrating this.

<br/>

**CONGRATULATIONS!** 

You have now help to upgrade your knowledge about Open Science, and have already shared this to help others learn too. 

From now on, it is all up to you! Some advice is to:

* Keep learning. Knowledge is power.
* Keep discussing these things with your colleagues, and develop a collective understanding of how Open Science influences you all in different ways.

<br/>

**Know a way this content can be improved?**

Time to take your new GitHub skills for a test-run! All content development primarily happens [here](https://github.com/OpenScienceMOOC/Module-1-Open-Principles/blob/master/content_development/Task_1.md). If you have a suggested improvement to the content, layout, or anything else, you can make it and then it will automatically become part of the MOOC content after verification from a moderator!

[![CC0 Public Domain Dedication](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
