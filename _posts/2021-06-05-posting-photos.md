---
layout: post
title: "Posting photos"
date: 2021-06-05 12:00:00 +1000
categories: [development, photos]
tags: [jekyll]
excerpt_separator: <!--more-->
---

This post will show of the simplest ways, in my opinion, to include photos in a post. There are more sophisticated methods to create an image gallery on Jekyll, but these solutions seem require much more hacking around to get everything (plugins, HTML, CSS, Javascript, ...) to work properly (and then things always change!). So instead, we will have a look at this rudimentary but clean approach.

<div class="row">
    <div class="column3">
        <a href="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/coathanger.jpg">
            <img src="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/coathanger_thumbnail.jpg" alt="Coathanger" style="width:100%"/>
        </a>
        <figcaption style="text-align:center"><i>The beautiful Coathanger</i></figcaption>
    </div>
    <div class="column3">
        <a href="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/hong-kong.jpg">    
            <img src="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/hong-kong_thumbnail.jpg" alt="Hong Kong" style="width:100%"/>
        </a>
        <figcaption style="text-align:center"><i>Hong Kong from the Peak</i></figcaption>
    </div>
    <div class="column3">
        <a href="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/snowing-franklin.jpg">
            <img src="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/snowing-franklin_thumbnail.jpg" alt="Snowing Benjamin Franklin" style="width:100%"/>
        </a>
        <figcaption style="text-align:center"><i>Benjamin Franklin enjoying the snow</i></figcaption>
    </div>
</div>

<!--more-->

&nbsp;

So far, this method still looks pretty nice! The downside is that it requires more manual work, and so it would be unsuitable/impractical for actual galleries with much more content.

<div class="row">
    <div class="column2">
        <a href="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/bushwalk.jpg">
            <img src="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/bushwalk_thumbnail.jpg" alt="Bushwalk" style="width:100%"/>
        </a>
        <figcaption style="text-align:center"><i>The great bushwalk</i></figcaption>
    </div>
    <div class="column2">
        <a href="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/last-light.jpg">    
            <img src="{{ site.baseurl }}/assets/images/2021-06-05-posting-photos/last-light_thumbnail.jpg" alt="Last light" style="width:100%"/>
        </a>
        <figcaption style="text-align:center"><i>Last light</i></figcaption>
    </div>
</div>

