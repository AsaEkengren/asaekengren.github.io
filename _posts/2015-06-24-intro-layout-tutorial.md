---
layout: post
section-type: post
title: Modifying the Header
category: tech
tags: ["tutorial"]
---

The intro part of the index page (Header) is consisted of four elements:

<ol>
  <li>A black favicon</li>
  <li>Background image</li>
  <li>Welcome text</li>
  <li>Your image</li>
</ol>

### Black favicon

The black favicon is an image on the left of the navigation bar. Preferably it
should be a black and white version of your favicon.

```yaml
black-favicon: "/img/black-lab-glass.ico"
```

### Background image

In order to set the background, set the path to following variable:

```yaml
background-img: "../img/intro-bg.jpg"
```

<small>NB! Keep the .. in the beginning of the background image path</small>

### Welcome text

The welcome text is controlled by the following (self-explanatory) variables:

````yaml
dynamic-typing: True
shuffle: True # Shuffle the lines.
loop: True
loop-count: False # Set False for infinite loop, or set any number for finite loop.
type-speed: 10 # Default 10
start-delay: 200 # Default 200
delete-delay: 5000 # Default 5000
lines: # You can add HTML Tags in the Text
  - text: "The lower you fall, the higher you'll fly."
  - text: "Where’s your will to be weird?"
``

### Your image

You can set your image from the following variable:

```yaml
me-img: "/img/jetpacktocat.png"
````

If you want to connect your Facebook profile image then you can use the
following. Replace `user_id` with your facebook user id. Facebook user id can be
found by clicking on your profile pic and the large number in the end of the url
just before '&type' is your user id. Note: fbid is not the same as user id and
user id only contains numbers.

```yaml
me-img: "https://graph.facebook.com/user_id/picture?type=large&width=500&height=500"
```

If you want to connect your Github profile image then you can use the following.
Replace `user_name` with your Github user name.

<pre><code data-trim class="yaml">
me-img: "https://github.com/user_name.png?size=500"
</code></pre>

If you want to connect your Gravatar profile image then you can use the
following. Replace `email_hash` with your Gravatar profile email hash. You can
create the email hash by using an online tool like
[md5hashgenerator](http://www.md5hashgenerator.com/), just enter your email and
it will generate the hash.

<pre><code data-trim class="yaml">
me-img: "https://www.gravatar.com/avatar/email_hash?s=500"
</code></pre>

All set!
