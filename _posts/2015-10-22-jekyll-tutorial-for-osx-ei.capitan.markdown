---
layout: post
title:  "Jekyll Tutorial For OS X EI.Capitan"
date:   2015-10-2 14:24:58 +0800
remark: Jekyll Tutorial
author: Andrew Wu
categories: jekyll
permalink: /post/
---

Before installation, you need to make sure your `usr/local/bin` is in you $PATH, if not, execute the following command in you terminal:
{% highlight ruby %}
export PATH=$PATH:/usr/local/sbin
{% endhighlight %}

And to avoid any sort of this access issue, when you install `jekyll`, use `sudo` command like:
{% highlight ruby %}
$  sudo gem install jekyll
{% endhighlight %}

Then, you might encounter this problem when you tried to install jekyll:
{% highlight ruby %}
$ sudo gem install jekyll
...
...
...
Building native extensions. This could take a while...
ERROR: Error installing jekyll:
ERROR: Failed to build gem native extension.
{% endhighlight %}

To solve this issue, you need the command line tools, simple enter `GCC` in the terminal, and it will pop up a alert for you to install that command line tools:
{% highlight ruby %}
$ gcc
{% endhighlight %}

Now, congrats! You are done with the installation. And next, follow the documents on the jekyll website to create your own blog!
{% highlight ruby %}
$ mkdir MyBlog                   //create a folder for your site
$ cd Myblog                      //point to the folder where you want to put the files
$ jekyll new                     //command to ask jekyll to build a blog 
$ jekyll serve --watch           //now go to localhost:4000 and see what happened, --watch allows the auto-generation to your browser
{% endhighlight %}


And for further information, like you want to figure out the file structure and explore what can be done, please check out the [Jekyll docs][jekyll-docs] on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
