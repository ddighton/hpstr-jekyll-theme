---
layout: page
title: Computational Analysis
description: ""
image:
  feature: abstract-11.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/
  
---

## Early Stages: Reading Tweets with R and Tableau

During the first year of data collection, I converted the JSON files of the Twitter data I’d collected so far into a spreadsheet form that mimicked the structure of the data Twitter afforded. Rows were delineated by tweet IDs and columns corresponded to the Twitter features I covered before like User Location, Tweet Text, and Coordinates. To get a grasp of important themes, as least those that were most frequently mentioned in tweets, I followed Kris Shaffer’s example in “Mining Twitter data with R, TidyText, and TAGS,” published as an Editor’s Choice feature in DHNow. Shaffer describes how researchers might use this suite that combines Google Twitter Archiving Data Sheets, or TAGS, with R and an R data structuring library to enable text mining and frequency analysis on Twitter datasets. Shaffer and his co-researcher Bill Fitzgerald used these tools to understand the way misinformation spreads on Twitter. These tools allow for word frequency charts and the parsing of bigrams, two-word associations that most frequently occur in a dataset. These bigrams enable several other kinds of analyses and visualizations: “We can produce a network analysis of words (essentially a 2D visualization of a Markov model; we could also do this with user data), we can compare word or bigram frequency with another Twitter corpus, and we could search for the most common hashtags and handles in the corpus to find other terms to add to the search that generates the TAGS archive” (n.p.). As Shaffer and Fitzgerald point out, generating bigrams can be a starting point for other kinds of computational and traditional analysis, which generate different possibilities for interpretations and opportunities for comparison that contribute complexity to an analysis. Because Twitter data is rich in metadata, there is multidimensionally within tweet entry. Shaffer and Fitzgerald ultimately focus in on the way in which urls are shared and disseminated across social networks of users to understand possible answers about how misinformation spreads on Twitter. I began with a similar though simpler approach to the dataset I collected, focusing on producing word frequencies and bigrams rather than networks. To protect users’ privacy, I followed Shaffer’s advice on using R to remove personal identifiers like handles and usernames as well as employing a standard list of stopwords. 
Insert Bigrams

In the initial word frequency visualization, issues of race and specific locations emerge. Generating bigrams, however, provides a more contextualized rendering of these themes. Instead of “people”, the bigram is “white people”; “anti” becomes “anti-gentrification”and “art” is “public art.” These richer descriptions might point to the prevalence of perceived agents involved in gentrification identified by users across the corpus as a whole or in areas where tweets are more prevalent. Because bigrams are word pairs, locations become clearer, for instance: Los Angeles, Boyle Heights, Boston’s Chinatown. This early and partial analysis allowed me to focus subsequent research efforts and visualization practices around these emerging themes and locations in a way that human reading 600,000 tweets probably never would have. This kind of macroanalysis (Graham, Milligan, and Weingart, 2015; Jockers, 2013; Ramsay, 2011) can complement traditional methods of close reading and research; however, as Jockers notes: 

> It is also problematic to draw conclusions about specific texts based on some general sense of the whole. This, however, is not the aim of macroanalysis. Rather, the macroscale perspective should inform our close readings of the individual texts by providing, if nothing else, a fuller sense of the literary-historical milieu in which a given book exists. It is through the application of both approaches that we reach a new and better-informed understanding of the primary materials” (28). 

Although Jockers’ discipline is literature, rhetoric and writing studies can use this methodological idea of vacillating perspectives to explore their collection’s larger data environment, in my case the whole collection of tweets on gentrification, and then balance this macroscale perspective with closer examination of data subset(s). This vacillation between macro and micro scale, computer and human reading, provides new comparative possibilities between data scales. This approach doesn’t quite completely resist the omniscient, distant view that feminist theories find problematic, but by providing micro analysis that attends to “situated contexts and geographic locations” (D’Ignazio), we might create polyvocal, nuanced data storytelling that brings a critical awareness to how these differing scales contribute to knowledge making. 

## Graphs and Charts

Tableau is a data analytic software that is frequently licensed by universities, including the one to which I’m affiliated, and it also offers a free version. Though primarily used by professional data analysts in business and nonprofts, Tableau has also been used for academic research and visualization in the humanities and social sciences. [Insert something from Alex Bruns,  In “Towards More Systematic Twitter Analysis: Metrics for Tweeting Activities,”]. After struggling with various other options that required more programming skills, like the R analysis I discussed above, I began to use Tableau because of its easy-to-use Graphic User Interface (GUI) and drag and drop analytical functionality. In Tableau, researchers can upload different file types, like excel or csv files, or, in large dataset cases like mine, link to an SQL database. Once the data has been loaded, visualizations are the primary way to understand the data. Image I is a screen shot of Tableau’s dashboard interface. The dimensions and measures on the left correspond to the names of rows and columns in my database structure. In order to understand how data has changed quantitatively over time, I dragged “Time” into columns and “Tweet ID” into rows, and Tableau generated a line chart. By dragging tweet type into colors, the line chart transformed into three lines, each color corresponding to a tweet type: @mention, original tweet, and retweet. Visualizations like line charts provide a pseudo-objective perspective in which the greatest quantity of items appear to be most significant. In the case of Image 2, the peaks in retweets seem to suggest that there is important activity occurring in those time periods. Tableau is interactive in the sense that it allows users to explore the granular data underneath the lines by clicking on a point on the chart, clicking on the view data icon, and then clicking on the full data tab. A pop-up box will display the underlying data, in this case the rows of tweets and metadata. Using these features, I could sort and export this data for further exploration, providing much smaller, more manageable data subsets that corresponded to peaks in user activity around gentrification and in some cases illuminated tweets and visuals that had gone viral. By doing this, I was able to see which tweets in my dataset were most frequently retweeted as well as matching that activity to particular times. By exploring the tweets, I was able to see how users were communicating about and representing gentrification. In the most retweeted tweets, gentrification was most often associated with popular culture events and changes in the built environment that didn’t relate directly to housing but a broader expanse of cultural colonization. In many of these popular retweets, gentrification is associated with white dominance over nonwhite others and often takes shape through cultural forms like entertainment or commodities. 

The greatest peak is a retweet that occurs on August 25th, with the following text and image:


Image 3 Most Retweeted Anti-Gentrification Tweet

In the subsequent retweets, mentions, and remixes, the user posted the original tweet and remixed it to persuade Twitter users that Taylor Swift is “gentrifying” Beyonce’s song “Formation” in her music video for “Look What You Made Me Do.” This user and others follow up with similar tweets that add more remixed lyrics like “I got ketchup in my bag, swag” and “I see it, I want it, I steal it so I’ll own it.” Not only do users participate in creating arguments about gentrification through visual and textual remix, in the replies to this posts and others like it, users argue about whether a term like “gentrification” can be applied to music and music videos. A chorus of users persuasively argues that gentrification is a process of whitening culture as well as space. The date of this tweet happens to be important, since this activity did follow the Video Music Awards and users were involved in the popular Twitter practice of live tweeting and event. As **** has found, sometimes conventional news outlets report on live tweeting events and “twitter storms”, a term to describe ****. Publications from the Miami Herald to the Huffington Post subsequently reported on the Twitter conversation around the Swift/Beyonce gentrification debate, remarking on how Twitter users’ identified and communicated about Swift’s use of aesthetic visual styles and lyrical content that were similar to Beyonce’s “Formation.” Laurie Gries (2015) points out that to trace the movement and impact of visual rhetoric researchers should also collect and analyze the “metaculture” around them, like news media coverage, other social media data, and various kinds of data explorations that help the researcher situate the data in time, space, and culture. Gries states “[t]hat the pace at which culture changes is driven by motion generated between the circulation of metaculture or ideas and interpretations about culture, and that thing it comments upon” (126). Visual rhetoric like the Swift Gentrification meme and the metaculture around it, then indicates processes of cultural change around gentrification, especially if they are followed by “the production of other actualized versions with the same image or derivatives that may resemble it in form, genre, style, content, or function” (122). Indeed, understanding gentrification as process of cultural appropriation and commodification is the common theme connecting the most popular gentrification tweets in my corpus (Image 4).

In many ways, examining individual tweets and visual rhetoric like the Swift Gentrification meme are richer ways of knowing this data than the Tableau graphs and charts; however, it is simply not feasible to human-read a collection of nearly two-million tweets, which makes data visualization a necessary part of working with this data. Tableau allows users to choose from many different graphs, charts, and map visualizations, but as Drucker points out these “formats are effective, efficient, and surprisingly obfuscating” (907). Tableau functions by further structuring data is according to dimensions and measures, and the resulting visualizations are all different shades of quantitative measurement of attributes, like tweets and users. For instance, this bar chart in Image 5 provides another way to visualize tweets based on frequency. Again, Tableau allows users to click on the bar and explore the underlying data, data which in contains more than just the most frequent posts. Conceivably, a researcher could pick out tweets that weren’t the most frequent, although that’s not the aim of the visualization that functions by graphically orienting the gaze to the quantitatively greatest data items. In the bar chart, the less frequently retweeted tweets aren’t even readily visible on the screen, although a user could click on the sort icon to switch the screen to show least retweeted tweets rather than most retweets. 

Although these ways of exploring the large dataset were interesting and provided a way for understanding how ad-hoc anti-gentrification rhetors communicated about gentrification, particularly in how gentrification was associated with white cultural domination, appropriation, and commodification of nonwhite culture and spaces, Tableau didn’t illuminate any of the tweets made by more organized anti-gentrification groups. I knew such groups existed in the dataset, partially through my initial R frequency analysis of bigrams, but also through human reading portions of the dataset spreadsheet. To make Tableau see these smaller groups, who, because they largely act more locally and outside of the realm of celebrity and entertainment, are not retweeted to the extent that memes about Taylor Swift or $15 40s are, I separated all tweets that contained “Boyle Heights,” a frequently mentioned location in the R analysis. I added these tweets to separate database and conducted additional research to provide smaller-scale partial view that also strives to situate and contextualize that data in bodies and geographical spaces. 