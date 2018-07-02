---
title: Here Comes Dr Jekyll
layout: post
category: Incubation
hero:
  gradient_corner: bottom
  gradient_color_1: '0,0,0,.5'
  gradient_color_2: '0,0,0,.2'
  full_screen: false
  gradient_side: ''
  image: "/uploads/test-tubes.jpg"
date: 2018-07-02 00:00:00 +0000
excerpt: How the new website was created
author: Tim Klapdor
tags:
- website
- jekyll
categories: Updates
---
For more than 3 years the uImagine website has been running on \[Wordpress\]([https://wordpress.org/](https://wordpress.org/ "https://wordpress.org/")). During that time there have been a few glitches, dodgy plugins, redos and a few unexplainable cases of weirdness that seem to resolve themselves in an hour or so. Oh and about a million security patches and updates. Wordpress is a fantastic platform, plastic in ways that no other web tool is, but at the same I’m finding it overkill for a lot of recent projects. Most of the time what we need isn’t a dynamic way of engaging with a huge page, but a simple stable way of navigating publisher information. I’m a front end guy, HTML and CSS are my cup of tea, so a lack of PHP skills has always hampered what I can personally do with Wordpress. I’ve been reliant on other people’s plugins to do relatively simple things, and that has created a few dependencies that don’t  make me very happy. 

One of the features I relied on too much was the page builder plugin built into the theme we used. I chose the theme because it did 99% of what I wanted, but a lot of that was achieved by using a page builder plugin. That was great initially - it was simple to create the layouts that I wanted pretty quickly and painlessly. But after one update to the plugin it rendered a heap of content  riddled with errors and required manual updates on every page. Editing the content wasn’t a simple process, pages were no longer a single content area with HTML, there were blocks and meta data everywhere, all which needed to be clicked and edited and saved. This made the task an onerous one and it finally dawned on me that it also meant migrating to a new theme, or to have a site without this particular page builder was virtually impossible. 

It’s at this point the issue of just how much maintenance was required to keep this site up and alive kicked in. It’s constant, and rightfully so because the security threat  and incidents of hacking keep on growing. However, this site doesn’t contain any secrets or private information. Nor did it really require a huge database, nor the various JS and CSS frameworks that made thing look pretty and buttons function. Recently the sites performance has started to slow down and I took that as a sign that something had to be done. 

I’ve been working with \[Jekyll\]([https://jekyllrb.com/](https://jekyllrb.com/ "https://jekyllrb.com/")) for a few years now. I’ve used it to build a range of sites now from a \[Resume Builder\]([https://github.com/timklapdor/resume-builder](https://github.com/timklapdor/resume-builder "https://github.com/timklapdor/resume-builder")), a \[podcasting tool\]([https://github.com/timklapdor/link-rot](https://github.com/timklapdor/link-rot "https://github.com/timklapdor/link-rot")) and our \[Online Learning Exchange\]([http://uimagine.edu.au/csulx/](http://uimagine.edu.au/csulx/ "http://uimagine.edu.au/csulx/")). I love the simplicity of this new wave of \[Static Site Generators\]([https://www.staticgen.com/](https://www.staticgen.com/ "https://www.staticgen.com/")), mainly because they remove a lot of the server, security and database issues that come with Wordpress. I've even written \[a whole blog post on using them\]([https://timklapdor.wordpress.com/2016/08/20/the-dynamics-of-static-sites/](https://timklapdor.wordpress.com/2016/08/20/the-dynamics-of-static-sites/ "https://timklapdor.wordpress.com/2016/08/20/the-dynamics-of-static-sites/")) before.  

Static Site Generators are incredibly flexible and speedy, and \*\*for novice users completely impenetrable and impossible to use\*\*.  

That’s right, there’s a big downside to Jekyll, which is its huge learning curve to get up and running. To get started you’ll need to open the actual terminal (how 1980s), type into the command line to install stuff, create sites, run servers and build sites. You’ll have to learn \[Liquid\]([https://shopify.github.io/liquid/](https://shopify.github.io/liquid/ "https://shopify.github.io/liquid/")) templating and \[YAML\]([http://yaml.org/](http://yaml.org/ "http://yaml.org/")) and write everything in \[Markdown\]([https://daringfireball.net/projects/markdown/syntax](https://daringfireball.net/projects/markdown/syntax "https://daringfireball.net/projects/markdown/syntax")). Authoring and editing happens in a text editor, no lovely GUI here, and with one small error or spelling mistake you can break your site and stop it from publishing. 

>The biggest problem with most Static Site Generators is that aren’t suitable for beginners. 

In the past this has meant that I need to do everything - but this creates it’s own bottlenecks and issues. It also hampers collaboration. I was able to get around that bit by using GitHub but that was another technical leap for many users. So when \[Forestry\]([https://forestry.io/docs/editing/menus/](https://forestry.io/docs/editing/menus/ "https://forestry.io/docs/editing/menus/")) came onto my radar I was keen to explore it. Forestry provides a familiar CMS (content management systsem) interface for Jekyll sites. It gives you rich text editors and powerful ways to configure your \[YAML\]([http://yaml.org/](http://yaml.org/ "http://yaml.org/"))) metadata system that makes it easy for users to engage with. 

!\[Forestry - Static Site CMS\]({{ site.baseurl }}/uploads/forestry-compressor.png)

Forestry provides the missing link for static site generators - a simple to use User Interface. Yes there are still technical aspects to the initial build of a site, but in terms of collaboration and getting non-technical people on board it's a game changer. Going back to having a Web Developer developing the site itself, using the skills of the trade rather than a reliance on pre-made templates and themes, is a great thing. 

The uImagine website is now running on this stack:

1\. Jekyll is the underlying technology for the site. 

2\. Pages are built using a custom HTML and CSS. Layouts take advantage of CSS Grid and Flexbox.

2\. All content is written in Markdown.

3\. YAML metadata is used extensively to provide customisation and to link pages and data together

4\. Jekyll \[Collections\]([https://jekyllrb.com/docs/collections/](https://jekyllrb.com/docs/collections/ "https://jekyllrb.com/docs/collections/")) are used for \[Projects\]({{ site.baseurl }}/projects), \[Events\]({{ site.baseurl }}/events) and the \[Team\]({{ site.baseurl }}/about.html#team) areas.

5\. \[Data Files\]([https://jekyllrb.com/docs/datafiles/](https://jekyllrb.com/docs/datafiles/ "https://jekyllrb.com/docs/datafiles/")) are used to populate the \[Publications\]({{ site.baseurl }}/publications) and \[Presentations\]({{ site.baseurl }}/presentations) areas.

6\. A vanilla version of \[Isotope\]([https://isotope.metafizzy.co/](https://isotope.metafizzy.co/ "https://isotope.metafizzy.co/")) is used for the filtering of \[Projects\]({{ site.baseurl }}/projects) and \[Events\]({{ site.baseurl }}/events). 

7\. \[GitHub\]([https://github.com/timklapdor/uimagine-website/](https://github.com/timklapdor/uimagine-website/ "https://github.com/timklapdor/uimagine-website/")) is used to manage the project, site build and version controls. 

8\. \[Forestry\]([https://forestry.io](https://forestry.io "https://forestry.io")) is linked to that GiHub repository and provides the User Interface for other members of the team to contribute the sites content. 

9\. Forestry also takes care of the build and FTP of the site to the uImagine Server, hosted by \[Reclaim Hosting\]([https://reclaimhosting.com/](https://reclaimhosting.com/ "https://reclaimhosting.com/")).

This site is very much a work in progress. I need to add in a search facility to the site, so I'm looking at a few options for that. But overall I'm very happy with how things have progressed. The site is fast, stable and the overhead for getting others involved in running and contributing to the site is very low.

---

"E. coli GFP" flickr photo by \[Kitkor\]([https://flickr.com/photos/kitkor/5512961783](https://flickr.com/photos/kitkor/5512961783 "https://flickr.com/photos/kitkor/5512961783")) shared under a Creative Commons (BY) license