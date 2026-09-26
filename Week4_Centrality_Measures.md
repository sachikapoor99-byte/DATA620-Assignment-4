# Week Four Assignment: Centrality Measures

For this assignment, I would use bill sponsorship and co-sponsorship data from the U.S. Congress. The data is available through the Congress.gov API. I would focus on members of the House of Representatives during the 118th Congress so the network would not become too large.

Each node would represent a member of the House. A connection would be created when one representative co-sponsored a bill introduced by another representative. I could also give the connections different weights based on how many times two representatives worked together.

The categorical variable I would use is political party, such as Democrat, Republican, or Independent. The dataset also includes information like each representative’s state and congressional district.

To prepare the data, I would first request an API key and use Python to collect information about the bills, their sponsors, and their co-sponsors. I would organize the information in pandas and then use NetworkX to create the graph. After building the graph, I would calculate degree centrality for each representative. I could then compare the average degree centrality of each political party and create a box plot to show the differences between the groups.

The outcome I would want to predict is legislative success. For example, I could define success as whether a representative had at least one sponsored bill pass the House or become law. My prediction would be that representatives with higher degree centrality may be more likely to have legislative success because they have worked with a larger number of their colleagues.

I would also compare whether this relationship is different across political parties. Members of the majority party might have both higher centrality and more successful bills because their party has greater control over the legislative process. However, centrality would not be the only factor. Committee assignments, seniority, leadership roles, and the subject of a bill could also affect its outcome.

Overall, this network could help show whether having more connections in Congress is related to a representative’s ability to move legislation forward.

## Data Source

[Congress.gov API](https://api.congress.gov/)
