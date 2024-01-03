# **REDDIT DATA ANALYSIS**

For this project I have extracted data of askscience and everythingscience subreddits from 11-10-2023 to 30-10-2023 using official python reddit api wrapper(PRAW). Due to recent policy changes at reddit, access to pushshift api which was widely used for data extraction of reddit for research purposes have been limited to the mods of subreddits.
The reason why I chose these subreddits are
- Both subreddits are on same topic i.e. science but with different targets. While askscience contains interesting questions, everythingscience mostly contains informational content often taken from highly acclaimed news and research articles.
- Both subreddits gives contributors option to add Flairs which are really useful to distinguish different topics asked in questions.
- Although there is a huge difference in number of subscribers, the upvotes and comments are present in similar a range.
## ABOUT DATA SELECTION
The 5 metrics used in this project to understand productivity of reddit contributors are
- Flair :- A flair is a tag which shows others what the post is about. For example, a physics flair would demonstrate its a post containing content related to physics. 
- Upvotes :- An upvote on Reddit is a way of expressing appreciation or approval for a particular post. It is a crucial metric to study about contributor productivity.
- Comments :- Higher number of comments could also be linked to better outreach of the post.
- Upvote_Ratio :- It is the ratio of upvotes to downvotes. In a highly scientific subreddit having higher upvote ratio could show higher objectivity.
- Crossposts :- According to reddit
  > Crossposting is an easy way to take a post from one community and share it with another community. When you crosspost content, the crosspost includes an embed of the original post, along with the username, community, and karma score on the original post.
- ID represents a unique id given by reddit to a particular post. It could be used to extract any other attribute associated with the post using praw. Created is the datetime of the post. Both these are descriptive features unique to a post.
