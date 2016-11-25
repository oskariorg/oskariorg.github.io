---
layout: post
title:  "Creating a blogpost"
date:   2016-11-22 09:22:48 +0200
categories: documentation
---
Create a new markdown file in `_posts` folder and name it following this format:  
`YEAR-MONTH-DAY-title.markdown`

# Writing blogpost:

Before you start writing you need to add:  
{% highlight text %}
---
layout: post  
title:  "Tested"  
date:   2016-11-23  
categories: test  
---  
{% endhighlight %}

in the beginning of your markdown file.  
Where  
`layout` is the html file you want to use in the `_layouts` folder.  
`title` is the title of your post.  
`date` is current date.  
`categories` is to which categories this post belongs to.  
`---` tells jekyll to use YAML's [**front matter**](https://jekyllrb.com/docs/frontmatter/) markup.

# Adding category:

If you want to create a new category which doesn't exist yet, you need to create a html-file in the `blog/categories` folder, ie `categoryname.html`

example file `test.html` for category test:
{% highlight text %}
---
group: blog
layout: category
title: test
description: All blogposts published under test
permalink: /blog/test/
category: test
---

{'%' include categories.html '%'}

{% endhighlight %}
`layout` is the html file you want to use in the `_layouts` folder.  
`title` is the title of your category.  
`description` is the description of your category.  
`permalink` is the link to the category in the browser.  
`category` is the current category when fetching posts.  
`{'%' include categories.html '%'}` includes the file which will show all posts in this category. Remove the `''` from the `%` signs.
