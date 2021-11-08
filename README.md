---
title: "Readme"
permalink: "/about/"
layout: page
---


* About me:"index.md"

* Revise the sidebar.html in include to change look of the sidebar

* Publications: "Publications.md"

* Project Portfolio: the markdown files in the "posts" folder. To turn off "read more", go to the includes folder, find home.html, delete the "<div ...read more..." line
    * Categories: accessibility, aibigdata, equity, resilience, transitnewmobility, travel behavior
    * To view all posts:https://jacobyan0.github.io/archive
    * detailed Jekyllrb guide on posts: https://jekyllrb.com/docs/posts/
    * Projects are organized by nav.html (in the includes and projects folders)
    * [Future] Make good use of excerpt_separator
      
    ![excerpt_separator](https://github.com/jacobyan0/jacobyan0.github.io/raw/master/images/Other/Excerpt_separator.png)

* Teaching: "teaching.md"

* Media: "Media.md"

* News: "News.md"

* Note1: Layout of all pages should be "page" except for posts
* Note2: all the content of a layout html is "included" when displayed the web page. So "layout" works more like "out-include" (i.e., content & include stuff in layout) and "includes" works more like "inner-include" (i.e., include stuff in include/xx.html file + other content of the html in development)


* Use Jekyllrb server for testing of web pages


### [Maybe useful later] Difference between page and post

* A post filename contains the title and the date of the post. An invalid date in the filename causes an error.

* Posts are comparable objects, which means two posts can be compared. The comparison is made by the post date and the post slugs.

* The generated default relative URL of a post and a page are different (e.g. /2000/01/01/my-post.html and /about.html).

* A page can be placed anywhere but a post can only be placed under _posts folder.

* A post has more data out of the box for use in Liquid templates (title, URL, date, id, categories, next, previous, tags, content).

* A post has a unique id.

* A post represents a blog post (so it is used to easily create a blog post). A page represents a website page.


### Acknowledgment: 
The website is built on the "constrast" theme forked from https://github.com/niklasbuschmann/contrast
