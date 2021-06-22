## Why Functional Monitoring?
Monitoring is as a crucial part of a successful Continuous Delivery strategy. Yet, monitoring is often 
is primarily focussed on technical metrics like instance health and error rate. 

These metrics are useful but
don't tell the whole story because the end-user perspective is missing. For instance, all services could be "green", yet our customers are not able to log in. 

Functional Monitoring helps to know the system from and end-user perspective

## How do I start with Functional Monitoring?
To help develop thinking around the topic and to come to an effective strategy we categorized different types of 
Functional Monitoring. Each with 

The Functional Monitoring Quadrants consist of 2 axes. 

First we differentiate activity that is coming from actual usage 
versus Synthetic Testing a.k.a.Testing in Production.

Then we differentiate U



###Functional Monitoring Quadrants
![](../functional_monitoring_quadrants_improved.jpeg)



### Case study: A checkout flow

![](../checkout_flow.png)

Consider the example here.

###User Flow Monitoring
####Goal
Measure availability and performance of a critical business flow from the user’s perspective.
####Example
I play a recorded checkout flow through the user's
perspective. I measure that the scenario works end-to-end
####Limitation
Assumption based happy flow. Users might follow a different path with unexpected problems, these will not be found pro-actively.
Subject to continuous maintenance.

###API Endpoint Monitoring
####Goal
Measure that the individual calls give the functionally correct responses, so incorrectness is detected fast.
####Example
I check that the payment-options call gives me the correct
payment options.
####Limitation
Small checks, you only measure the parts but not the sum of the parts.

###Real User Monitoring
####Goal
Measure actual usability and performance of the website from the customers perspective.
####Example
I insert JavaScript (client-side code) to measure where
customers drop off, or experience slowness.
####Limitations
Less data when there is less usage (e.g., at night). Performance measurements are impacted by the capabilities of devices and connectivity of the user.

###Business Metrics 
####Goal
Use data from the different applications to get insights into the business goals to determine if there is an anomaly.
####Example
I measure the orders over time to detect whether I get
less orders then expected.
####Limitation
Anomaly Detection Less valuable when there is a low amount of traffic.



est stability
