---
layout: post
title: "Add Google-plus Comments Box to Jekyll website"
description: "Add Good plus to your Jekyll Blog with the step-by-step tutorial"
author: "Ajinkya"
coverImg: "post-bg.jpg"

---

# Add Google-plus Comments Box to Jekyll website or any static page

This post shows how to step-by-step Add Google-plus Comments Box to Jekyll blog or to any static website. You can see the preview at bottom of this page. This website was build using Jekyll.

### Installation

If you are using Jekyll;


1) Create `comments.html` file inside your `_includes` folder with below code

{% highlight liquid %}
{% raw %}
  <script src="https://apis.google.com/js/plusone.js"></script>
  
  <div class="g-comments"
      data-href="{{site.baseurl}}{{page.url}}"
      data-width="642"
      data-first_party_property="BLOGGER"
      data-view_type="FILTERED_POSTMOD">
  </div>
{% endraw %}
{% endhighlight %}


2) Now just make sure you have this property defined in your `_config.yml` file (replace the url with your website URL) View my [soruce code here!](https://github.com/steelx/jekyll-blog/blob/gh-pages/_config.yml) 

{% highlight liquid %}
{% raw %}
  baseurl: http://jekyll-blog.com/
{% endraw %}
{% endhighlight %}


3) include `comments.html` wherever you wana display Google plus comments, preferably inside posts layout file.

{% highlight liquid %}
{% raw %}
  {% include comments.html %}
{% endraw %}
{% endhighlight %}

I hope this post was useful, please dont forget to Google PLUSONE this post or comment below.
Please view the source code on your live website pressing `CMD/CTRL+ U` to check the generated URL on your webpage after commiting the files. If this doesnt work post your comments below and I will be glad to help you.

