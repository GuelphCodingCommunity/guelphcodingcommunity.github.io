README
======

Introduction
------------

[guelphcodingcommunity.github.io](https://github.com/GuelphCodingCommunity/guelphcodingcommunity.github.io)
is the source for the Guelph Coding Community's main website (hosted at GuelphCode.com).

It uses the awesome [Jekyll](http://jekyllrb.com/) gem to compile a static website out of basic
HTML, CSS, Javascript, and [Markdown](http://daringfireball.net/projects/markdown/syntax) files.

To host a copy of the website or test on your own machine please see [INSTALL.md](INSTALL.md)

Issues
------

Issues are tracked by the built-in issue tracking functionality of Github. 

If you believe that the site has a mistake, is missing a feature, or should have an enhancement, please raise it as an issue on the repository.

Contributing
------------

Members of the Github organization for the Guelph Coding Community have permission to merge pull requests and close issues. Contributors who are not a part of the organization can request approval or submit a pull request.

###Creating a new event

New events are written in [Markdown](http://daringfireball.net/projects/markdown/syntax) and are picked up on the [events](events.html) page automatically. A list of all events that are scheduled or have passed can be found in the [\_posts/events](_posts/events) folder. 

1. Create a new markdown file in the [\_posts/events](_posts/events) folder. The title should follow the naming scheme of **YEAR-MONTH-DAY-post-title.md**.
2. Add the [YAML frontmatter](http://jekyllrb.com/docs/frontmatter) to the beginning of the file. The specific frontmatter to include can be found in the [template](_posts/events/template.md) file. Specify the category as **event**, add any appropriate tags, and provide the **eventinfo** details.
3. Write the content for the event below the frontmatter.
4. You're done! Jekyll will automatically pull the info out of the file and compile everything to the right place.

###Creating a new blog post 

New blog posts are written in [Markdown](http://daringfireball.net/projects/markdown/syntax) and are picked up on the [news](news.html) page automatically. A list of all blog posts can be found in the [\_posts/news](_posts/news) folder. 

1. Create a new markdown file in the [\_posts/news](_posts/news) folder. The title should follow the naming scheme of **YEAR-MONTH-DAY-post-title.md**.
2. Add the [YAML frontmatter](http://jekyllrb.com/docs/frontmatter) to the beginning of the file. The specific frontmatter to include can be found in the [template](_posts/news/template.md) file. Specify the category as **news**, and add any appropriate tags.
3. Write the content for the blog post below the frontmatter.
4. You're done! Jekyll will automatically pull the info out of the file and compile everything to the right place.

###Changing styles

The style of the website is managed using [LESS](http://lesscss.org) in the [less/main.less](less/main.less) file. It is then compiled down to the linked css in [css/main.css](css/main.css).

Changing the style of an element should be done in LESS then compiled to CSS, and pushed *in the same commit*. This allows us to keep the LESS and CSS in sync. 

Including new styles (across all pages) can be done by adding to [\_includes/styles.html](_includes/styles.html). It is not currently possible to add styles for a single page.
