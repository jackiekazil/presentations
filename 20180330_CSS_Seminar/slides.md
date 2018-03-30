# Mesa, ABMs in Python 3

### Overview and
### dissertation proposal

By Jacqueline Kazil

CSS Friday Seminar, March 29, 2018

![](../images/mesa_logo.png) <!-- .element width="50px" -->


----

## Agenda

- Mesa - Overview and Live Demo
- Research questions
- Breakdown of work -- four papers
- Questions / discussion about Ph.D proposal
- *Brief discussion of Mesa packages*


Note:
The last part is brief stage setting to how Mesa Packages are proposed to work.
First, a little about me, CSS Student, PSF Board, Python programmer for > 10 years.

----

### Bias Warning

![Izzy in Python Onesie](../images/izzy_in_python_onesie.jpg) <!-- .element height="60%" width="60%" class="fragment" -->

Note:
- I fear an inheriant bias.
(Click to show Izzy)
- Explored various frameworks & languages over the years
- Taught/built curriculum for various languages
- I try to back my approach/decisions with data



----


### Bias Warning

![](../images/geoq.png) <!-- .element width="65%" -->

github.com/ngageoint/geoq

Note:
- PIF project -- My mission: disaster response and recovery.
- Evaluation process - Ruby versus Python
- Example: Coding cirriculum at work.
- How decision was made


----

### Mesa: History & Today


* Started in 2013 w/ David Masad and I
* Up to 45 contributors
* Meet monthly for dev meetings
* Current release 0.8.3 (soon to be 0.8.4)

----

![](../images/old_mesa.png) <!-- .element width="550px" -->


Note:
Early Mesa.

----

![](../images/mesa_today.png) <!-- .element width="660px" -->

(Mesa Demo)

Note:
- Now, instead of telling you about it, let me show you...

Afterwards...
- At the end of this talk, I will touch on a specific part of Mesa to transition into the next talk.

----

### Python growth and data science

- Guido van Rossum's Darpa Proposal (1999): "Computer Programming for Everybody."
    - Source: van Rossum, Guido. “Computer Programming for Everybody.” , July 1999, citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.123.6836&rep=rep1&type=pdf. <!-- .element style="font: 15px arial, sans-serif; font-color: #999999; padding: 15px" -->
- Python is the next big thing for [Insert domain] science.


Note:
- Next big thing in Science is a series of research.. every domain seems to claim it.
- ie Earth Sciences
- Scipy even has domain specific mini tracks
- Overall we have been pretty successful

----

![](../images/growth_major_languages-1-1400x1200.png) <!-- .element width="600px"-->

* Source: Robinson, David, et al. "The Incredible Growth of Python | Stack Overflow." Stack Overflow Blog, 4 Dec. 2017, stackoverflow.blog/2017/09/06/incredible-growth-python/.
<!-- .element style="font: 15px arial, sans-serif; font-color: #999999" -->

Note:
"wealthy countries (those defined as high-income by the World Bank) tend to visit a different set of technologies than the rest of the world."

----

![](../images/non_high_income_graph-1-1-1400x1000.png) <!-- .element width="600px"-->

* Source: Robinson, David, et al. "The Incredible Growth of Python | Stack Overflow." Stack Overflow Blog, 4 Dec. 2017, stackoverflow.blog/2017/09/06/incredible-growth-python/.
<!-- .element style="font: 15px arial, sans-serif; font-color: #999999" -->


Note:
But non-high income countries show a similar trend, but slightly different.
At PSF a large portion of our grant money goes to non-high income countries
Grant process grew largely in 2016 & 2017, when we scaled it up.
So, we haven't seen the effects yet.
We also have official Ambassadors in South America and soon in Africa.

----

### Research Questions

Theme one: Python and Open Source

- RQ 1: How can the Python programming language, which is rooted in open source, enable agent-based modeling to a wider audience?
- RQ 2: How does an ABM library in Python compare to the most popular ABM libraries used by researchers?

----

### Research Questions

Theme two: ABM in Python compared to other ABMs

- RQ 3: How have development patterns varied on agent-based libraries impacted the success or failure of those libraries?
- RQ 4: How do users want to use an ABM API? What are the expectations?

----

## Chesterton's Fence

![A fence](../images/fence.jpeg)

Note:
- Just because the fence doesn't have a clear purpose, work to understand it.
- First understand the historical context first - it can help you in the long run.
- Deploying is hard, because people are risk averse in government.
- Same reason for the cloud.
- "if it is not broken, then why fix it?"

----

### Breakdown of work -- four papers

* Comparison contribution patterns for Mesa, Netlogo, Mason, Swarm, Repast
* Mesa paper - architecture, features, sample projects...
* Mesa 1.0 - What do users want - locking the API
* Benchmarking Mesa, against other libraries


Note:
- The meat of the output will be 4 papers.
- Which we will discuss is more detail now.
- I know enough to be danagerous and to frame this work.
- Some areas I know more, but I am not "expert" yet.

----

### Paper: Comparison contribution patterns & culture

- Mesa, Netlogo, Mason, Swarm, Repast
- Popularity of... [framework, language] over time
- Commits, conversations, general activity, release cycles, etc.
- Conferences / Events? - Mesa has no formal ones, but what about Swarmfest?
- Where are they now?


Note:
- How to validate these five as THE ones to compare?
- Citations? What if there are multiple papers - ie Mason has 3.
- A project with little development != dead. It could mean stable?
- Development culture changed over time - comparison apples to apples?
        - ie CVS, SVN, Git

----

### Paper: Mesa

- aka 'the Mason paper' but for Mesa
- Why is Python a good idea? Why is it a bad idea?
- Architecture, features, sample projects, etc
- How we came up with the architecture
- What is the bus factor and how will work carry on?
- Mesa modularity and working with other libraries

----

![](../images/mesa_architecture.png) <!-- .element width="700px"-->

* Source: Masad, David, and Jacqueline Kazil. "MESA: an agent-based modeling framework." 14th PYTHON in Science Conference. 2015. <!-- .element style="font: 15px arial, sans-serif; font-color: #999999" -->



----

### Mesa 1.0

- The Mesa team discussed, "What is Mesa 1.0? / What does it mean to be 1.0?"
- Many possibilities came up for 1.0 -- like general housekeeping
- But what does it REALLY mean to be 1.0? <!-- .element class="fragment" -->
- 1.0 is an opportunity to breaking backwards capatibility <!-- .element class="fragment" -->
- It means being stable. <!-- .element class="fragment" -->


Note:
- Housekeeping
    - moving examples out and making sure they version match, Add bar charts
    - These are not hard
- But what does it mean to be one?

----

### Paper: Mesa 1.0, locking the API

- Talking to users about the good and bad of actually using Mesa.
- i.e. "When you tried to build a model, where did you start?"
- Yes... IRB. No... a survey only won't work
- Methods will be grounds in user-center design


Note:
I am going to spend a little more time on this one, since it might not be as clear.
(at the end)
- So why is this important?

----

![](../images/api_user_interface.png)


Note:
- The idea is to make the API as accessible as possible.
- Mesa is not Netlogo, but should it be?
- I don't know. I need to need talk to users.
- Are there minor things that I can fix to improve the experience?

----

![](../images/requests_example.png) <!-- .element width="1000px"-->


Note:
- This is the power of an API that was empathic to users.
- URLLib2 (Standard Python) versus Requests
- In doing user research, to try to get to this for Mesa -- should I also talk to users from the other libraries? That could get really big really fast.


----

### Paper: Benchmarking Mesa

- Looking at same projects in main libraries (i.e. Heat bugs)
- Validating Mesa: Can Mesa provide the same results?
- How does each library scale - 100, 1000, 100,000, 1,000,000
- What are key features that they have
    - i.e. How does Mesa's networks perform against other libraries.

Note:
- Moving on...
- What is important for bench marking?

----

## Any Pending Questions / Discussion

Note:
- Great! Now we can move to the bonus section!

----

## Mesa Ecosystem

- Individuals build complemenatary libraries for Mesa
- Libraries include rules for agents or world, minor logic or major features (ie GIS)
- Domain experts manage their respective domains
- Mesa core team might help or facilitate
- This is being documented by Tom Pike in Mesa docs

----

![](../images/external1.png) <!-- .element width="800px"-->

----

![](../images/external2.png) <!-- .element width="800px"-->

----

![](../images/external3.png) <!-- .element width="800px"-->

----

![](../images/external4.png) <!-- .element width="800px"-->

Note:
- What this looks like is still being worked out.
- 2 ways to intigrate
- 1. Pull in as attributes / logic
- 2. Create subclassed objects

----

# The End

## jackiekazil@gmail.com

![](../images/mesa_logo.png) <!-- .element width="400px" -->

Note:
- And with that, let's move to Econ-ark


