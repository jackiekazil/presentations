# How running from zombies is the same as market behaviors

By Jacqueline Kazil

PyTennessee, February 9, 2018

----

![Izzy in Python Onesie](../media/izzy_in_python_onesie.jpg) <!-- .element width="80%" -->

Note:
- I do a lot in the Python community.
- I will use this photo forever.

Before I get into my main part of my talk, there are two items of housekeeping.

----

## Python Software Foundation

https://www.python.org/psf/

* The PSF protects the Python trademark
* Gives out grants to support Python events and Python development
* Organizes and hosts PyCon US
* Provides fiscal sponsorship support

& Much much more <!-- .element: class="align_left" -->


----

## Education Request for Ideas

http://bit.ly/PSF-RFI-EDU

How to increase Python presence in education?

* Really open ended
* Small or big - $10 to > $10 million
* Deadline Feb 18

Note:
- PSF Board Committee for Python in Education is looking for ideas...
- ...how the PSF can help members of our community increase the presence of Python in education.
- After we collect ideas, if we think something is exciting, we will come back and request a proposal.

----

## PyCon 2019: Cleveland, OH

https://us.pycon.org/2019/

* Tutorials: May 1-2
* Talks & events: May 3-5
* Sprints: May 6-9

..and PyCon 2020: Pittsburgh, PA


Note:
- Cleveland is a short non-stop flight from Nashville.
- You should stay for sprints - get experience.
- PyCon will probably move West
- PyCon brings me to mention the Maintainers summit

----

## PyCon: Maintainers Summit

http://bit.ly/maintain2019
https://www.papercall.io/pycon-maintainers-summit

* First year thru hatchery program
* Discussion of tooling, community, funding, and sustainability
* CFP open until March 15 for lightening talks

Note:
* The vast majority of libraries that exist have a fragile number of maintainers.
* In August 2017, all active Mesa core members fell off the face of the earth.

----

## Things I just mentioned

* Python Software Foundation (PSF)
* PSF Education Request for Ideas (Feb 18)
* PyCon 2019: Cleveland, OH (May 1 to 9)
* Maintainers Summit & CFP (March 15)


Note:

If you have questions about any of these things, please don't
And now for the regular scheduled talk...

----

## The Real Talk

... modeling the complex world we live in.

part tech talk, but also

part rethinking how you see the world.


Note:
* I tried to pick something everyone can enjoy.
* part data science, part tooling, part rethinking how you see the world.
* I hope you all get something from this talk.


----

![Cartoon of Jackie graduating with PhD](../media/phd2020.png) <!-- .element width="80%" -->


Note:
* Why listen to me? I am partically an expert
* Hoping to finish by 2020.
* Some of the work that I mention today IS my PhD
* At work, I model our IT infastructure and app interactions and dependencies

----

## Overview of today's talk

* Introduction to complexity systems
* What is complexity science or the study of complex systems
* Considerations for building models
* Some of the practical applications



Note:
What I hope you will learn in this talk...
1. A general understanding of the practical application
2. Some might dig into the tools
3. If nothing else, u learn how to survive a Zombie attack

----

## Tooling

* Mesa (Python) - Agent-based modeling
* Networkx (Python) - Network/graph analysis
* Netlogo (Logo) - Agent-based modeling

Note:
* Just in case you want to play around with some of the tools while I talk
* Mention examples

----

## "Your watch is complicated, your family is complex"

Said by David Krakauer, Evolutionary Biologist

Note:
* A watch is predictable, a family is not
* The mechanisms in watch are perfectly rational
* I know my family is not
* Love you all!

But what does this mean?

----

![](../media/complexity_policy_book.png) <!-- .element width="40%" -->


Note:
* Roland Kuper highlights a model in his book
* ... which tests the impact of adaptive cruise control on road capacity
* Who here is from a place with terrible traffic? (you are going to love this)
* If 100% of new cars had adaptive cruise control..
* .. how much would road capacity increase in 1 year?
* 30%


----

## Traffic in Ethiopia
[![Ethiopian traffic](../media/traffic_shot.png) <!-- .element width="80%" -->](https://youtu.be/UEIn8GJIg0E?t=22 "ethiopian_traffic")

Note:
* This is an intersection in Ethiopia.
* It has no traffic lights. So, how does it work?
* Flocking.  (Describe the behavior and individual decisions.)



----

## Birds flocking

[![](../media/flocking.png)<!-- .element width="80%" -->](http://www.youtube.com/watch?v=bb9ZTbYGRdc "")

Note:
* Each bird is following the leader or their neighbor
* In some ways this systems are completely different
* But in others they are not


----


![](../media/complex_systems_organizational_map.jpg) <!-- .element width="65%" -->


Note:
* "Complex systems" means a lot
* It even encompasses Machine Learning

Source: https://en.wikipedia.org/wiki/File:Complex_systems_organizational_map.jpg

----

![](../media/map_of_complexity_science.png) <!-- .element width="100%" style="max-width: 150%;"-->

2018 Map of Complexity Sciences by Brian Castellani


Note:
* You can see how the science changed over time.
* Started in 1960s/1970s.
* Since then computational power has improved and so has software.
* I can't cover everything, so I am going to focus on two areas

Source: http://www.art-sciencefactory.com/complexity-map_feb09.html

----

## Agent-based models

![](../media/map_abms.png) <!-- .element width="100%" style="max-width: 150%;"-->


Note:
* Thomas Schelling built one of the easiest and well know models.
* Segregated neighborhoods can arise not just by active racism
* but also due to a mild preference for neighbors of the same ethnicity
* Rob Axtell (GMU) did a lot of work in economics modeling

Source: http://www.art-sciencefactory.com/complexity-map_feb09.html


----

## What is agent-based modeling?

ABMs, MAS, Game theory, Cellular automata, Microsimulation, Individual-based models. Complex Simulations...

Note:
* ABMs go by many names
* MAS related - Focused on solution, not simulation.
* Game theory: related, but we want less than perfectly rational agents, no closed-form solutions.
* CA: subset of ABM
* Microsim: used in GIS to mean ABM
* Individual: ABMs are called in ecologywhat ABM are sometimes called in ecology.

----


## What is agent-based modeling?

Computer simulation <!-- .element: class="align_left pad_l" -->

Consisting of agents <!-- .element: class="align_left pad_l" -->

... interacting with one another <!-- .element: class="align_left pad_l" -->

... in order to study an overall system <!-- .element: class="align_left pad_l" -->


----

## Components of a model

Space <!-- .element: class="align_left pad_l" -->

Agents <!-- .element: class="align_left pad_l" -->

Time <!-- .element: class="align_left pad_l" -->

Visualization (not required) <!-- .element: class="align_left pad_l" -->


Note:
* Models have space, agents, time, and possibly a visualization element,
* You can run headlesss, especially when you are doing parameter sweeps.


----

## Conway's game of life

![](../media/conway.gif) <!-- .element width="75%"-->


Note:
* You could say this is an ABM in its simplest form
* These shapes are not agents, but each cell is one.
* Rule: Cells live or die based on the number of cells around them
* Early example where individual rules give rise to emergent behaviors

Let’s look at another tool - network libraries

Source:
https://en.wikipedia.org/wiki/Conway's_Game_of_Life#/media/File:Gospers_glider_gun.gif


----


## Networks

![](../media/map_network_science.png) <!-- .element width="100%" style="max-width: 150%;"-->


Note:
* Two names to note here...
* Duncan Watts - Small Worlds
* Albert-Lazio Barabasi - Scale free networks
* Both have written very accessible / easy reads on networks

Source: http://www.art-sciencefactory.com/complexity-map_feb09.html

----

## General Network types

![](../media/network_types.png) <!-- .element width="100%"-->

Source: Huang, Chung-Yuan, Sun, Chuen-Tsai and Lin, Hsun-Cheng (2005).

Note:
* Small-world - 6 degrees of separation
* Stanley Milgram experiment 1969
* Milgram is also known for shocking obience experiments like you may have see in Ghost busters
* Kevin Bacon
* Scale free - internet; rich get richer


Source: Huang, Chung-Yuan, Sun, Chuen-Tsai and Lin, Hsun-Cheng (2005). 'Influence of Local Information on Social Simulations in Small-World Network Models'. Journal of Artificial Societies and Social Simulation 8(4)8 <http://jasss.soc.surrey.ac.uk/8/4/8.html>.


----

![](../media/networks_sf_powerlaw.png) <!-- .element width="85%"-->


Note:
* Scale free follow power law distribution
* Many have one connection, few have many


Barabasi, A. L. (2003). Linked: How everything is connected to everything else and what it means.

----

# Modeling

# "the right thing"

Note:
* The world is big. How do you know what to include in your model? That depends.
* Take my example of modeling applications - deployment on hot chicken Tuesday
* Do we need to model Hot Chicken Tuesday?


----

## Segregation Model

![](../media/mc1.png) <!-- .element width="125%"-->


Note:
* classic model from 1971
* Agents can be happy or sad based on their neighbors (javascript)
* This adds a level of agency above the game of life --
* the agent moves to another cell
* Small individual bias can lead to large collective bias.


----


## Predator-Prey Dynamics

![](../media/mc2.png) <!-- .element width="115%"-->


Note:
*  Ecological model
* Sheep eat grass, Wolf eat sheep, Both reproduce
* This adds interactions with environment

Source: Wilensky, U. (1997). NetLogo Wolf Sheep Predation model. http://ccl.northwestern.edu/netlogo/models/WolfSheepPredation. Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.


----


## Political Dynamics

![](../media/mc3.png) <!-- .element width="85%"-->


Note:
* Agents aren’t individual people or animals
* They are simulated states that interact and fight
* Repast -- JAVA w/ custom IDE



----

## Migration Modeling

![](../media/mc4.png) <!-- .element width="85%"-->


Note:
* Simulation of displaced people flows in East Africa
* using real-world environmental, conflict and road network data.
* Example takes us from simulated worlds to the real world
* Real life simulation
* This is MASON - JAVA

http://socialcomplexity.gmu.edu/projects/easternafrica/

----


## Epidemiological Simulation

![](../media/mc5.png) <!-- .element width="125%"-->


Note:
* Isn't hypothetical, actually used by CDC
* Model from Los Alamos National Lab
* This is a 1:1 model
* Infectious disease simulation using census data, clinic locations, etc.
* Hand coded

----

## Demos


* Predator-Prey Dynamics in Netlogo
* Schelling in NetLogo
* [Schelling by Ncase](https://ncase.me/polygons/)

----

## Modeling on the front-end

* Parable of the Polygons (Javascript) - [ncase.me/polygons](ncase.me/polygons)
* Agent Base (Javascript) - [bit.ly/abm-ants](bit.ly/abm-ants)
* Agent Script (CoffeeScript) - [agentscript.org](agentscript.org)

----

## Modeling on the back-end

* NetLogo (Logo), 1999 - [bit.ly/abm-netlogo](bit.ly/abm-netlogo)
* MASON (Java), 2003 - [bit.ly/abm-mason](bit.ly/abm-mason)
* RePast (Java), 2006 - [bit.ly/abm-repast](bit.ly/abm-repast)
* Mesa (Python), 2015 - [bit.ly/abm-mesa](bit.ly/abm-mesa)


Note:
* Guido Darpa grant 2001
* In the grant - Logo, was nice, but we are done with it.
* Netlogo was pulling a Madonna

----

## Chesterton's Fence


![](../media/fence.jpg) <!-- .element width="55%"-->

Source: [Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Chesterton%27s_fence)


Note:
* Reference to  G. K. Chesterton's 1929 book The Thing.
* If you are going to delete or overrid something, you should understand it first
* And aknowledge it is no longer valid

----

## Python Research

![](../media/python_research.png) <!-- .element width="100%"-->

Note:
* There was nothing that existed when we got started.
* There seemed to a problem of libraries belonging to one person and dying
* Indra started the same time we did.


----

## Demo of Models

* Docs: [bit.ly/abm-mesa](bit.ly/abm-mesa)
* Code: [github.com/projectmesa/mesa](bit.ly/abm-mesa)

Note:
* Let's look at some models!


----

## How to run Demos

You install the requirements for that model

```
$ pip install -r requirements.txt
```

```
mesa runserver
```

Browser opens to http://127.0.0.1:8521/


Note:
* Runserver - just like Django
* We used port 8521, because 8888 is used for jupyter notebooks
* Zipcode in AZ

----

![](../media/mesa_diagram.png) <!-- .element width="70%"-->

Source: Masad and Kazil (2015).

Note:
* Model has a scheduler and space
* The scheduler activates the agent
* Viz server get data from Space
* Server generates Browser page & all modules on that page
* Batch Runner, as seen in the schelling example, allows for data sweeps
* Data collector, collects data to analyze later

Source: Masad, D., & Kazil, J. (2015). MESA: an agent-based modeling framework. In Proceedings of the 14th Python in Science Conference (SCIPY 2015) (pp. 53-60).


----

## Mesa's Scheduling Feature

![](../media/mesa_scheduling.png) <!-- .element width="70%"-->

Note:
* Notebook example & source: Prisoner’s dilemma
* Sequential activation, where agents are activated in the order they were added to the model
* Random activation, where they are activated in random order every step
* Simultaneous activation, simulating them all being activated simultaneously.
* Inspired by Kenneth Commer’s paper in 2014
* Consider your schedule works today when queueing up processes - system state

[Comer2014] Comer, Kenneth W. “Who Goes First? An Examination of the Impact of Activation on Outcome Behavior in AgentBased Models.” George Mason University, 2


----

## Mesa Packages

![](../media/mesa_packages.png) <!-- .element width="70%"-->

Note:

* Mesa functionality add - mesa-geo (not to be confused with GeoMesa)
* Agent & env based - econ-mesa
* Future goal is to have a whole ecosystem (like Django packages)
* People can mix and match schools of thought

----

![](../media/multilevel_mesa.png) <!-- .element width="80%"-->

Source: [Multi-Level Mesa](https://github.com/tpike3/ml_mesa)

Note:
* Most recently created by Tom Pike, a colleague at George Mason.
* It is in progress.
* ML_Mesa allows for holonic (Tom taught me that word) organization to models
* Neighborhoods, houses, families, people, etc


----

## Our goals with Mesa

* Framework for reuse
* Decoupled / decentralized
* Domain experts "own" components
* Reproducibility
* Building models on accepted truths

Note:
* Decouple - Django versus Flask
* Well established models would be well tested and turn into "accepted truths"
* ie We accept that the Request library is going to do what is does
* If it doesn't then we submit a ticket or PR


----

# So, how is running from zombies the same as market behaviors?


Note:
* You learned a little about the domain, practical examples, tooling...
* So, how is running from zombies the same as market behaviors?
* It is the logic and reasoning in the decisions with make
* Play neuron video
* Short answer: actors are looking to survive, rational versus irrational
* Long answer is in this books

----
![](../media/modeling_zombies.png) <!-- .element width="50%"-->


Note:
* This book is the long answer.
* I have a copy up front if you want to see it
* Yes, the author's real name is Robert Smith?


----


# The End.

Questions? <!-- .element: class="align_left pad_l" -->

@jackiekazil <!-- .element: class="align_left pad_l" -->

jackiekazil@gmail.com <!-- .element: class="align_left pad_l" -->

github.com/projectmesa/mesa <!-- .element: class="align_left pad_l" -->


