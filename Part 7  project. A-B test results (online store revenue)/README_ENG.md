## Prioritization/testing hypotheses for increasing revenue in an online store - evaluating the results of an A / B test

**Project status:** *completed*

**Libraries used:** `pandas`, `matplotlib`, `numpy`, `scipy`, `math`, `datetime`

### Description of the project:

Together with the marketing department of a large online store, we prepared a list of hypotheses for increasing revenue.
We have data on 9 hypotheses for increasing the revenue of an online store with the specified parameters and the results describing the conduct of an A/B test.

**Our mission**:
* prioritize hypotheses;
* analyze the results of the A/B test;
* make a decision based on the results of the test.

**Research Progress**

The study will take place in two parts:
1. Prioritization of hypotheses
    - apply the ICE framework to prioritize hypotheses;
    - apply the RICE framework to prioritize hypotheses;
    - let's see how the prioritization of hypotheses has changed when using RICE instead of ICE.
2. A/B test analysis
    - build graphs: cumulative revenue / cumulative average check / cumulative conversion by groups; relative change in the cumulative average check / cumulative conversion of group B to group A; dot plot of the number of orders by users / order values;
    - calculate the percentiles of the number of orders per user / order value;
    - we calculate the statistical significance of differences in conversion / in the average check of an order between groups according to "raw" data / according to "cleaned" data;
    We will make a decision based on the results of the test.

**Conclusions on the project:**

Based on the facts found, the test can be stopped and considered a success because, given the available data, group B is consistently better than group A.
