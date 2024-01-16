# 🔗 X-Post-Adviser

🔗 This side project uses python to search for tweets with a high view count and interaction, checks the ratio of the view count to interaction and gets the optimal ratio. It then suggests based on time of post and other factors what and when users should likely post to get a good view and impression ratio on their posts.

## 🔗 Detailed description

🔗 The project uses python and gets input from a user based on his country and followers and view count and post to be typed, if X API allows countries to be used the API searches for posts with a high view count and a high impression count, it also checks the follower count of the users with those high impressions and their impressions relative to the users own following.

🔗 The script will then filter the necessary posts and convert them into a view-to-impression ratio. The higher the ratio, the better chances of being filtered. It then takes the posts of these filtered results (Only texts and no retweets). It saves the posts in a Json format with the time, text of post, view count, impression count, and view-to-impression ratio.

🔗 The script will then go through these posts and record each post temperature, mood, position, context, and what it is about by making use of AI APIs and recording them and saving them in the Json file.

🔗 The script then makes predictions of the time of post and what the post should generally be about in order to see an increased post view and or engagement on the post. It does so by generating a probability number by which the closer it is to one the higher the chances of it reaching the specified view count and possibly engagement.

🔗 If the script generates a figure x for which: 0.7 ≤ x ≤ 1.0 This means that the post the user typed is most likely to reach a higher view count and most likely an optimal view-to-impression ratio.

🔗 If the script generates a figure x for which: 0.5 ≤ x ≤ 0.69 This means that the post the user typed may reach a higher view count and possibly an optimal view-to-impression ratio.

🔗 If the script generates a figure x for which 0 ≤ x ≤ 0.49 This means that the post the user typed is less likely to reach a higher view count and even less likely to reach an optimal view-to-impression ratio.
