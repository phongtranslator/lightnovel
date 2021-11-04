---
title: Volume 4
layout: page
description: null
img: https://1.bp.blogspot.com/-nASpc7rFWZg/YYLYtOeqX2I/AAAAAAAACbY/j8ccklmhDk4gJx6_7h22agt9dYw3mXIWgCLcBGAsYHQ/s16000/IMG_0188.PNG
importance: 4
category: Nguyệt đạo dị giới
---
![](https://1.bp.blogspot.com/-nASpc7rFWZg/YYLYtOeqX2I/AAAAAAAACbY/j8ccklmhDk4gJx6_7h22agt9dYw3mXIWgCLcBGAsYHQ/s16000/IMG_0188.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-el3-rlAhqDU/YYL7TGMfJ4I/AAAAAAAACbo/ZHIoDKv6lioNTyiZRAXR6x1wlvjqANB6QCLcBGAsYHQ/s16000/IMG_0189.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-Aw1_tK6LF0g/YYL7TL2qClI/AAAAAAAACbk/5leGt_FdTqoVxgcz2thVDRM_m2w4zWvPwCLcBGAsYHQ/s16000/IMG_0201.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-xVOCSl5d0po/YYL7TCRgk-I/AAAAAAAACbg/O6ZItf8rZIgFgh9gTv2Ke_2vAVFVqn4kQCLcBGAsYHQ/s16000/IMG_0222.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-Wd9I_hj9Dbg/YYL7T5k_rTI/AAAAAAAACbs/6egNdwMH-BUxKSs87fI4u4EV7nUzFKr_gCLcBGAsYHQ/s16000/IMG_0235.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-WOp0whfQ_dE/YYL7UPYB2rI/AAAAAAAACbw/dOehVoJ0T-EFLNL175aeuq5tSywYraFowCLcBGAsYHQ/s16000/IMG_0277.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-YY0mSQteovY/YYL7UXmuGyI/AAAAAAAACb0/yoDSAFOlJ8cy7qqsLsoIkBoQNz--LaqsgCLcBGAsYHQ/s16000/IMG_0299.PNG){:class="img-fluid"}
![](https://1.bp.blogspot.com/-xMRrWsZR4ss/YYL7UykN59I/AAAAAAAACb4/J2dcMSrkakMosIwkfALlG56y8MpnpyRTACLcBGAsYHQ/s16000/IMG_0332.PNG){:class="img-fluid"}
<br />
<br />
<br />
<br />












Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/tsukimichi4.png
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/1.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/3.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/5.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/6.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% responsive_image path: assets/img/11.jpg title: "example image" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
