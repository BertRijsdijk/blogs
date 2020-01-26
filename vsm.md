#### You perceive your time to market for new features to be slow and want to speed up
You experience that things are slow, and it's hard to finish anything within a sprint length. You've tried to deliver 
smaller increments, but it is still a struggle to complete these in a reasonable amount of time. 

One of the reasons might be that wasteful activities and unnecessary handovers are hiding in your
development process. 

#### A Value Stream Map (VSM) can help you uncover this kinds of waste in your software delivery process

Value Stream Mapping is a form of lean-management and was one of the foundations that made the Toyota Production 
System. It maps the series of events that take a product or service from the beginning of the specific process (inception) 
until it reaches the customer. Even though it stems from a manufacturing world, it can be applied to software as well. 
 
#### How to do it for a software project?
I recommend doing it in a workshop format where everyone who is involved in the value stream is gathered 
(from inception to delivery of the feature to the customers). The technique is simple but the devil is in the details.
Based on a few relevant example slices you map the value stream horizontally from left to right. 
Now vertically map the finer grained tasks including wait times and possible loops between them. 

Next, classify each fine-grained task as Customer Value Adding (CVA), Non Value Adding(NVA) and Waste. This is harder 
then it seems and expect a lot of discussions (do you think code reviews are wasteful when you can pair program?)

Also add the average processing and wait times for the item. It is now possible to calculate cycle efficiency!

Note that the visual and collaboration aspects are important and performing these steps alone will often already lead 
to ideas for optimizations. Next to that it can also bring an increased level of empathy in case of silo'ed organisations.

#### Can I do it just for the development team?
You can and it will be still be very useful for local optimization. The advantage is that a team can do it without any
dependencies on the rest of the organisation. It is smaller and is easier to organise. Most value is 
achieved by mapping the complete value stream though. If this is hard to organise in your project this could point to an 
organisational and / or cultural problem.

#### Could you share some examples of waste that was identified and quantified by a VSM?


#### We are doing Scrum. I've been told a VSM does not apply for Scrum teams
In Scrum, the three pillars Transparency, Inspection and Adaptation should enable autonomous, T-shaped teams to 
self organise, optimize (and eliminate waste). In reality though, teams with various maturity levels struggle 
to do so. Often they are not aware of the wasteful nature of certain activities and the hidden cost of handovers so they
do not try to optimize for this.  

Scrum masters and Agile Coaches often fail to effectively facilitate and challenge teams in this area. A VSM can help in
this scenario as well. 

I do make some adjustments for Scrum: The only official roles in a Scrum team are Dev, PO and SM I tend to focus on 
the tasks and not work from roles. Furthermore (mature) Scrum teams tend to be less rigid and more fluid in terms of 
the flow of work. Still, certain steps do always take place and lead to a picture as below, usually mirroring 
the CI/CD pipeline with all the human tasks required for each step.

#### Should I use specialized tooling?
Tooling exists and can definitely make automation of the calculations easier, as well as repeatability. 
I find the results are better using the walls though. The visual aspect of it is important 
and through collaborating interactively important insights are shared and a common understanding is reached.

#### The implications of lots of handovers in knowledge work
The cost of context switching by loss of focus in knowledge work is even more severe in 
(link to blog the hidden cost of context switching)

#### Make your coaching effort 'measurable'

#### Other contexts where Value Stream Mapping can be provide Value
Creating a DevOps, CI/CD pipeline

#### When would you not use it?

#### Conclusions
VSM's can help you make inefficiencies in the development process visible. In my opinion it is an essential element in 
the toolbox of any coach. Furthermore, for teams it tends to be inspiring and can help kickstart a culture of continuous
improvement. Last but not least, it can make team progress and coaching results more tangible.  

![](parachute.jpg)
![](snail.jpg)


#### The implications of lots of handovers in knowledge work
Cost of context switching by loss of focus. Perhaps not as much for a manufacturing process, but very costly to 
knowledge work
(link to blog the hidden cost of context switching)
#### The relationship between wait times and focus