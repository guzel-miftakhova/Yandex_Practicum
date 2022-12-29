# Identify inefficient call center agents

**Project status:** *completed*

**Libraries used:** `pandas`, `matplotlib`, `seaborn`, `time`, `datetime`, `numpy`, `sys`, `requests`, `scipy`, `urlencode`

### Description of the project:

"Nupozvoni" is a telecom provider of virtual telephony, our clients are call centers that:
* distribute incoming calls to operators,
* make outgoing calls by operators,
* operators can also make internal calls - calls between each other within the virtual telephony network.

We want to help them find inefficient operators, as well as offer the most favorable rates so that the client lives with us for a long time and does not overpay.

*Efficiency* is an assessment of how optimally the call center resources are used to achieve the required results, i.e. it is high-quality customer service with rational use of available resources.

**The task** is to find the most inefficient operators. Signs of low efficiency:
1. In the case of those call centers that specialize in handling incoming external calls:
- a lot of missed, as well as few calls received per day,
- a long wait for an answer when making calls, including with a small number of calls to the operator (meaning that the wait can be long even with a large operator load, which indicates that there are many calls, and with a small operator load, which may indicate not strong desire of the operator to answer the call).
2. In the case of those call centers that specialize in calling (outgoing external calls):
- few pickups, as well as few or no attempts to contact again with a missed call,
- low call duration.

**Research progress:**
1. Review and preprocessing of data.
2. Exploratory data analysis:
* we will divide call centers by the direction of calls (incoming calls or outgoing calls);
* add new columns to the dataframe and select only external incoming and outgoing calls;
* leave for analysis only those records in which an operator was assigned (for incoming calls).
2. Definition of inefficient operators:
* compare the actual number of calls that each operator received with the number of calls that the operator can receive during the day;
* see what is the average waiting time per day and compare with what is typical for operators;
* compare the actual number of calls each agent made with the number of calls an agent can make during a day;
* Calculate the average duration of a call for an outgoing call and compare it with the duration of an operator's conversation per call.
3. Testing statistical hypotheses:
* outgoing calls of call-cents are more often missed than answered;
* with incoming calls, due to the long waiting time, they often do not wait for the appointment of an operator.

---
**Conclusions on performance indicators for call centers specializing in external incoming calls.**
    
Effective in terms of two indicators of operators, as a rule, one per call center, there are those with two and very few of those with three.
    
According to one of the two indicators, 1-5 operators are effective, less often more.

Not effective at all, 1-2 operators per call center, but there are also those where there are 5 or more of them.
    
1. Number of calls per day:
    - effectively operators: 597 people;
    - ineffective operators: 141 people;
2. Waiting time on the line per day:
    - effectively operators: 138 people;
    - not efficient operators: 600 people.
    
**Performance score findings for call centers specializing in external outbound calls.**
    
As a rule, there are only one/two agents effective in terms of two indicators per call center, but there are also those where there are three or more.

According to one of the two indicators, 1-5 operators are effective, less often more.

Not effective at all for 1 operator per call center, but there are also those where there are more of them.
    
1. Number of calls per day:
    - effectively operators: 781 people;
    - ineffective operators: 52 people;
2. Call duration:
    effectively operators: 246 people;
    - ineffective operators: 587 people.

## Presentation and dashboard

The presentation can be viewed at [link](https://disk.yandex.ru/i/H1ywfOoDWiS0Ig)

The dashboard is hosted on [Tableau Public](https://public.tableau.com/views/-_16669659004100/-?:language=en-US&:display_count=n&:origin=viz_share_link)
