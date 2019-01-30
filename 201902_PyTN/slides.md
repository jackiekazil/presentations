# How running from zombies is the same as market behaviors

By Jacqueline Kazil

PyTennessee, February 9, 2018

Note:
-

----

![Izzy in Python Onesie](../media/izzy_in_python_onesie.jpg) <!-- .element width="80%" -->

Note:
About me...
- PSF, Python, Education, Finance, PyLadies Auction
- Me and complexity - how to got into it

----


# Overview of today's talk

* Introduction to complexity science by example
* How it fits in the ecosystem of data science
* What tools exist in Python
* Some of the practical applications

Note:
What I hope you will learn in this talk...
1. A general understanding of the practical application
2. Some might dig into the tools
3. If nothing else, u learn how to survive a Zombie attack


----

# Traffic example from Ethiopia
[![Ethiopian traffic](../media/ethiopian_traffic.jpg)](https://youtu.be/UEIn8GJIg0E?t=22 "ethiopian_traffic")<!-- .element width="200%" -->

Note:
Let's die right in.
This is an intersection in Ethiopia.
It has no traffic lights. So, how does it work?
Flocking.  (Describe the behavior and individual decisions.)

[//]: # ()


----

  <video>
    <source data-src="video.webm" type="video/webm" />
    <source data-src="video.mp4" type="video/mp4" />
  </video>



----








Zombie example:

Netlogo

Swarm example
Osccilliation example







![](../media/modeling_zombies.png) <!-- .element width="50%" -->

Note:
- Mathematical Modelling of Zombies by Robert Smith?
- Robert Smith? with a question mark, not the lead singer of the cure



----

Complexity quote...


"Your watch is complicated, your family is complex."
Great Krakauer, Santa Fe Institute



----


# PREVIOUS CONTENT ------- DELETE

OR

# How the government made me a better programer

By Jackie Kazil

Note:
- During this talk I will highlight a series of lessons.
- These can be used in gov OR in private sector


----

Tech in government has changed a lot...

.. and so have I. <!-- .element: class="fragment" -->

----

First, a little about myself...

- Worked in government from 2011 to 2015
- Presidential Innovation Fellow 2013 to 2014
- Python Software Foundation Board member
- PyLadies leader - internationally and in DC
- Board member of Byte Back
- PSF Fellow
- ... and other random things

Note:
Byte Back is an organization that teach basic digital literacy skills in order to
put individuals into living wage careers.

----

![](../images/book.png) <!-- .element width="40%" -->

----

# El Sentinel

![El Sentinel screenshot](../images/elsentinel.png) <!-- .element width="50%" -->

Note:
Trabajé como periodista para un periódico español en el sur de Florida.
Donde pretendo hablar español.

----

![Moved to DC](../images/movedtoDC.jpg)

Note:
I came to DC 10 years ago!
These heads are from the baseball team in DC

----

Things have changed a lot!

![Izzy in Python Onesie](../images/izzy_in_python_onesie.jpg) <!-- .element height="60%" width="60%" -->

Note:
Went from journalist to civil servant.
And had a baby.

----

![Library of Congress](../images/LOC.jpg) <!-- .element height="80%" width="80%" -->


loc.gov

Note:
- 2011 to 2013
- This is not where the great big change happen
- When I walked in, this was a well functioning team
- There were pockets of this in government
- Tech stack was Python, Django, & Postgres

----

The team worked on lots of important things...

----


![LOC is down](../images/locdown.png)

Note:
Like this one.

----

![LOC is down](../images/locdown.png)

Note:
And this one.

----

![LOC is down](../images/locdown.png)

Note:
And this one. This one is my favorite.

----

Lesson: If you are not on the cloud, you need to move, otherwise someone will take screenshots of your downed website and share it at a conference.

Note:
- This is why LOC is having these problems.
- The work doesn't matter as much I had the honor to work in the corner of government that was functioning well.
- However,...

----

Lesson: A team only functions as well as the environment in which it is run.

Note:
- Hence why you are seeing the projects ast they are today.
- If you don't give you people the proper tools, they can't do their job.

----

## Why wouldn't someone move to the cloud?

Note:
- Because they are afraid of risk
- & they have issues w/ buecracy
----

Managing data centers is hard. If that is not your business, pay someone else to do it for you.

----

If fact, deploying code is one of the hardest things to do in government.

It can take six months to more than a year.

Note:
- Why?
- Because if you don't deploy, then you won't have problems.
- It is easier to say 'no' than to say 'yes'

----

## Lesson: Chesterton's fence

![A fence](../images/fence.jpeg)

Note:
- Just because the fence doesn't have a clear purpose, work to understand it.
- First understand the historical context first - it can help you in the long run.
- Deploying is hard, because people are risk averse in government.
- Same reason for the cloud.
- "if it is not broken, then why fix it?"

----

Automated deployments to the cloud == less risk.

Note:
- Because if there is an issue, you can deploy a fix quickly

----

Many small deployments are less risky than one single, large deployment.

A - B < A - C

Note:
- Because the changes are incremental.
- The delta between A & B is less than A & C.
- Each change has less impact.

----

We can learn a lot about the way tech worked (or didn't work) through its devs and deployment processes.

----

### Regulation

Less regulation <--------------------------> More regulation

Note:
- Less regulation == Your cousin wins the contract
- More regulation == Your friend wins the contract, because they are the only ones who can navigate.
- Neither your cousin or your friend are experts in the work.
- Which means you end up with situations like...

----

![](../images/fema.png) <!-- .element width="75%" -->

Note:
- One person won this contract and hired a wedding company to make the meals.
- They made 50,000 out of 30 million that were required.
- Why would you hire a wedding cater & not someone who works in truly massive meal preparation

----

![](../images/hc.png)

healthcare.gov

Note:
- Slow, locks up users, drops them, bad data.
- This system requires special consideration, b/c secure data.
- 55 contractors -- all were confident in their system, but no end to end testing
- I don't know what happened, but I imagine somewhere I dev said... this is not going to work.

----

### Meanwhile...

----

![](../images/CFPB.png)

cfpb.gov

Note:
- While I was at LOC, the agency was started in 2011 in response to the financial crash of 2008 to protect consumers.
- They set an example for what tech should be like in government.
- However, they also had a clean slate.
- Much of their work was and is in Python!
- I almost went to work there in 2013, but didn't.

----

President Obama wanted to bring "Silicon Valley" entrepreneurs and engineers into government.

So, he appointed Todd Park as the second CTO of the U.S. in March 2012.


----

### Todd created the Presidential Innovation Fellows (PIF)

- Inspired by Code for America
- Short "tours of duty" to work on projects with the potential to save lives, money, create jobs, and make government more efficient
- There were 18 fellows in the first round, now...

Note:
- The purpose was to attract talent and try to get them to stay after they finished their "tour of duty"

----

![](../images/pif.png) <!-- .element width="75%" -->

presidentialinnovationfellows.gov

Note:
- 122 Fellows as of late Early 2018

----

Lesson: Create a fellowship and give the fellows lots of freedom and air cover to attract top talent.

----

Application due during PyCon 2013

Note:
- Heard about the PIF program during a happy hour from one of those 18.
- I wasn't going to submit, but the application was easy, so I did.
- I received 3 interviews, 2 offers

----

![](../images/thestreet.png) <!-- .element width="55%" -->

Note:
- Those two offers were across the street from each other.
- The good news is that if I wasn't happy at FEMA, Dept of education told me tos stop by on my home


----

Lesson: Do not *not* pursue an opportunity. Apply for anything that interests you.

Don't let imposter syndrome get in the way of your goals.

----

![](../images/geoq.png) <!-- .element width="65%" -->

github.com/ngageoint/geoq

Note:
- My mission: disaster response and recovery.
- Get money into the hands of people who need it.
- This project used in diasters in Moore, Oklahoma & Colorado Floods.
- But also internationally: Typhoon Maysak, Nepal Earthquake, Saipan - Typhoon Soudelor

----

Lesson: Rewrite versus build upon -- carefully consider your path and make sure you are not being biased.

Note:
- The project was originally written in Ruby -- but after a careful evaluation, it was best to rewrite in Django / Python.

----

### Meanwhile...

Note:
- As I was finishing my tour of duty, there was a group of folks looking to make the work that PIFs were doing more pernament, because one person for 6 months to one year wasn't enough.
- During its 2nd year, the PIFs was operationalized inside the G.S.A. and there was growing discussion about how to bring folks in for longer than 6-12 months.

----

![](../images/18F.png) <!-- .element width="50%" -->

18f.gov

Note:
- 18F is a digital consultancy FOR the U.S. government INSIDE the U.S. government.
- 2014
- GSA is a federal agency that employs about 20,000 people across the country. It handles government wide policy, real estate, procurement, and is basically the admin & operations team for the federal government.

----

And they used Python, Javascript, and Ruby

----

What were the goals of 18F?

Note:
- 18F will transform how the U.S. Government builds and buys digital services -- remember those contract issues?
- builds and buys in a human-centered, design-centric, agile, open, and data-driven way.

----


Delivery is the strategy.

Note:
- 18F was influence by GDS (Government Digital Services)
- As Mike Bracken of the UK’s Government Digital Service says, “the strategy is delivery.”

----

Lesson: Always be shipping.

Note:
- If you are not shipping code, then what are you doing?

----

As I mentioned earlier, software deployment is hard in government... so is hiring.


Note:
- hiring can take as long as 6 to 9 months

----

To make 18F work and to make it successful, we were "Hacking Bureaucracy".

----

## Lesson: "Hackhing the Bureaucracy"  according to Hillary Hartley

- Find innovators inside of the government who have solved similar problems. <!-- .element: class="fragment" -->
- Engage the stakeholders early and often. <!-- .element: class="fragment" -->
- Set up an MVP to get started quickly & iterate. <!-- .element: class="fragment" -->
- Make sure you are working with real users. <!-- .element: class="fragment" -->
- Always stay aligned with the rules of the bureacracy. <!-- .element: class="fragment" -->
- Formalize the process/solution for reuse. <!-- .element: class="fragment" -->

----

Lesson: It's okay to hack your way around the rules, but you must stay aligned with them. - Hillary Hartley

----

![](../images/18F2014.png)

Note:
18F grew to over 150 people in about 1.5 years.

----

## Core tenants of operation at 18F

----

The needs of the user should drive all decisions.

----

Lesson: Everything is an API to
everything else. - Jon Bodner

Note:
- Every engineer needs to learn User research

----

![](../images/18FMethod.jpg)

methods.18f.gov

Note:
- These are great for engaging users and bringing human-centered design to engineering.
- Here are some examples....

----

## Journey Map

![](../images/journeymap.png)

----

## Affinity Map

![](../images/afin1.png)

Note:
- https://docs.google.com/presentation/d/1vIuruOSOV2LZHbVbWkKZExmOhCJ8dQM4UmS6uAqYNO0/edit#slide=id.g1508aa5191_0_704

----

## Affinity Map

![](../images/afin2.png)

----

## Dot Vote

![](../images/dotvote1.png)

----

## Dot Vote

![](../images/dotvote2.png)

----

## Dot Vote

![](../images/dotvote3.png)

----

## Dot Vote

![](../images/dotvote4.png)

----

## Dot Vote

![](../images/dotvote5.png)


----

While we are on the topic of giving back...

## Some More Projects that ~~state & local governments~~ anyone can use

1. Analytics hub
1. Quick mini-sites for content
1. Market research for procurement
1. Help small businesses find opportunities


bit.ly/7projectsBy18F

Note:
- Let's move on to the next core value...

----

Open By Default

Note:
- 18F opens everything by default
- Sadly the government does not.

----

![](../images/osgov.png) <!-- .element width="75%" -->

opensource.org/personas/government

Note:
- This is a list of policies, news, and laws in select countries.

----

![](../images/githubgov.png)

government.github.com/community

Note:
- You can see what governments are building & which are on github.

----

Lesson: Not all projects will work for all countries. People are different.

Example: Estonia versus United States

Note:
- Estonia is a leader in the digital gov space.
- They created a digital identity for their people & now everyone uses it.
- If the U.S. did this the same time that Estonia did, people in the U.S. may have freaked out, b/c culturally they like their privacy.
- On to the next core value...

----

Be Data Driven.

----

![](../images/ana1.png)

analytics.usa.gov

Note:
- This is one the tools available that I mentioned earlier.
- It publishes your analytics to the world.
- There were 2.68 billion visits over the past 90 days.

----

![](../images/ana2.png) <!-- .element width="50%" -->

Note:
- It is tax time for Americans and they are looking for refunds from the government.

----

![](../images/ana3.png)

Note: Weather, earthquakes, etc are popular as well.

----

![](../images/ana4.png)

Note:
- No matter what time of year, USCIS is always on this list.
- It is one of the highest touch points of gov
- While other people will interact once a year with IRS, they will come back to this page 10 times.


----

Lesson: Don't assume you know what people want. Use data.

Note:
- I wouldn't have guessed that USCIS would consistently be most popular.
- With dot voting as a data point -- we might have guessed the winner of that as well.
- And the last core value...

----

Be Agile.

Note:
- Not going to spend a lot of time on this.
- There are plenty of talks on this topic out there.


----

Lesson: Explicitly write this into your contract and be prepared to cancel the contract when other parties want to practice waterfall or agile-fall.

Note:
- Once I had a partner hand me 86 pages of requirements before we event started coding.
- They said they were "agile".
- They didn't want to practice agile.
- Nope. Not doing it.

----

![](../images/usdslogo.png) <!-- .element width="80%" -->

usds.gov

Note:
- Lastly, I wanted to give a shout out to USDS.
- They were a sister org that we worked with.
- Oversimpled they were like the fire fighters and we were like the delivery team.

----

![](../images/usdsplays.png) <!-- .element width="85%" -->

playbook.cio.gov

Note:
- They summed up a lot of what was happening in gov in a great play book


----

And where are they now?

----

![](../images/18F.png) <!-- .element width="50%" -->


Note:
- According to Fed Scoop -- 24.5% of 18F talent has left.
- 18F is now under the procurement / contracts arm of the agency
- However, there is a new office of American Innovation?

----

![](../images/piflogo.png)

Note:
- last bill signed into law by President Obama made statutory the Presidential Innovation Fellows
- The last act as president was for Obama to make the program prenament

----

![](../images/cfpblogo.png)

Note:
- A bunch of tech employees went to 18F
- The current government is not fond of the agency -- views it as too much regulation

----

Lastly...

![Library of Congress](../images/LOC.jpg) <!-- .element width="75%" -->

Note:
- During the making of this talk a bird told me that they were in definitely moving to the cloud.

----

![](../images/18fjump.jpg)

Questions?

jackiekazil@gmail.com


Note:
- YAY! LOC!!!!!
- Finally... if you are interested in working in Puerto Rico, they are talking about making changes!
