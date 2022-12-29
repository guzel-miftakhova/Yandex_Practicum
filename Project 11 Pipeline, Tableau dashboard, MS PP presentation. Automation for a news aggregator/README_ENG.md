# Creating a custom events dashboard for the news aggregator

**Project status:** *completed*

**Libraries used:** `pandas`, `matplotlib`, `plotly`, `sqlalchemy`

### Description of the project:

We work for Yandex.Zen. Almost all of our time is spent analyzing user interaction with article cards.

Each card is defined by its theme and source (it also has a theme).
Examples of topics: *"Beauty and Health"*, *"Russia"*, *"Travel"*.

The users of the system are characterized by the age category. Let's say *"26-30"* or *"45+"*.

There are three ways for users to interact with the system:
* The card is displayed for the user (`show`);
* The user clicked on the card (`click`);
* The user has viewed the card article (`view`).

Managers ask the same questions every week:
1. How many user interactions with cards occur in the system, broken down by card topics?
2. How many user interactions with cards do sources with different topics generate?
3. How do the topics of the cards and the topics of the sources compare?

Obviously, it's time to automate the process and make a dashboard for managers.

**Task:** using Yandex.Zen data to build a dashboard with metrics of user interaction with article cards for use by managers.

**We need**:
1. Discuss in detail with managers the composition of the dashboard, its appearance and the set of displayed data.
2. Communicate with database administrators and find out where and how the necessary data is collected.
3. Decide with them where to store aggregate tables.
4. Start developing the pipeline and dashboard.

**Conclusion on the project:**


The dashboard is available at [link](https://public.tableau.com/views/_16642857231360/Yandex_dzen_1?:language=en-US&:display_count=n&:origin=viz_share_link).

The presentation has been prepared and is available at [link](https://disk.yandex.ru/i/D1_cjV3SrX8OpA).
