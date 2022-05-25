---
layout: page
title: research
permalink: /projects/
description: research projects.
social: true
enable_katex: true
---
### Data-Driven Motion-Force Control Scheme for Redundant Manipulators: A Kinematic Perspective

<a href="sceneunderstanding"><img class="col one" src="/assets/img/projects/tii_laptop.png"/></a>
Redundant manipulators play a critical role in industry and academia, which can be controlled from the kinematic or dynamic perspective. The motion-force control of redundant manipulators is a core problem in robot control, especially for the task requiring keeping contact with objectives, such as cutting, polishing, deburring, etc. However, when a manipulator’s model structure is unknown, it is challenging to take motion-force control of redundant manipulators. This article proposes a data-driven-based motion-force control scheme, which solves the motion-force control problem from tshe kinematic perspective. The scheme can take effect and estimate the structure information, i.e., the model parameters involved in the forward kinematics when the structure of the manipulator is incomplete or unknown. A recurrent neural network is devised to find the solution to the scheme. Besides, the theoretical analysis is presented to prove the correctness of the scheme. Simulations and physical experiments running on seven degrees of freedom redundant manipulators illustrate the superb performance and practicability of the scheme intuitively. The key contribution of this article is that, for the first time, a motion-force control scheme aided with data-driven technology is proposed from a kinematic perspective for the redundant manipulators. [Read more …](tii)

### A Simultaneous Learning and Control Scheme for Redundant Manipulators With Physical Constraints on Decision Variable and Its Derivative

<a href="sceneunderstanding"><img class="col one" src="/assets/img/projects/tie_laptop.jpg"/></a>
In this article, a simultaneous learning and control scheme built on the joint velocity level with physical constraints on the decision variable and its derivative, i.e., joint angle, joint velocity, and joint acceleration constraints, is proposed for the redundant manipulator control. The scheme works when the structure parameters involved in the forward kinematics are unknown or implicit. The learning and control parts are incorporated simultaneously in the scheme, which is finally formulated as a quadratic programming problem solved by a devised recurrent neural network (RNN). The convergences of learning and control abilities of the RNN are proved theoretically. Simulations and physical experiments on a 7-degrees of freedom (DOFs) redundant manipulator show that, aided with the proposed scheme and the related RNN solver, a redundant manipulator with unknown structure parameters can perform a given inverse kinematics task with high accuracy while satisfying physical constraints on the decision variable and its derivative.
 [Read more …](tie)

### MKE Scheme for Planning and Control of Dual-arm Robotic System Aided with Recurrent Neural Networks

<a href="sceneunderstanding"><img class="col one" src="/assets/img/projects/ijcnn_pic.jpg"/></a>
Dual-arm robotic systems have great advantages over the single-arm robotic system, for the arms can either run independently or cooperate to finish the task. In this paper, minimum kinetic energy (MKE) is concerned as a performance index for the planning and control of a dual-arm robotic system. First, two sub schemes are formulated on the left arm and right arm of the robot, which are constructed on velocity level with consideration of manipulators' physical constraints. Then, the two sub schemes are unified into one scheme, which is finally transformed into a quadratic program (QP) problem. For solving the formulated QP problem, a recurrent neural network (RNN) is devised based on the Lagrange multiplier method. At last, the simulations and simulative experiments on a dual-arm redundant robotic system named Baxter are carried out. The simulation results reveal that the devised RNN model has a good performance for solving the presented MKE scheme applying to the dual-arm robotic system.
[Read more …](IJCNN)



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
