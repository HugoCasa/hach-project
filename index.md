![Greta vs Trump](/assets/images/cover-image.jpeg)
<br>*Source: Ian Baker*

# Is the Greta effect fake news?
>> *"If standing up against the climate and ecological breakdown and for humanity is against the rules, then the rules must be broken."* Greta Thunberg

For years now climate change has been one of the dominating topics in public debate.
Since 2018, the "Friday for Future" movement has taken to the streets in an attempt to be heard by policy makers, led by a young woman from Sweden with a cardboard board.
<br>
We will show how the debate was dominated by certain groups of people over the years, how they have been speaking about climate change and what has changed since Greta Thunberg arrived on the stage. 
<br>
In order to quantify the changes, sentiment analysis and language complexity analysis were performed on quotes on climate change from the Quotebank dataset. 
<br>
We will analyze the two years before Greta took off as a person of public interest and the two years after. She started protesting in Sweden in August of 2018, but newspapers really started paying attention to her in early 2019. We define 2017-2018 as the years before Greta (b.G.) and 2019-2020 are considered after Greta (a.G.). 

> *Speaker announcement : "Ladies and gentleman, welcome on board of the Gretaboat with destination to Better World..."*

# Let us embark on the Gretadaventure
Let's start with some context on the debate before like who was being quoted on climate change in the years b.G and if anything has changed with Greta? 

> We will take you along Greta's journey to explore the world of the climate change debate. We will see what she encountered when she answered her calling as role model for a whole generation, how Europe and the US are indeed two very different places and what Trump and Greta have in common. 

### Who is speaking about climate change?
We found that Greta doesn't belong to the typical speaker quoted on climate in the Quotebank dataset. She's a young woman, not a politician and from a country with a rather small population in Europe. 
<br>

Let's start by taking a look at the distribution of the gender of the quoted speakers over the years. 

{% include plots/gender_piecharts.html %}

We can only observe a small increase in the percentage of women quoted throughout the years. It remains at roughly 20% which is far from being representative of the population. Other genders were also present in the dataset but their numbers were irrelevant compared to the two dominating categories and were therefore not visible on the graphs. This shows again underrepresentation of some groups of people in the quoted speakers. 

### A topic for old men?

{% include plots/age_plot.html %}

Ah, we see here that indeed the majority of speakers tend to be older rather than younger... 
<br>
The sample of population speaking about climate change in 2018 has a mean age of 56 years. The majority of speakers in the dataset are politicians and it's biased towards english speaking news, so this doesn't come as a big surprise.

> The years before Greta (b.G): The years before Greta are characterized by a lot of old men speaking about climate change. 

<br>
The fact that Greta, 16 years old, is being quoted about climate change is a game changer, as she stands out from the typical population in this context.
We wonder if this change will persist, or if she is just an exception that proves the rule. 
<br>
After some background checking, we found that due to some inconsistencies in the wikidata every speaker without any entry for age is attributed an age of 21 years. This explains the peak of 21 year olds being quoted on climate change.

> The years after Greta (a.G.): We hoped to see some change in the years after Greta (2019 and 2020) in terms of distribution of age and gender of the speakers.

### How many times is Greta actually quoted ?

{% include plots/greta_quoted.html %}

Greta first appeared in the media around september 2018 and the number of times she was quoted ever since is simply mindblowing. Starting from the bottom in 2018, by 2019 she was not only in the top 10 most quoted speakers of year in the climate change category, but she was number one.  <br>
{% include plots/top_speakers.html %}
<br>
This shows that she must have had an impact on the debate. Everyone was starting to quote the young swedish woman. She even overtook Donald Trump. 😳
<br>
This leads us to the moment we've all been waiting for... The award of the 2019 most quoted quote goes too :
>> *"School strike for the Climate."* Greta Thunberg

It was quoted 727 times. Same quote. 727 different news media articles. That's a lot!
<br>

# Greta sailing over the big pond
On 14th August 2019, Greta left Plymouth on a boat in a trip to New York that lasted 15 days. Could you imagine that? 15 days on the sea on a small boat? That takes quite the courage! 😱
<br>
She did this, so that she could reach the US to attend the 2019 UN Climate Action Summit and remain carbon neutral. Quite the project, right?
What did she find when she sailed across? 

### A warm welcome

> Greta has now reached the USA, but how do the US and Europe compare when it comes to public debate about climate change? 

<br>
In order to find out about the differences we analyzed the quotes over the two years b.G and a.G. and compared the US to Europe. 

{% include plots/europe_us_complexity.html %}

The complexity of the scores were generated using the textstat library using the standard text scorer. For example, a score of 9 means that the quote can be read and understood by an average 9th grader. 
<br>

>To demonstrate the scorer, let's take a look at a random quote from the US and from Europe.
>> *"Understanding and predicting future changes in tropical rainfall patterns is one of the greatest and most important challenges facing climate science today"* John Marshall, complexity: 15.0
>
>Let's see what the US have to say: 
>> *"We have these questions about climate change but we have no direction yet on what we should in fact say. So, we wrote very wishy-washy answers and they got submitted to Secretary Mattis's team. And they came back to us and said, `These are too weak. Secretary Mattis believes in climate change and the risk to national security."* Maureen Sullivan, complexity: 8.0
>
>Reading them one can already guess that the second quote from the US scores lower, but why is that? 
>
>It cannot be due to the length of the quote, as it is much longer and still scores lower than the first. The scorer we used for the analysis is based on multiple functions that take into account number of words, complex words, and sentences. A possible explanation for the difference in complexity could be for example that the  'wishy-washy answers' in the second quote score lower than the 'tropical rainfall patterns' from the first quote. 

And what about the sentiment on climate change? Might there be a difference in how the US and Europe feel and speak about this topic?

{% include plots/europe_us_sentiment.html %}

>Let's generate another pair of random samples to see how they score sentiment wise. 
>
>>*"Withdrawing from the Paris climate agreement is bad for the environment, bad for the economy, and it puts our children's future at risk,"* Mark Zuckerberg, sentiment score: -0.9991
>
>>*"The European Union must align our climate and energy policy according to the 1.5 ° C [ rise in average global temperatures ] target. That means that the EU must achieve carbon neutrality by 2050,"* Kimmo Tiilikainen, sentiment score: 0.8459

The first quote from the US scores much lower in terms of sentiment than the latter. This is in line with our subjective perception of the quotes. 

Clearly Europeans find themselves higher ranked in terms of complexity of language as well as in terms of mean sentiment when it comes to talking about climate change.
Nevertheless, let's not jump to conclusions what this has to say about the difference between the US and Europe.
<br>

Greta now faces an entirely different bunch of speakers, who are much more negative and less complex in the way they speak about climate change. 
Moreover, only two big players stand out in the politics game. The next step is therefore to figure out how the two major parties in the US behave.

### The war of the home parties

It is no big news that the two main parties in the US (Democrats and Republicans) are two political opposites fighting against each other. It has been this way for ages and we are still far from a change. How do they compare when it comes to the topic of climate change ?

{% include plots/republican_democratic_sentiment.html %}

The mean sentiment linked to the Democrats is on average higher than the one linked to the Republicans. This isn't a big surprise, as climate change was not really a top priority of Donald Trump's program since 2017. As we all remember, he withdrew from the Paris climate accord on 1st June 2017, we believe that made it quite clear.
<br>
And how do the two major parties compare in terms of complexity?

{% include plots/republican_democratic_complexity.html %}

Interestingly enough, there doesn't seem to be a large difference between the two parties. Especially not as large as the difference between the US and Europe. 
<br>
Let's look at the end boss of the final level of Greta's journey.

### Greta vs Trump

Now that we have some context, we can finally reach the pinnacle of comparisons. Ladies and gentlemen, please welcome Greta Thunberg and Donald Trump :

{% include plots/greta_vs_trump.html %}

There isn't such a big difference in complexity and sentiment for the two speakers.
<br>
Even though the republicans seem to have a lower language complexity score on average, Trump seems to be higher on that scale. This is surprising, as Trump does not usually shine because of his well thought through statements. 
The fact that Greta's language complexity is so low could be explained by the fact that english is not her mother tongue and her age.
<br>
These results become interesting when we look at the sentiment score. 
Greta starts off very positively in 2018 and endures a severe fall in only a few months time to join Trump's levels and remain there until 2020. This phenomena could be due to the fact that Greta appeared as a light in a dim world, by bringing to the table the topic of climate change. 
We believe the sentiment of her quotes dropped because of the fact that she quickly started bringing forward the consequences of climate change and to insist on how hopeless the current politics was. So, how could you link a positive sentiment with hopeless thoughts you wonder ? Well, clearly it is impossible.

## Are we not forgetting something here? Duh, Climate Change! 

Greta was of course a tour de force but what else might have had an impact on the public climate change debate?

# Natural disaster

> Have you ever heard of Imelda? 
>
> She was a tropical storm that hit the US in September of 2019. She caused a lot of flooding in Texas and hence also damage to property.

The plot below shows the total damage to property in the US caused by weather events over the years. Additionally, it shows the weighted sentiment score over time. In this way we can explore how extreme weather events may have an influence on the climate change debate. 

{% include plots/damages_weighted_sentiment.html %}

It seems like natural disasters have an impact on the climate change debate. This doesn't come as a great (greta) surprise, but how much the curve of weighted sentiment follows the damage to property is still impressive. 
The first peak in damage to property was the tropical storm Imelda, whereas the second even higher peak in November 2019 was thunderstorms in Texas causing a lot of damage. 
<br>
We believe that these natural disasters cause the public debate about climate change to heat up again. Politicians, who are the most quoted group in the dataset, are quoted on this subject a lot when an extreme weather event has happened. But how can the weighted sentiment give us any indication about the public debate?
<br>

>Let's see how different example quotes score in terms of sentiment: 
>
>> *"Climate change is real"*, sentiment: Positive, 0.9976
>> 
>> *"Climate change is an urgent matter"*, sentiment: Positive, 0.9773
>> 
>> *"It's time to act on climate change"*, sentiment: Positive, 0.9962
>
>We can see from these few example quotes that even though they convey a message of urgency, they still score positively. 

>An example quote from October 2019 from the US shows the same thing: 
>
>>*"New Jersey is extremely vulnerable to the impacts of sea-level rise and global warming, and today's executive order outlines a bold and comprehensive set of actions to ensure that our communities and infrastructure are more resilient against future storms"* Phil Murphy, sentiment score: Positive, 0.998
>
>Even though the speaker is speaking about the recent events and the urgency to act, the overall sentiment is positive. 

One might expect the weighted sentiment score to fall after natural disasters. However these examples show, that after events like tropical storms that cause a lot of damage, when the debate about climate change is likely to fire up again, the weighted sentiment score can still rise. 
As the weighted sentiment score weighs the number of times a quote was used additionally to it's sentiment, it gives a clear picture of the debate at any point.
<br>

Let's see how Greta and Trump compare with these two measures: 


{% include plots/damages_weighted_sentiment_greta_trump.html %}

Ah, it seems like when there is a lot of damage to property, Greta's positive quotes are used a lot. This strenghtens our assumption that these natural disasters have an impact on the climate change debate and who is quoted on this topic.

# Bringing it home

We embarked on a climate change journey in a mission to understand the context of debate and how it evolved around the topic for the past years. More specifically, we followed Greta’s path as she has been one of the leading speakers on the topic of climate change since the beginning of 2019 and tried to identify her impact in the situation.
<br>
We have discovered she arrived to a debate dominated by old men and initially believed she might have ignited a spark of revolution that could’ve changed the discussion around climate change on a global scale.
<br>
We then sailed with Greta over the big pond to investigate how the US compare to Europe in terms of language complexity and sentiment on the topic of climate change and found that in Europe the discussion is often linked with more complexity and on average with more positivity than in the US. We tried pushing the comparison further by focusing on someone at the other end of the political spectrum, namely Donald Trump. We found that the quotes of these two speakers don’t differ too much in terms of sentiment and complexity regarding climate change.
<br>
Finally, we tried to turn the problem upside down and look for other potential game-changers, so we looked into extreme weather events in the US. We performed an analysis on the correlation of extreme weather events with change in sentiment over the years and obtained an interesting result: there is a correlation between weather events and the weighted sentiment sum of all climate quotes.
<br>

It's impossible to think about the climate change debate these days without thinking about Greta Thunberg. Even though she didn't fundamentally change the demography of who is being quoted on climate change, she became the top speaker on the topic in a matter of months. Her impact on the debate reaches further than just the Quotebank dataset. 
<br>
We found that what might have an actual longer lasting impact on the climate change debate, is the climate itself. We saw how the natural disasters and the damage to property caused a peak in the weighted sentiment score, as there was an increase in urgency about the topic. 
<br>
<br>
p.s. : Did you know we used the words "climate change" 40 times in this page ?
<br>
<br> 
p.p.s. : You checked the number didn't you ?
<br>
<br>
p.p.p.s. : Thank you for reading this far !
