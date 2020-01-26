![](parachute.jpg)

#### You perceive your time to market for new features to be slow and want to speed up
You experience that things are slow, and it's hard to finish anything within an iteration. You've tried to deliver 
smaller increments, but it is still a struggle to complete these in a reasonable amount of time. 

One of the reasons might be that wasteful activities and unnecessary handovers are hiding in your
development process. 

#### A Value Stream Map (VSM) can help you uncover this kinds of waste in your software delivery process

Value Stream Mapping is a form of lean-management and was one of the foundations that made the Toyota Production 
System. It maps the series of events that take a product or service from the beginning of the specific process (inception) 
until it reaches the customer. Even though it stems from a manufacturing world, it can be applied to software as well.
<br/><br/>
There it is an extremely helpful technique because of the high cost of of context switching in 
knowledge work and software development specifically (link to blog the hidden cost of context switching) 
 
#### How to do it for a software project?
I recommend doing it in a workshop format where everyone who is involved in the value stream is gathered 
(from inception to delivery of the feature to the customers). The technique is simple (but the devil is in the details).
Choose a few relevant and representative example slices to map the value stream horizontally from left to right. 
Now vertically map the finer grained tasks including wait times and possible loops between them.<br/><br/>
Next, classify each fine-grained task as Customer Value Adding (CVA), Non Value Adding(NVA) and Waste. This is harder 
then it seems and expect a lot of healthy discussion. 
<br/><br/>
Add the average processing and wait times for the item. It is now possible to calculate cycle efficiency! Do not
be surprised if your cycle efficiency is below 30%! 
<br/><br/>
Note that the visual and collaboration aspects are important and performing these steps alone will often already lead 
to ideas for optimizations. Next to that it can also bring an increased level of empathy in case of silo'ed organisations
 and you will help make the growth of a team more tangible. 

#### Can I do it just for the development team?
You can and it will be still be very useful for local optimization. The advantage is that a team can do it without any
dependencies on the rest of the organisation. It is smaller and is easier to organise. Most value is 
achieved by mapping the complete value stream though. If this is hard to organise in your project this could point to an 
organisational and / or cultural problem.

#### Could you share some examples of waste that was identified and quantified by a VSM?
Yes, a client I helped recently had a double code review (one in the team and one outside). The amount of handovers 
and wait times had always been hidden but now became clearer.  
 
 
 After a tough discussion we convinced one
of the teams to experiment with
<br/><br/>
Another client had a Product Owner signoff task which on average took several days to be completed, mostly consisting of
wait time. In this case the development teams were very aware of the problem but the VSM exercise helped convince the 
Product Owner through data that this quality gate was incredibly expensive. It became clear that the PO needed 
to work more closely with the team throughout the iteration instead of validation after the implementation. 

#### We are doing Scrum. I've been told a VSM does not apply for Scrum teams
In Scrum, the three pillars Transparency, Inspection and Adaptation should enable autonomous, T-shaped teams to 
self organise, optimize (and eliminate waste). In reality though, teams with various maturity levels struggle 
to do so. Often they are not aware of the wasteful nature of certain activities and the hidden cost of handovers so they
do not try to optimize for this.

Scrum masters and Agile Coaches often fail to effectively facilitate and challenge teams in this area. 
<br/><br/>
I do make some adjustments for Scrum: The only official roles in a Scrum team are Dev, PO and SM I tend to focus on 
the tasks and not work from roles. Furthermore (mature) Scrum teams tend to be less rigid and more fluid in terms of 
the flow of work. Still, certain steps do always take place and lead to a picture as below, usually mirroring 
the CI/CD pipeline with all the human tasks required for each step.

#### Should I use specialized tooling?
Tooling exists and can definitely make automation of the calculations easier, as well as repeatability. 
I find the results are better using the walls though. The visual aspect of it is important 
and through collaborating interactively important insights are shared and a common understanding is reached.

#### Other contexts where Value Stream Mapping can be provide Value
Creating a DevOps, CI/CD pipeline. Finding bottlenecks and understanding the impact of (external) development dependencies

#### Downsides and when to not use
Consider not using the technique if it you expect it could be used to measure the performance of a team for accountability
 reasons or if psychological safety is lacking. Besides being an undesirable situation it will not work. collaboration 
 spirit and creativity will not be there.   <br/><br/> 
The numbers you calculate are an valuable indication, but are not exact and hard numbers. Also, make sure that creating
the VSM doesn't become waste by spending enormous amounts of time gathering the data. Estimates will usually do fine!  

#### Conclusions
VSM's can help you make inefficiencies in the development process visible. In my opinion it is an essential element in 
the toolbox of any coach. Furthermore, for teams it tends to be inspiring and can help kickstart a culture of continuous
improvement. Last but not least, it can make team progress and coaching results more tangible. Try it!

![](maxresdefault)
