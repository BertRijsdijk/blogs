## Why Functional Monitoring?
Monitoring is as a crucial part of any successful Continuous Delivery implementation. 

I often we see development teams have a hard time striking the right balance between different 
kinds of monitoring, focussing on observability primarily in terms of technical metrics like error rate.

Technical metrics are useful but don't tell the story from the end-user perspective. 
For instance, all services could be "green", while our customers experience broken functionality. 

Functional Monitoring helps to bridge the gap between technical metrics and real user impact, 
greatly enhancing overall observability of the system.

### Functional Monitoring Quadrants
To help build an effective strategy for Functional Monitoring we developed the _Functional Monitoring Quadrants_  

The quadrants consist of 4 complementary types of Monitoring which together will help
you build a effective strategy for validating functional correctness of your software running in production. 

On the horizontal axis we differentiate activity that is coming from actual usage 
versus _simulated activity_, also know as _synthetic testing_ or _testing in production_. 

With synthetic testing we continuously get information about the availability of the system. In other words, we generate the information
about the system by executing tests in production according to a schedule (e.g. every 5 minutes). The downside is that it is not the "real" user
experience, as it is based on assumption on the most common usage

On the other end there is real user activity which generates information based on actual usage. We could say this is more "real" yet we depend
on the amount of traffic. For example when there is little usage at night problems might go undetected.

On the vertical axis we differentiate activity which is part of the direct _user experience_ where we measure each 
step of the user journey versus the _Business Requirements_ which focus on monitoring business metrics

In each Quadrant we defined the single kind of test which we think is most suitable. 
It might be possible to come up with other tests too.


![](../Functional_Monitoring_Quadrants_.jpeg)
All of these different perspecitves matter and give us specific insights, while they also have their
own limitations. Together they for a complete picture. Let's look at the examples to learn more.

## Functional Monitoring in real life
### Case study: A checkout flow

![](../checkout_flow.png)

_Consider this example case_. We will implement Functional Monitoring in a checkout-flow. 
It consists of 3 steps:
- Customer Details
- Shipping
- Payment

We have some integrations with internal and external services like a payment service provider.
We want to be in control and not blindly trust on the external service

How could we approach this checkout flow? What kind of monitoring can we do in each quadrant?

## Functional Monitoring by Example
### Quadrant 1: User Flow Monitoring
#### Goal
I want to measure availability and performance of a critical business flow from the user’s perspective.
#### Example
I play a recorded checkout flow through the user's
perspective. I measure that the scenario works end-to-end and how long it takes to go through the complete flow
#### Limitation
Assumption based happy flow. Users might follow a different path with unexpected problems, these will not be found pro-actively.
Subject to continuous maintenance.

### Quadrant 2: Real User Monitoring
#### Goal
Measure actual usability and performance of the website from the customers perspective.
#### Example
I insert JavaScript (client-side code) to measure where
customers drop off, or experience slowness.
#### Limitations
Less data when there is less usage (e.g., at night). Performance measurements are impacted by the capabilities of devices and connectivity of the user.

### Quadrant 3: Business Metrics 
#### Goal
Use data from the different applications to get insights into the business goals to determine if there is an anomaly.
#### Example
I measure the orders over time to detect whether I get
less orders then expected.
#### Limitation
Anomaly Detection Less valuable when there is a low amount of traffic.

### Quadrant 4: API Endpoint Monitoring
#### Goal
Measure that the individual calls give the functionally correct responses, so incorrectness is detected fast.
#### Example
I check that the payment-options call gives me the correct
payment options.
#### Limitation
Small checks, you only measure the parts but not the sum of the parts.

## Best practices
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

If you don't have a front-end you could do a sequence of API calls
Update user journey on real data 

## Conclusion
We've seen examples of a test in each Quadrant. It really depends on your situation the amount   you probably need them all to some extent
