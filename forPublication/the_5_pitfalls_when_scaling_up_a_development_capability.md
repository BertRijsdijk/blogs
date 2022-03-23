# The 7 pittfalls that make software scale-ups fail (and what you should do about it)

## The challenge: From Start-up to Scale-up
Growing a new software into a scale-up is hard. This phase of a company requires a shift in thinking and very specific leadership skills
that differ greatly from what was needed from the start-up phase.
<br></br>
In this blog I am describing a set of _problems_ and _patterns_ that I have observed in some of the scale-ups I've worked with.
If not addressed, these patterns can be detrimental to the future of these organisations and could ultimately lead to failure.<br></br>
For each identified problem I will try to give a tangible solution based on my experience, here we go.

## 1. Scaling the teams up quickly over scaling up the teams organically
Expansion of the development teams and capabilities are not always driven by an organic need in terms of output or concrete goals 
and objectives. Sometimes the expansion is driven by future expectations and pressure from investers to go grow fast for some future velocity. 
Scaling up can then seems to almost become a goal in itself. <br></br>
Sometimes organisational growth is driven by concrete targets but the only reflex known is just to add more bodies in the assumption 
that velocity will at least keep going up to an extent. 
<br></br>
The result could come as a surprise: When adding resources too quickly it becomes very hard to instill or uphold things like healthy development practices and team purpose. There is alo a
cost associated with more complex communication patterns in and between bigger teams.
<br></br>The problem becomes visible in the form of lower velocity, lower predictability and lower quality. It is undoubtly tied in with a number of other problems listed in this blog. 

<b>Organic growth</b> is to add only so many resources that enable you to maintain an increasing the number of features that can be released a.k.a. <b> working software in production</b> 
while maintaining healthy development practices. 
<br></br> DORA and technical-dept metrics could be used for the purpose of determine if the teams can absorb more. <b>Stalling progress in these metrics can be an indicator to stop or change course in your hiring process</b>. 
<br></br>Consider working on increasing the key metrics first _and getting specific hires to improve those_ before you start growing the product teams again and choose no-hires over poor hires.

## 2. Backlog filled with low business value items an/or missing system to determine value

Under the stress of demanding stakeholders, clients and investors the backlogs get filled up quickly while the company is still learning about it's value and mission. 
The result is an enormous body of potential work with undetermined value. Even the growth of the development team itself will lead to more backlog items as most employees 
will likely try to be useful and suggest improvements and things they need to do to make the product and developer experience better.

The problem becomes visible in the form of long backlogs where PBI's miss business value, prioritisation becomes difficult and missing objective business value criteria. 
A missing written product goal is also a red flag as well as missing business goals to measure the succes of the software against. 

In organisations that have this problem software teams often lack a sense of purpose.

When you are finding yourself in this spot you could consider the following approach to make it better:
<b>
1. Have a written down company mission, business goals for all to see
2. Create a system to determine business value in an objective way. Think for example of a scorecard for PBI's against business goals or company mission 
3. Measure and score backlog items against it, for example through business value poker
4. Always include metrics how to measure success for each feature or experiment
5. Callibrate the sytem with your product management team so it get's better over time
6. Use measurements to re-iterate on the business goals, company vision and business value
7. Repeat the process
</b>
<br>

Succes depends on using such system with discipline. Letting go of a feature where you invested in 
emotionally or financially is hard. It could be tempting to game the system. It requires a strong vision, leadership and a 
experienced product management capability to avoid stepping into these traps.
 
Read:

- The lean startup by Eric Ries (yes, even though you consider yourself
a scale-up) 
- the professional product owner by SCRUM.org

## 3. Isolation and silo forming between value streams

This is a pattern which I've come across in some organisations that explore different potential fatures and / or revenue streams at the same time.
The work is divided over several end-to-end teams working in parallel where a  level of isolatition between the teams is observed.<br></br>
These teams each focussed on particular areas or features that share a lot of technical and functonal similarities.<br></br>
The teams can easily end up being silo'ed from each other while at the same time using a lot of shared code. When the teams are aware 
of only their own team mission it can lead to poorly optimized software.

Observable symptoms are: Suboptimal and inconsistent end-user experience, poor system performance, inflexible and entangled (micro) services architecture,
poor performance

What can you do about it?

- <b>Make sure your development teams have enough knowledge about the key company mission and products</b>. 
  - Update them on a continuous basis and involve them early
  - Involve them in an active way (e.g.  in figuring out user journey and goals together with the business, communicate via examples)
- <b>Consider using one backlog instead of having each team work on their own
- Make sure an ongoing discussion between the teams is facilitated on a regular basis, for instance with</b>
  - A daily standup between the teams, like Scrum of Scrums
  - Team representatives or whole team visits the demo / sprint review of other teams
  - Using an architecture guild with representative of each team to understand where the other teams are heading on technical path 
  - A shared architecture picture that is continuously updated and visible to everyone (wall and / or virtual board)
  - Shared items like DoD's and non-functional requirements 
  - Lightweight architectural decision logs in the code

## 4. Loss of contact with the end-user product in development team
  
Strongly correlated to #3 this can be seen at companies that give their team narrow technical missions 
which are not directly related to the working end-user product. Sometimes there are even teams that have never used
or seen the end product. <br></br>I am not talking about enablement teams like SRE or platform teams, , which improve developer experience
or take some of the shared infra / cloud work between the teams away. 
No I am talking about team component based teams, also refered to as _horisontal_ teams.<br></br>

This kind of system disconnects 

<br></br>Symptoms include:
- Bad UX experience of the end-product
- Late feedbackloop outside the team (e.g. test and/or stabilization sprint), 
- Teams that can not take end-to-end ownership
- Inter-team dependencies (e.g. backend services need to be finished first before other teams can start)
- Poor non-functional performance
- Architecture doesn't enable a good end product

What to do about it?

<br></br>
## 5. Only focussing on functionality and forgetting enablement for the teams to take end-to-end responsibilty
<br></br>
## 6. Creating heavy business processes and to much focus on 'allignment'

A symptom of the problem is scale-up that makes you feel like you are part of a big corporate environment. Software release procedures are long and cumbersome. Getting a new laptop requires filling in a form.
<br></br>

## 7. Repeating the same mistakes over and over again, instead of learning 

The comfort for all to not look and just "look forward" 

- Blameless retrospective
## Solutions


Development doesn't understand business needs
##Conclusions


There is so much to do!
Increasing developer experience\
Enable measurement of the development process\
Implementing a strategy for technical and functional monitoring from the get-go and building it into the product\
Focus on the top 3 valuable items for your clients and  or end-users and swarm around these\
Share a tangible product strategy with your development teams (s)


Ultimately, the maturity of the leadership and product management teams matter in being able to set the proper expectations 


SRE teams - Risk tolerance 
Platform team
Measurements code complexity - Relationshis between services - Service decomposition
cycle time, mean time to repair, deployment frequency, change failure rate

Matching ambitions with ..
### My investor expects me to grow quickly. What do I do with all these bodies?






Forgetting to be a learning organisation 



Scaling up also implies bigger backlogs that need to be filled. There are two sides to this phenomenon.
More people will work and create ideas which will often lead to backlog items and the expectancy of more capacity itself can
trigger more promises and variants on product offering.
