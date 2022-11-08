# Testing changes related to the introduction of an improved recommender system in the online store


**Project status:** *completed*

**Libraries used:** `pandas`, `matplotlib`, `numpy`, `datetime`, `sys`, `requests`, `scipy`, `math`

### Description of the project:

We have a dataset with user actions, a technical task and several auxiliary datasets at our disposal.

**Technical task:**
* Test name: `recommender_system_test`;
* Groups: `A` (control), `B` (new payment funnel);
* Launch date: `2020-12-07`;
* New user recruitment stop date: `2020-12-21`;
* Stop date: `2021-01-04`;
* Audience: 15% of new users from the `EU` region;
* Purpose of the test: testing changes associated with the introduction of an improved recommender system;
* Expected number of test participants: 6000.
* Expected effect: within 14 days from the moment of registration in the system, users will show an improvement in each metric by at least 10%:
    - conversions to view product cards — `product_page` event;
    - cart views — `product_cart` event;
    - purchases — `purchase` event.
 
**Our task** is to evaluate the results of the A/B test:
1. Evaluate the correctness of the test. For this we need to check:
    * intersection of the test audience with a competing test;
    * coincidence of the test and marketing events, other problems of time limits of the test.
2. Analyze the test results.

**The study will take place in three stages:**

1. Data review and data preprocessing.
2. Evaluation of the correctness of the test and exploratory data analysis.
3. A/B test analysis.

**Conclusions on the project:**

Comparison of the results of group `B` with group `A` separately for each event showed that *there are statistically significant differences*
between the proportions of users who made events in each group.
    
***Expected effect:*** in 14 days from the moment of registration in the system, users will show an improvement of each metric by at least 10% is not achieved.
    
**Thus** it can be assumed that in general, the changes associated with the introduction of an improved online store recommendation system,
has a strong influence on user behavior. Also, perhaps, incorrect division into groups, user participation
in several tests at once, marketing campaigns conducted on test dates.
