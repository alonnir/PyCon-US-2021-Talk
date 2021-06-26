# PyCon-US-2021-Talk
Slides and code for "Getting an Edge with Network Analysis" [talk at PyCon US 2021](https://us.pycon.org/2021/schedule/presentation/60/).

Interested in learning more about network analysis? Check out **[SNAcks](https://github.com/alonnir/snacks)** for a highly curated resource list (or a snack size awesome list).

The video of the talk is now available [here](https://www.youtube.com/watch?v=DPqhV21tSAc).

---

### Take-home assigments

1. Wikipedia surfing challenge
- Use Wikipedia's data to build a netwrok, where articles act as nodes and internal links between one node to another are the edges. Calculate measures such as [betweeness centrality](https://networkx.org/documentation/stable/reference/algorithms/centrality.html#shortest-path-betweenness) or [PageRank](https://networkx.org/documentation/stable/reference/algorithms/generated/networkx.algorithms.link_analysis.pagerank_alg.pagerank.html#networkx.algorithms.link_analysis.pagerank_alg.pagerank) to find important and interesting nodes. What interesting things can you learn about Wikipedia's network?

- Using the network you built, choose 2 articles on Wikipedia for very different topics (e.g. [Python Conference](https://en.wikipedia.org/wiki/Python_Conference) and  [Hot-air balloon](https://en.wikipedia.org/wiki/Hot-air_balloon)) and find all the paths between them. What can you observe by exploring the different paths?


Data can be found [here](https://en.wikipedia.org/wiki/Wikipedia:Database_download) and some inspiration can be found [here](https://github.com/search?q=wikipedia+network+analysis).

Edit: Thanks to a kind commenter in PyCon's live chat, I learnt about this fantastic site - [Six Degrees of Wikipedia](https://www.sixdegreesofwikipedia.com/).

2. How would you answer the Biz Dev question?
In the talk we introduced a [dataset](https://github.com/alonnir/PyCon-Us-2021-Talk/tree/main/data) with transactions on a peer-2-peer payments platform. How would you use this data to find merchants/businesses using this platform? Hint: what would you expect the network around metchants would look like, and how will it be different from networks around "standard" users.

3. You work for a social network and want to limit the spread of misinformation. 
- How would you use network analysis to do that effectively?
- Try to think how network where (mis)information travels fast look like, and how is it different from networks where the spread of (mis)information is slower.

4. [I Want Out](https://www.reddit.com/r/IWantOut/) is a community on reddit where posts' titles detail the [OP](https://www.urbandictionary.com/define.php?term=OP)'s country of origin, and desired relocation country. For example: `[IWantOut] 23M USA-> Netherlands`. 
- Get your hands on a data set of posts from the subreddit. Fortunately, it's [relatively](https://towardsdatascience.com/scraping-reddit-data-1c0af3040768) [easy](https://www.reddit.com/r/redditdev/comments/ce4fj3/best_way_to_get_all_posts_from_a_subreddit/etytw71/?utm_source=reddit&utm_medium=web2x&context=3) to collect that data.
- Use the dataset you obtained to create a _directed_ network. What interesting things can you learn from the network? Which are the top countries users want to leave? Which countries are the most desired locations?
- Extra points if you add age, gender or occupation (which are often included in the title of the post) as node _attributes_.
- Finally, try to think what are the limitations of such analysis. Is the data biased in any way (or multiple ways)?
