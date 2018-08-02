+++
title = "Distribution"
pagetitle = "Service Level Agreements for Distribution"
description = "Service Level Agreements for Distribution"
svgicon="/images/distribution.svg"
icon="fa-distribution"
isDirectory = false
weight = 2
alwaysopen = false
+++

The following are the Service Level Agreements for Distribution

# SLA Distribution

During the Term of the TravelgateX License Agreement (as applicable, the "Agreement"), the Covered Service will provide:

* a Monthly ***Uptime*** Percentage to Customer of at least [99.95]% (the “Service Level Objective ” or “SLO”).
* a Monthly ***Overhead*** Accounting to Customer related to the requested Hotels number.

If TravelgateX does not meet the SLO, and if Customer meets its obligations under this SLA, Customer will be eligible to receive the Financial Credits agreed. This SLA states Customer’s sole and exclusive remedy for any failure by TravelgateX to meet the SLO.

## Definitions

The following definitions apply to the SLA:

* “**Covered Service**” means:

	* Responses to requests as part of the TravelgateX Distribution Service.

* “**Downtime**” means:

	* For Responses: Whatever response different to code HTTP 200 when customer have regular access to Internet and for whatever performed request.
	
* “**Downtime Period**” means a period of one or more consecutive minutes of Downtime. Partial minutes or Intermittent Downtime for a period of less than one minute will not be counted towards any Downtime Periods.

	* “SLI uptime” is the mechanism used by TravelgateX to monitor downtimes on the Distribution Service.
	* “SLO uptime (SLOup)” is the degree to which a service is in a specified operable and committable state at the start of a request, when the request is called for at an unknown, i.e. a random, time.

* “**Degradation**” means a quality of service (QoS) out of expected SLO overhead.

	* “SLI overhead” is a indicator used by TravelgateX to account QoS on the Distribution Service. It relates to the amount of time TravelgateX adds over supplier or backend-service time response. Network overhead is not included.
	* “SLO overhead (SLOoh)” will be unsatisfied when 95% of the requests (related to requested hotels) overcome an established amount of time above 15 minutes on an ongoing basis.
	

* “**Monthly Uptime Percentage**” means total number of minutes in a month, minus the number of minutes of Downtime suffered from all Downtime Periods in a month, divided by the total number of minutes in a month.

* “**Monthly Overhead Accounting**” means total number of broken SLO overhead in a month. We assess SLOoh on requested hotels number basis hence we define several sub SLOoh:

sub SLOoh (ms) | Range (requested Hotels number)
:---------------: | :-----------:
<25 | <= 1
<40 | [1-50]
<90 | [50-100]
<225 | [100-500]
<325 | [500-1000]
<450 | [1000-2000]
Not covered | >2000

A SLOoh would be broken when whatever sub SLOoh breaks.

* “**Availability percentage**” means the following:


Monthly Uptime Percentage | (Pending to discuss with Jose Diaz) Percentage of monthly bill for the respective Covered Service in which did not meet SLOup that will be credited to future monthly bills of Customer
:-------------------------: | :-------------------------:
99.00% - < 99.95% | 10%
95.00% - < 99.00% | 25%
< 95.00% | 50%



* “**QoS accounting**” means the following:

Monthly Overhead Accounting | (Pending to discuss with Jose Diaz) Percentage of monthly bill for the respective Covered Service in which did not meet SLOoh that will be credited to future monthly bills of Customer
:-------------------------: | :-------------------------:
3 - < 1 | 5%
5 - < 3 | 10%
> 5 | 20%

## SLA Exclusions

The SLA does not apply to any: (a) features excluded from the SLA (in the associated Documentation), or (c) errors: (i) caused by factors outside of TravelgateX’s reasonable control; (ii) that resulted from Customer’s software or hardware or third party software or hardware, or both; (iii) that resulted from abuses or other behaviors that violate the Agreement;


