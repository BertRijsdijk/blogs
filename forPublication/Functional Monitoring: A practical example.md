## Why Functional Monitoring?
Monitoring is a crucial part of any successful Continuous Delivery implementation. 

We often see development teams have difficulty striking the right balance between different 
kinds of monitoring, focusing on observability primarily in terms of technical metrics like error rate.

Technical metrics are helpful but might not tell the whole story.
For instance, all services could be "green", while our customers experience broken functionality. 

Functional Monitoring helps bridge the gap between technical metrics and real user impact to make
the observability of the system complete.

### Functional Monitoring Quadrants
To help create an effective strategy for Functional Monitoring we developed the _Functional Monitoring Quadrants_.  

The quadrants consist of 4 complementary types of Monitoring that, when combined, 
will make it easier to create a complete strategy for validating the functional correctness. 

![](../Functional_Monitoring_Quadrants_.jpeg)

On the horizontal axis we differentiate activity from actual usage 
versus _simulated activity_, also known as _synthetic testing_ or _testing in production_. 

With synthetic testing, we continuously get information about the availability of the system. 
We can generate the information about the system by executing tests in production according to a schedule 
(e.g., every 5 minutes). The downside is that it is not the "real" user
experience: We make assumptions based on the most common usage.

On the other end there is real user activity that generates information based on actual usage. 
We could say this is more "real", yet we depend on the amount of traffic. 
For example, when there is little usage at night, problems might go undetected.

On the vertical axis we differentiate activity that is part of the direct _user experience_. 
We measure each step of the user journey versus the _Business Requirements_, 
which focuses on measuring trends in business metrics like anomalies detection.

These different perspectives matter and give us specific insights, 
while they also have their limitations. 
Together they paint a complete picture. Let's look at the examples to learn more.

## Functional Monitoring in real life
### Case study: A checkout flow

![](../checkout_flow.png)

To give you an idea how these Quadrants can be used, 
I am going to use a generic case study that a lot of you can relate to: a checkout process.

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
I want to measure the availability and performance of a critical business flow from the user’s perspective.
#### Example
I play a recorded checkout flow through the user's
perspective. I measure that the scenario works end-to-end and how long it takes to go through the complete flow.
#### Limitation
Assumption-based happy flow. Users might follow a different path with unexpected problems: these will not be found pro-actively.
Subject to continuous maintenance.

### Quadrant 2: Real User Monitoring
#### Goal
Measure actual usability and performance of the website from the customers perspective.
#### Example
I insert JavaScript (client-side code) to measure where
customers drop off, or experience slowness.
#### Limitations
There is less data available when usage is lower (e.g., at night). Performance measurements are impacted by 
the capabilities of devices and the connectivity of the user.

### Quadrant 3: Business Metrics 
#### Goal
Use data from the different applications to get insights into the business goals to signal anomalies.
#### Example
I measure the orders over time to detect whether I get fewer orders than expected.
#### Limitation
Anomaly Detection is less valuable when there is a low amount of traffic.

### Quadrant 4: API Endpoint Monitoring
#### Goal
Measure that the individual calls give the functionally correct responses, so incorrectness is detected fast.
#### Example
I check that the payment-options call gives me the correct
payment options.
#### Limitation
Small checks, you only measure the parts but not the sum of the parts.

#### What if there is no GUI?
If you don't have a front-end but for example, expose a REST API to your customers a sequence of REST calls as 
performed by the users of the API might give you valuable data. 


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
• Exclude from A/B testing and Analytics



## Conclusion
We've seen examples of a test in each Quadrant. The Quadrants can help you build functional monitoring 
that is complementary to technical metrics. When combining functional and technical monitoring 
you gain a complete picture of the correctness of your system. This way you will get in control, 
gain confidence, and will be able to determine the _real_ impact of incidents.  
