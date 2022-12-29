## Determination of a favorable tariff for a telecom company

**Project status:** *completed*

**Libraries used:** `pandas`, `matplotlib`, `numpy`, `scipy`

### Description of the project:

Megaline is a federal mobile operator. Clients are offered two tariff plans: "Smart" and "Ultra".

We have the data of 500 Megaline users for 2018.

**Description of tariffs:**
1. Tariff "Smart"
* monthly fee: 550 rubles
* included 500 minutes of calls, 50 messages and 15 GB of data
* the cost of services in excess of the tariff package:
    * minute of conversation: 3 rubles
    * message: 3 rubles
    * 1 GB of Internet traffic: 200 rubles
2. Tariff "Ultra"
* monthly fee: 1950 rubles
* included 3000 minutes of calls, 1000 messages and 30 GB of internet traffic
* the cost of services in excess of the tariff package:
    * minute of conversation: 1 ruble
    * message: 1 ruble
    * 1 GB of Internet traffic: 150 rubles

*Note*

*Megaline always rounds seconds to minutes, and megabytes to gigabytes. Each call is rounded separately: even if it lasted only 1 second,
will be counted as 1 minute. For web traffic, individual sessions are not counted. Instead, the monthly total is rounded up.
If a subscriber uses 1025 megabytes this month, they will be charged for 2 gigabytes. Unused for the previous month calls, sms,
internet is not carried over to the next month.*

To adjust the advertising budget, the commercial department wants to understand which tariff brings in more money.

**Our mission**
    analyze the behavior of Clients and draw a conclusion - which tariff is better.

**Research Progress**

The study will take place in three stages:
 1. Data review.
 2. Data preprocessing.
 3. Preliminary analysis of tariffs on a small sample of customers and verification of hypotheses:
      * the average revenue of users of the "Ultra" and "Smart" tariffs differ;
      * the average revenue of users from Moscow differs from the revenue of users from other regions.
   
 **Conclusions on the project:**
  - on average, at the "Ultra" tariff, users spend more minutes on calls, write more messages and spend more Internet traffic, but there are fewer such users;
  - the "Smart" tariff is more popular, it brings more money, regardless of the region.
