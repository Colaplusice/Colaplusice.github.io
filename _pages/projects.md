---
layout: page
title: research
permalink: /projects/
description: research projects, still on building.
social: true
enable_katex: true
---
<!-- ### [Dada-driven control of redundant manipulators](manipulator_learning)

<a href="/tii"><img class="col one" src="/assets/img/projects/tii_laptop.png"/></a>

We focus on solving the control problem of robots from an optimizing  perspective. 
In some realistic scenenarios. The manipulator's structure imformation is not very explicit due to long-time using caused abrasion. In addition, for some homemade manipulators, it's hard to obtain its structure parameters such as DH parameters accurately. We propose a data-driven based method which do not involve the kinematic model of the manipulator.    [Read more …](manipulator_learning) -->

### [Learning-based task of manipulator to execute throwing task](MLP_learning)

<a href="/projects/MLP_learning"><img class="col one" src="/assets/img/projects/MLP_learning.jpg"/></a>
 We use the MLP to construct a learning neural network to execute a throwing task. The input of the neural network is a 13 dimension vector (4 for posture (quaternion) and 3 for position of the hand, and six for twist velocity of the throw action), and the outout is a 7 dimension vector. (landing position and orientation) [Read more …](MLP_learning)




### [Learning-based motion-force control scheme investigated on mobile manipulator](mobile_learning)

<a href="/projects/mobile_learning"><img class="col one" src="/assets/img/projects/mobile_learning.jpg"/></a>
 We investigate the learning algorithm on the mobile manipulator. [Read more …](mobile_learning)

<!-- 
### [Dada-driven control of redundant manipulators](manipulator_learning)

<a href="/tii"><img class="col one" src="/assets/img/projects/tii_laptop.png"/></a>

We focus on solving the control problem of robots from an optimizing  perspective. To be specific, the manipulator's 

In some realistic scenenarios. The manipulator's structure imformation is not very explicit due to long-time using caused abrasion. In addition, for some homemade manipulators, it's hard to obtain its structure parameters such as DH parameters accurately. We propose a data-driven based method which do not involve the kinematic model of the manipulator.    [Read more …](manipulator_learning) -->


<!--
**A bit of Text**

Some maths:

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

Some Code:


{% highlight python %}
def test(a=1):
  # Example can be run directly in your JavaScript console
  import numpy as np
  for i in range(5):
    a=[x.strip('.') for x in b{i}]
{% endhighlight %}

~~~py
def test(a=1):
  # Example can be run directly in your JavaScript console
  import numpy as np
  for i in range(5):
    a=[x.strip('.') for x in b{i}]

~~~


<div class="img_row">
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
</div>


<div class="col three caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/5.jpg" alt="" title="example image"/>
</div>


![image](/assets/img/12.jpg){:width='33%'}
<div class="col three caption">
    This image can also have a caption. It's like magic.
</div>

-->
<!--

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %} -->
