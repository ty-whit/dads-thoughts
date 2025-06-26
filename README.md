# Dad's Thoughts Blog

Welcome to the source code of my blog. All the writing for this is originall written in markdown. I've been using Obsidian for years at this point, and really appreciate the fact that it doesn't lock you into a file format, as I've jumped back and forth between Windows, MacOS, and Linux a lot over the last 10 years, and markdown works across all them. It does have it's short comings, so I have found myself utilizing other edits, like PyCharm and Visual studio code for some actual writing tasks as well as Obsidian. 

For years now, I've been wanting to actually publish a blog where I write about different games that I think that children should be playing. As dad who plays video games, I understand first hand what I want my kids engaging with and what I don't think they should be interacting with. For a deeper discussion on that topic, go check out the entry titled [Reason for this blog](https://ty-whit.github.io/dads-thoughts/Kids-Reviews/Motivation). 

While that was the original motivation for wanting to actually start posting things on the internet, I realized at about the same time that I wanted to be creating more positive content around masculinity and parenting. I was also finding videos talking about the indie we and making cases for making your own website. That's what this has ended up turning into. Instead of trying to sign up for something like [Neocities](https://neocities.org/), I figured I'd just go ahead and do the same thing using GitHub Pages, where I could use git and all the other processes that I'm already used to with work. Deciding 
## Basic setup

Full tutorial with screenshots & videos: https://dev.to/defenderofbasic/host-your-obsidian-notebook-on-github-pages-for-free-8l1. 

It's basically (1) fork this (2) go to repo's "Settings" > "Pages", Under "Build and Deployment" select GitHub Actions. Then go to "Actions" and enable GitHub actions for your fork. Edit the pages in [source/content](./source/content) with Obsidian or any text editor. It generates HTML using [Quartz](https://github.com/jackyzha0/quartz). To generate the HTML locally, run `npx quartz build --serve` in `./source/`

## Raw HTML pages

There is a [source/raw_html](./source/raw_html) folder that gets copied into the build folder in CI. This lets you host arbitrary HTML outside of quartz. Example: https://defenderofbasic.github.io/obsidian-quartz-template/raw-html-test.html

I made the "raw HTML" option for people who are generating HTML UI's with Claude/ChatGPT but want to tweak them/host them themselves. Or make a personal archive of web pages, etc.

## Further customization

> Quartz is meant to be extremely configurable, even if you don’t know any coding. Most of the configuration you should need can be done by just editing quartz.config.ts or changing the layout in quartz.layout.ts.

https://quartz.jzhao.xyz/configuration
