![](../parachute.jpg)
#### You perceive your time to market for new features to be slow and want to speed up
You experience that things are slow, and it's hard to finish anything within an iteration. 
You've tried to deliver smaller increments, but it is still a struggle to complete these in a reasonable amount of time. 
One of the reasons might be that wasteful activities and unnecessary handovers are hiding in your development process. 
#### A Value Stream Map (VSM) can help you uncover these kinds of waste in your software delivery process
Value Stream Mapping is a form of lean-management and was at the foundation of the Toyota Production System.
A VSM maps the series of activities that take a product or service from the beginning of the specific process (inception) until it reaches the customer. 
<br/><br/>
Even though the technique stems from a manufacturing world, it can be applied to software as well.
In software development it is an extremely helpful technique because of the [high cost of context switching](https://xebia.com/blog/epic-focus-measure-your-way-to-a-better-time-to-market/) in knowledge work and software development specifically.
 
#### How to do it for a software project?
I recommend doing it in a workshop format where everyone who is involved in the value stream is gathered (from inception to delivery of the feature to the customers).
The technique is simple (but the devil is in the details).
Choose a few relevant and representative example slices to map the value stream horizontally from left to right. 
Now vertically map the finer-grained tasks including wait times and possible loops between them.
<br/><br/>
Next, classify each fine-grained task as Customer Value Adding (CVA), Non-Value Adding(NVA) and Waste.
 This is harder then it seems so expect a lot of healthy discussions.
<br/><br/>
Add the average processing and wait times for the item.
It is now possible to calculate the cycle time/efficiency!
Do not be surprised if your cycle efficiency is below 30%! 
<br/><br/>
Note that the visual and collaboration aspects are important and performing these steps alone will often already lead to ideas for optimizations.
Next to that, it can also bring an increased level of empathy in the case of siloed organizations and you will help make the growth of a team more tangible. 
#### Can I do it just for the development team?
You can and it will still be very useful for local optimization.
The advantage is that a team can do it without any dependencies on the rest of the organization.
It is smaller and is easier to organize.
Most value is achieved by mapping the complete value stream though. If this is hard to organize in your project this could point to an 
organizational and/or cultural problem.
#### Could you share some examples of waste that were identified and quantified by a VSM?
Yes, a client I helped recently had a double code review (one in the team and one outside). The huge amount of handovers 
and wait times had always been hidden but now became visible to the teams. Because of all the waiting teams would switch to other tasks.
Effectively everything was in progress at the same time. After a tough discussion, we convinced one of the teams to experiment 
with pair programming. Besides knowledge sharing this greatly reduced the cycle efficiency (as much as 25%!) creating an upward spiral for
the team. 
<br/><br/>
Another client had a Product Owner signoff task which on average took several days to be completed, mostly consisting of
wait time. In this case, the development teams were very aware of the problem but the VSM exercise helped convince the 
Product Owner through data that this quality gate was incredibly expensive. It became clear that the PO needed 
to work more closely with the team throughout the iteration instead of validating features after implementation. 
#### We are doing Scrum. I've been told a VSM does not apply for Scrum teams
In Scrum, the three pillars Transparency, Inspection and Adaptation should enable autonomous, T-shaped teams to 
self organize, optimize (and eliminate waste). In reality, teams with various maturity levels struggle 
to do so. Often they are not aware of the wasteful nature of certain activities and the hidden cost of handovers so they
do not try to optimize for this.
Scrum masters and Agile Coaches often fail to effectively facilitate and challenge teams in this area. 
<br/><br/>
I do make some adjustments for Scrum: The only official roles in a Scrum team are Dev, PO, and SM.
I tend to focus on the tasks and not work from roles.
Furthermore (mature) Scrum teams tend to be less rigid and more fluid in terms of the flow of work.
Still, certain steps do always take place and lead to a picture as below, usually mirroring the CI/CD pipeline with all the human tasks required for each step.
#### Should I use specialized tooling?
Tooling exists and can make the automation of the calculations easier, as well as repeatability and 
storing results from specific measurement periods.
I find the results are better using the walls though.
The visual aspect of it is important and through collaborating interactively important insights are shared and a common understanding is reached.
#### Downsides and when to not use
Consider not using the technique if you expect it could be used to measure the performance of a team for accountability reasons or if psychological safety is lacking.
Besides being an undesirable situation it will not work. 
collaboration spirit and creativity will not be there.
<br/><br/> 
The numbers you calculate are a valuable indication but are not exact and should not be treated as hard numbers.
Also, make sure that creating the VSM doesn't become waste by spending enormous amounts of time gathering the data.
Estimates will usually do fine!  
#### Conclusions
VSM's can help you make inefficiencies in the development process visible.
In my opinion, a VSM is an essential element in the toolbox of any coach.
Furthermore, for teams, it tends to be inspiring and can help kickstart a culture of continuous improvement.
Last but not least, it can make team progress and coaching results more tangible.
Try it!
![](../maxresdefault.jpg)