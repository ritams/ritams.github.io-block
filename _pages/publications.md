---
layout: archive
title: ""
permalink: /publications/
author_profile: true
---


Opinion Dynamics: Depolarization by Random Network Nudge
=======================

The study of opinion dynamics dates back to 1956 when French and John first formulated a basic model. After that many models of opinion dynamics have been proposed in the last few decades. Most notable ones are the voter model, majority rule model, and DeGroot's model. Though these models are good starting point in the study of opinion dynamics, the results from these models are not realistic. These models always lead to consensus in opinion. 
In this age of internet and social media, people now have more freedom in choosing whom they can interact with. It is human nature to interact with people similar to our own self, known as homophily. Many social media platforms take advantage of homophily by recommending connections between similar persons to make their platforms more engaging. Though there are a few advantages like increased engagement, aggressive personalized recommendation leads to echo chamber. In 2020 F. Baumann et al. proposed a model which includes all these subtleties.

Model
-----

**1. Activity Driven Modeling:** At every time step only active agents are allowed to interact with others and update their opinions.  From empirical data the distribution of activity of the agents is found to be a power law.
**2. Homophily:** This model incorporates homophily by introducing an interaction probability which decays as power law as the distance between opinions of two agents increases.

This model was successful in qualitatively capturing the real world features like polarization, radicalization,and consensus in opinion for different parameter values. This model also shows the agents who are more active,have strong opinions, agents and their neighbours who have similar opinions.

Depolarization
-------

The effect of echo chamber has become a major issue in today’s social media platforms, which also contributesto increasing polarization of opinions.  To mitigate echo chamber effect, we came up with an idea of nudgingthe people to form connections with random people.To implement this we modified the interaction probability such that an agent will form a connection with auniformly chosen random agent with a small probability $p$, and with probability $(1−p)$ it will form a connectionwith an agent chosen according to homophily probability

The small value ofpensures that the agents are connecting to similar people most of the time, and in themeantime they also form a few random connections to reduce the effect of echo chamber.

Results
----

With  this  modification  in  the  interaction  probability  we  are  successfully  able  to  achieve  depolarization  and have  significantly  reduced  the  effect  of  echo  chamber.   Depolarization  happens  gradually  as  we  increase  thenudge  probability $p$.   Though  relatively  large  value  of $p$ leads  to  radicalization,  for  a  large  enough  systemthe  depolarized  state  is  relatively  stable.   To  formally  address  this  issue  of  radicalization,  we  have  nudged a  fraction  of  the  population,  and  using  a  linear  cost  function  to  maximize  the  depolarization  and  minimize radicalization, we have found a numerical solutions for optimal fraction of population and nudge probability $p$.


Extreme Events
======

Extreme  events,  defined  as  the  events  whose  numerical  values  differ  significantly  from  the  values  of  typical events and exceeds a predefined threshold, are ubiquitous in natural or man made systems.  From earthquake,drought, flood to power black out and stock market crash, extreme events often disrupt the functionality of the system.  And due to this huge applicability in real world systems, extreme value statistics have gained a lot of interest among researchers.

Along with other questions researchers are often interested in the probability distribution of spacing $(S_i=\frac{E_{i+1}}{E_i})$  between  two  consecutive  extreme  events  and  the  probability  distribution  spacing  ratios  $(r_i=\fract{S_{i+1}}{S_i})$.Though for uncorrelated time series these probability distributions can be calculated analytically, obtaining an analytical expressions for these distribution in the case of correlated time series is difficult.  In 2008 Santhanamet al. have calculated an analytical expression for the spacing distribution which holds good for large spacing,but there is no such expression for the distribution of spacing ratios.

Spacing Ratio
---
Starting from a fractional Brownian motion (or fractional Ito motion) we are trying to obtain an analytical expression  for  the  probability  distribution  of  the  consecutive  spacing  ratio$(r_i)$.   From  extensive  numerical simulations we have found that at large ratio the probability distribution of spacing ratio behaves like a powerlaw, whose exponent depends both on the threshold and correlation exponent of the time series.

Thomae's Function
----
As the time series data points equispaced in time, the spacing between two extreme events is a integer multiple of a constant time interval,  hence the spacing ratios are rationals.  While using uniform binning to plot the distribution of spacing ratio we have noticed a fractal like behaviour near $r= 1$.  We have modified the definition of spacing ratio to be $( \tilde{r}_i=\frac{S_{i+1}}{S_i+S_{i+1}})$ such that  $\tilde{r}$ takes rational values from $(0,1)$.  Surprisingly, we find that the distribution resembles the Thomae’s function.  We are also trying to find out if there is any relation between the fractal dimension of the distribution and the correlation exponent of the time series.

