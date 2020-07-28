---
title: "Getting Started With Hugo"
date: 2020-07-22T14:48:33Z
---

So I've started building a new site here as a set of github pages. This has mainly involved playing with couple of site generators, and seeing how I get on with them. 

My motivation in this is pretty simple I need to get better at blogging. The tooling I use a a big contributing factor to that. So here are the requirements I've laid out:
1) Can be hosted using [GitHub Pages](https://pages.github.com/)
2) Is [JAMStack](https://jamstack.org/) based i.e. staticly generated markup fed by API's if required.
3) Posts can be written in markdown.

On the journey so far I've tried:
- [Jekyll](#jekyll)
- [Hugo](#hugo)

Now for the past 20 years I've pretty much solely developed in C#. So a move to Go or Ruby (even if it's only small bits) is big step. 

To help me get back up and running and to help others too I've put together a really simple tutorial to allow you to get started without install in ruby/jekyl or hugo. 
- [It's Alive, My Mr Hyde](tutorials/getting-running-with-jekyll) or getting started with Jekyll
- [I think I'm past the Hump](tutorials/getting-running-with-hugo) or getting started with Hugo

My impressions thus far are as follows, I love the speed owkring in both of these generators. 
Each has faily similar features with some unique benefits, however I need to select one so here my highlights:


## Jekyll
[Jekyll](https://jekyllrb.com/)
This ruby based generator has gained alot of traction. It is used extensively for githubpages even powering the main githubpages site.
### Templating
I really like the way that layouts are handled within Jekyll, the folder stucture feels similar to what I would have used years ago when hand cranking html sites.
I feels a little like going back to asp at times with the embeded code. 
At time the embedded code seems a little too much enven for simple task like a loop. That said this may come from my dislike of the Juby syntax rather than anything more inherent. 
### Performance
Given I'm not working with particulary large sites I was a little disappointed in the generator performance, it felt like we were gatheringa ALOT or unneccesary packages for a simple task. Granted my connections is not exactly stella at the moment but it still too a couple of mins to buid in a docker container. 
### Clarity
One way I'm assessing what I'm looking at there is how quickly I can adopt the tech and how readable the source code is. In this regard I find jekyll a little awkward. It is probably just the ammount of time I've spent working in ASP.net but there were a couple of points where it feels a little inconsistent.

## Hugo
[Hugo](https://gohugo.io/)
This Go based tool is pretty powerful. I was recommend it by [@sympodius](https://twitter.com/sympodius), which immediately says alot to me. Go is an interesting laguage so I'm intrigued to see how this works.

### Templating
Immediately, hgo puts me at eas with the way botht he templates and and the architypes provide consistent formatting. Having layouts live in the theme which is isolated from the site really helps with getting up to speed. Initially I wasn't sure what I through of including the template as a submodule, that sid I quite like the idea and it certainly helps to speed up the build time.

### Perfomance
As expected for anything written in go it is FAST. I really do mean fast where with other systems the dependencies take some time to intially load with Hugo it was immediate. 
Another small point to not is it was docker capable straight away, with the jekyll setup I had to provide a bunch of different options to the server to get automatic reloads to work, with Go this is the default configuration.
### Clarity
Overall I've found the hugo system fairly simple to get up and running. I especially appreciated the quick create templating with architypes. The folder structure makes a great deal of sense and well this site has been generated using hugo.

## Summary
I've tried 2 so far and I have to sayu I do likeboth of these generators though I've chosen for the moment to stick with Hugo. 
The next step will be a custom theme, and I'm sure I'll write about it as I go along.