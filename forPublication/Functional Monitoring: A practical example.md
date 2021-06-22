## Why Functional Monitoring?
Monitoring is as a crucial part of a successful Continuous Delivery strategy. Yet, we see that monitoring often 
is primarily focussed on technical metrics like instance health and error rate. 

These metrics are useful but
don't tell the story from the end-user perspective. For instance, all services could be "green", while our customers experience broken functionality. 

Functional Monitoring helps to bridge the gap between technical metrics and real user impact, greatly enhancing overall observability of the system.

## But which kind of Functional Monitoring?
We've come up with 4 distinct but complementary types and categorized them into what we call the _Functional Monitoring Quadrants_.  

On the horizontal axis we differentiate activity that is coming from actual usage 
versus simulated activity, also know as _synthetic testing_ or _testing in production_.

On the vertical axis we differentiate activity which is direct user-facing 
versus activity which is  _implementation facing_. These tells us something about functional correctness but the relation to the used is _indirect_.

All of these kinds of Monitoring give us specific insights, while they also have their
own limitations. Let's look at some examples to learn more

###Functional Monitoring Quadrants
![](../functional_monitoring_quadrants_improved.jpeg)


##Functional Monitoring by Example
###Case study: A checkout flow

![](../checkout_flow.png)

Consider the example case. We will implement Functional Monitoring in a checkout-flow. 
It consists of 3 steps:
- Customer Details
- Shipping
- Payment

We have some integrations with internal and external services like an external service to check the customer address.
We want to be in control and not blindly rely on the external service

How could we approach this checkout flow? What kind of monitoring can we do in each quadrant ? Let's dive in

###Quadrant 1: User Flow Monitoring
####Why?
I measure availability and performance of a critical business flow from the user’s perspective.
####Example
I play a recorded checkout flow through the user's
perspective. I measure that the scenario works end-to-end, the flow can be completed and how long it takes
####Limitation
Assumption based happy flow. Users might follow a different path with unexpected problems, these will not be found pro-actively.
Subject to continuous maintenance.

###Quadrant 2: Real User Monitoring
####Goal
Measure actual usability and performance of the website from the customers perspective.
####Example
I insert JavaScript (client-side code) to measure where
customers drop off, or experience slowness.
####Limitations
Less data when there is less usage (e.g., at night). Performance measurements are impacted by the capabilities of devices and connectivity of the user.

###Quadrant 3: Business Metrics 
####Goal
Use data from the different applications to get insights into the business goals to determine if there is an anomaly.
####Example
I measure the orders over time to detect whether I get
less orders then expected.
####Limitation
Anomaly Detection Less valuable when there is a low amount of traffic.

###Quadrant 4: API Endpoint Monitoring
####Goal
Measure that the individual calls give the functionally correct responses, so incorrectness is detected fast.
####Example
I check that the payment-options call gives me the correct
payment options.
####Limitation
Small checks, you only measure the parts but not the sum of the parts.

##Best practices
• Identify the most critical flow(s)\
<br/>
• Start with one flow and learn\
<br/>
• Keep the number of tests to a minimum\
<br/>
• Make it fail\
<br/>
• Don’t make the assertions overly strict\
<br/>
• Exclude from A/B testing and Analytics\

##Conclusion
We've seen examples of a test in each Quadrant. It really depends on your situation the amount   you probably need them all to some extent
