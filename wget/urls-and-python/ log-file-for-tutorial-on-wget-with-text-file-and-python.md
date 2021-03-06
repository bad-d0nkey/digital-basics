---
tutorial: wget-urls-and-python
date: 01-10-21
tags: digital_basics, wget
---

# what I was trying to do

tried to do the urls-via-different-methods thing with wget
+ tutorial: https://graddh.netlify.app/docs/tutorials/wget/#using-wget-with-a-list-of-urls
+ repo: `[wget](https://github.com/bad-d0nkey/digital-basics/tree/main/wget)`

## how it might connect to other research I'm doing

still not sure. i have heard it thrown around, so i know that it is useful. for what specifically (beyond "that it downloads stuff from the web") i'm still unclear. (that is, the scenario in which i would personally use this to collect the data i typically work with is unclear, but i can see potential.)

## what I did

#### using a list of urls
+ step 1: navigated to links in coursebook
	+ updated links, navigated to these links

+ step 2: made a .txt [with the url addresses](https://github.com/bad-d0nkey/digital-basics/blob/87e57adfc8a4d3c988655e94015c03231fb230f5/wget/urls-and-python/urls.txt), saved

+ step 3: entered the code w/ .exe added: `wget.exe -i urls.txt -r --no-parent -nd -w 2 --limit-rate=100k`
	+ this did not work. the following was returned
	+ googling and stackoverflowing ensued -> nothing quite matched 
![wget_error_urls](wget_error_urls.png)

+ step 4: tried making a directory, saving file to directory, following steps again
	+ this did not work. the same error (but with a different file path) was returned
	+ googled and stackoverflowed again -> results weren't better (wrong language, methinks)

+ step 5: took to discord, walked away
	+ the solutions offered weren't quite applicable (i don't have the vocabulary to clearly communicate, but i invariably get good prompts from my lovely cohort), but prompted me to start from the bottom with the data

+ step 6: manually typed the urls in a new file, confirmed they all worked, saved file to proper directory

+ step 7: passed the same argument (w/ .exe added) 
	+ this worked just fine. 
	
![itworked](itworked!.png)

+ step 8: hunt down ghost
	+ currently trying to hunt down the ghost in the machine - or file, really - through discord. i am noting that this is the fourth paste-related incident that has resulted in wonkiness. this is a pattern. and it is me-centric. 

#### using python to generate a list of urls

+ step 1: made a directory
	+ old hat at this now. was fine and fancy.

+ step 2: made a [.py file with the script](https://github.com/bad-d0nkey/digital-basics/blob/c20ed7ddf6dded3264aa23c51b789fec40b3d033/wget/urls-and-python/urls.py), saved it where it should go
	+ made sure to use an actual text editor -> i had forgotten to do so for "little things" and was having some problems (per above). this has fixed it.
+ step 3: followed through rest of tutorial
	+ .py flipped to a [.txt file](https://github.com/bad-d0nkey/digital-basics/blob/c20ed7ddf6dded3264aa23c51b789fec40b3d033/wget/urls-and-python/urls_python.txt), did the machinations
	+ checked [the folder](https://github.com/bad-d0nkey/digital-basics/wget/urls-and-python/war-diaries/)
 and all is dandy

## challenges 

forgetting to use a proper editor presented a challenge. the rest actually went surprisingly well. 

i still need to understand why i would use one prompt environment over another, or, if they do the same thing with slightly different approaches, maybe figure out which i prefer. i can't seem to articulate why i need to untangle this for myself - i'm not phrasing my questions correctly. so, i'm going to dig around a bit re: the different approaches to see why they're different and when one would use one over the other. i think that will make things more clear - and enable me to keep the right kinds of notes for the right kinds of approaches. 

## thoughts on where to go next

not sure until i figure out how other people have used this doing the kind of work i do. i am going to look at past projects and see where i had to make work-around decisions because i didn't have the right skills, then try to see where i can incorporate what i have learned (which will direct what else i need to learn as next steps)

## update

related to the other wget log update, which i probably should have put here instead, so i won't belabour the point here. i'm starting to be able to untangle things and get what i'm looking at when i look at the terminal. 

![yarn](yarn.PNG)

i even managed to add anaconda to my terminal viewer. ha-ha!

![anaconda added](anaconda.PNG)
