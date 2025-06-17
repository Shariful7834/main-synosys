---
title: "Do Alice Weidel and the AfD benefit from Musk's attention on X?"
subtitle: ""

tags:
  - elections
  - social media

summary: ""

categories: []
date: "2025-01-24"

lastMod: "2025-01-24"

featured: true

draft: false

authors: ["sami", "admin"]

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
caption: ""
focal_point: ""
# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
---

**Has Elon Musk manipulated X to give the AfD more reach? He has made it clear in posts, articles and election events that he is a fan - and at the same time, Alice Weidel's reach on X has increased significantly. Could these developments be linked? This blog post describes a data analysis in which we take a closer look at which accounts have received how much reach and whether Musk's influence can be determined. Where does the sudden increase in Weidel's reach on X come from?**

**Note: This work has not yet been peer reviewed.** A more detailed description of the analysis, the methods, as well as the code and data can be found <a href="https://osf.io/jcqen/" target="_blank">here</a>.

In recent weeks, there has been a lot of fuss about Elon Musk's possible influence in favour of the AfD. First, on 20 December, he wrote on his platform X (formerly Twitter) that <a href="https://x.com/elonmusk/status/1869986946031988780" target="_blank">only the AfD can save Germany</a>. On 28 December, Die Welt published a guest article by Musk in which he expressed the same position. Finally, on 9 January, he held a public conversation on X with the AfD candidate Alice Weidel.

As already reported in <a href="https://bsky.app/profile/jhillje.bsky.social/post/3lfckchdifs2u" target="_blank">one</a> place or <a href="https://bsky.app/profile/curdknupfer.bsky.social/post/3lfcp265mgs2k" target="_blank">another</a>, Weidel gained a lot of reach on X. <a href="https://www.zeit.de/politik/deutschland/2025-01/bundestag-wahlkampf-einmischung-wahlkampf-musk-elon-weidel-alice-pruefung" target="_blank">The German parliamentary administration then announced</a>  that it would investigate whether Musk is influencing the election campaign. At the same time, <a href="https://www.zdf.de/nachrichten/politik/eu-kommission-elon-musk-x-algorithmus-100.html" target="_blank">the EU Commission</a> is demanding insight into possible changes to X's recommendation algorithms. This article analyses the possible impact of Musk's activities on the reach of the AfD and Weidel in particular on social media. 


<div class="baskerville tl f1-l f4-m f4">
            <iframe src="/Fig_1.html" width="100%" height="700px" frameborder="0"></iframe>
          </div>

**Figure 1** Number of followers of various German politicians (top) and views of Weidel's posts with and without retweets from Elon Musk (bottom, retweets outlined in red).

**Weidel's jumps in reach often coincide with Musk's expressions of sympathy**

Let's start with the number of follows on X (Fig. 1, top). For the politicians Lindner, Scholz, Merz and Habeck, we see how the number usually grows: slow and steady. It is different with Weidel. We see two sharp jumps and a steady but faster increase in between. The first increase occurred around 20 December. At this time, Musk posted that only the AfD could save Germany and also mentioned the AfD in other posts. However, these were only mentions (with and without links) and not retweets. This is an important difference. In the case of a retweet, the original post also appears in Musk's timeline and, as he is followed by over 200 million people, this automatically generates a lot of reach. With ‘mere’ mentions, those who follow Musk first have to go to the respective profile of the account mentioned and that is often a bigger hurdle.

Around 28 December - Musk's contribution to Die Welt - he retweeted a post by Weidel for the first time (in which she thanked him for the guest article). This post has 15 million views (Fig. 1, below, outlined in red). However, the public conversation with Musk seems to have had a particular impact on the number of her followers. In the days leading up to 9 January, Musk mentioned and retweeted Alice Weidel several times, which earned her as many as 24 million views for one post, and on 10 January her number of followers increased by almost 150.000.

Figure 1 shows that individual posts by Weidel that were retweeted by Musk received a large number of views. However, individual posts without retweets also have a high reach. In order to find out whether there was a specific point in time when Weidel's views started to increase, we carried out a so-called changepoint analysis. Roughly speaking, this method is used to find out whether the data can be better described with one or two trend lines and, if there are two, where the break should be made. The analysis showed that there was already a significant break on 16 December. On that day, Olaf Scholz lost the vote of confidence in the German parliament. The two trend lines are shown in red in the lower part of Figure 1. You can see that the second line is well above the first. In the first period, Weidel's posts received an average of almost 140.000 views, then almost 790.000.

**A few retweets with a wide reach have created views for Weidel's posts**

<iframe src="/Fig_2.html" width="100%" height="600px" frameborder="0"></iframe>

**Figure 2** Development of the views of Weidel's posts over a period of 36 hours. Note: The post in the centre is no longer available, but it was also announced on <a href="https://alice-weidel.de/aktuelles/neuer-beitrag-auf-x-com-229/" target="_blank">Alice Weidel's website</a>.

Let's now take a closer look at Weidel's posts. To do this, we regularly accessed X over a longer period of time so that we could not only record the absolute numbers, but also their development, i.e. how quickly they grow. Figure 2 shows the six most viewed posts by Alice Weidel and their dynamics over 36 hours. The dashed lines show the time at which Musk mentioned Weidel and the red lines show that this post was even retweeted by Musk. Two things are striking about the posts that were retweeted. Firstly, these tend to have the most views and secondly, the views only jump in these cases and this always takes place shortly after the post was retweeted by Musk. We were unable to find similar jumps for the four other politicians.

<iframe src="/Fig_3.html" width="100%" height="700px" frameborder="0"></iframe>

**Figure 3**	Engagement metrics of posts by various German politicians before and after 16 December 2024.

Figure 3 shows not only the views, but also retweets and likes of individual posts. The ratio of views and retweets provides an indication of the distribution of the post. If a post has many views but comparatively few retweets, then there is probably one or more accounts with a very wide reach among the retweets. In the case of Alice Weidel's post, you can see a sharp increase in views after 16 December, but a less sharp increase in retweets. A comparison with the other four politicians also shows that it is Weidel's views that increased after 16 December, but not her retweets. You can see the contrast when you look at Habeck in particular, whose posts receive comparatively many retweets. It seems as if he has an active base that retweets his posts, whereas with Weidel it tends to be individual accounts that use their high reach to generate views for her through retweets.

**The rest of the AfD has not gained as much as Weidel**

<iframe src="/Fig_4.html" width="100%" height="900px" frameborder="0"></iframe>

**Figure 4**	Views of the posts of various AfD accounts over time. Linear y-axis in the upper diagram, logarithmic at the bottom.

Did only the reach of Alice Weidel's posts experience such rapid growth or does this apply to all AfD members? Figure 4 provides information on this. It shows the views of posts by AfD members (38 in total) and Alice Weidel. At the top it is a linear measure and at the bottom a logarithmic one in which the distances gradually increase. It is clear that Weidel's posts receive many views compared to the other AfD accounts. However, an upward trend can also be seen for the other accounts, which began at the start of December. It is difficult to spot this with the naked eye, so we have also done changepoint analyses for the posts of a few AfD accounts. However, the analysis does not show an increase comparable to that of Weidel. Even though some other AfD members and the official party accounts are experiencing an upswing on X, it is less strong and less sudden.

Musk's reposts and public statements have likely given Weidel reach
What can we conclude from this about the influence of Elon Musk on the reach of the AfD and Alice Weidel? Firstly, we need to explain the limitations of our method. As already mentioned, we collected snapshots of politicians' posts over an extended period of time. For the five discussed here, we have done this more closely since 10 January. This can be seen very clearly in Figure 1, as the points have been closer together since then. On the one hand, however, this means that there are gaps and irregularities in the snapshots and that we can say less about the dynamics before 10 January. In addition, we also have no access to the geographical origin of the users who saw Weidel's post. This would of course be interesting, especially in the context of the upcoming federal elections. In addition to the methodological limitations, however, there is a much more fundamental problem. We have no direct access to the modes of action of X's algorithm. As long as we do not have this, we can only collect data and deduce modes of action by means of circumstantial evidence. We also deliberately see our results only as indications that suggest an explanation, rather than evidence that clearly proves something. Against this backdrop, it is particularly important that the long-disputed obligation to provide access to research data, which is now enshrined in <a href="https://www.interface-eu.org/publications/researcher-access-platform-data-under-dsa-questions-and-answers" target="_blank">Art. 40 of the Digital Service Act</a>, is brought to life. It is a shame that researchers had to wait so long for the Commission's delegated act. <a href="https://ec.europa.eu/info/law/better-regulation/have-your-say/initiatives/13817-Delegated-Regulation-on-data-access-provided-for-in-the-Digital-Services-Act_enBut" target="_blank">But now it is here</a>.

Alice Weidel has rapidly increased both the views of her posts and the number of her followers in the weeks since 16 and 20 December. She has gained almost 400.000 followers in this period - that is more than Friedrich Merz has in total. Her posts also have a greater reach than those of any other German politician. It seems very obvious that this has to do with Musk's activities. The pattern of posts he has retweeted from Weidel in particular suggests this. Her views, on the other hand, were more likely to have been influenced by the frequent mentions by Musk and ultimately the public talk between the two. The most obvious conclusion is that Musk's mentions, retweets and the conversation have given Weidel an increased reach, from which her subsequent posts that are not retweeted by Musk now also benefit. We found no evidence of an adjustment of the algorithm in Weidel's favour, even though it is known that Musk's statements on X are particularly visible and a retweet from him can lead to a shift in discourse. The same applies to other AfD accounts. An increase can be measured for a few of them, but it is less noticeable than for Weidel. Overall, however, it should be noted that the explanations are not mutually exclusive. Just because Weidel's upswing can also be explained by Musk's AfD-friendly posts does not mean that potential changes to the algorithm could not have led to even more, but perhaps more subtle, changes.

**So far, the effect seems to be limited to X**

<iframe src="/Fig_5.html" width="100%" height="900px" frameborder="0"></iframe>

**Figure 5**	Views of posts by various German politicians on Facebook, Instagram, TikTok and X.

Finally, an integration of the results in the larger field of social media platforms. Figure 5 shows the views of Weidel's posts and those of the other four politicians on Facebook, Instagram, TikTok and X. Firstly, it can be seen that the views for Facebook are the lowest and those on the other platforms are still more comparable. You can also see that the views of individual politicians' posts can vary greatly depending on the platform. For example, Scholz is more popular on TikTok than Habeck, but the opposite is true on Instagram and X.

Alice Weidel expressed her thanks to Musk for his article in Die Welt not only on X, but also on the other platforms. These posts often received an exceptionally high number of views. However, it is not unusual for individual posts to receive a lot of coverage. Lindner's TikTok post showing him being attacked with shaving foam also received over 25 million views and individual posts by Habeck or Lindner achieved even more reach on Facebook or Instagram than those by Weidel. Nevertheless, we carried out a changepoint analysis to find out whether Weidel's posts also received more views on other platforms after 20 December. Again, the analysis did not reveal any conspicuous results. So far, we cannot find any strong evidence that Weidel's popularity on X is also spreading to other platforms. As things stand, the Musk effect is therefore limited to X.

We would like to thank Matthias Kettemann for his helpful feedback. The data was last updated on 27/01/2025 and data collection is ongoing. A version of this report was published in German at the Digital Society Blog of the Alexander von Humboldt Institut für Internet und Gesellschaft <a href="https://www.hiig.de/musk-x-und-afd/"  target="_blank">here</a>. A more detailed description of the analysis, the methods, as well as the code and data can be found <a href="https://osf.io/jcqen/" target="_blank">here</a>.
