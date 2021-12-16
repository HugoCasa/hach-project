# Is the Greta effect fake news?
> *If standing up against the climate and ecological breakdown and for humanity is against the rules, then the rules must be broken.* Greta Thunberg

For years now climate change has been one of the dominating topics in public debate.
Since 2018 the "Friday for Future" movement has taken to the streets in an attempt to be heard by policy makers, led by a young woman from Sweden with a cardboard board.

We will show how the debate was dominated by certain groups of people over the years, how they have been speaking about climate change and what has changed since Greta Thunberg arrived on the stage. In order to quantify the changes, sentiment analysis and language complexity analyis was performed on quotes on climate change from the Quotebank dataset. We will analyze the two years before Greta took off as a person of public interest and the two years after. As she started protesting in Sweden in August of 2018, but newspapers really started paying attention to her in early 2019, we define 2017-2018 as the years before Greta (b.G.) and 2019-2020 are considered after Greta (a.G.). 

> *Speaker announcement : "Ladies and gentleman, welcome on board of the Gretaboat with destination to better world...*

# Let us embark on the Gretadaventure
First things firts : context !
### Female... Male... Where does she stand in the debate ?
What's quite interesting about Greta Thunberg is that she isn't the typcal public speaker profile. She's young and not a male. To support our claim, we decided to explore gender diversity and age distribution in the quotes concerning climate change and how these two variables evolved with time.

{% include plots/gender_piecharts.html %}

We can only observe a small increase in the percentage of women speakers throughout the years. Their quantity remains roughly around 20% which is far from being representative of the population. Other genders were also present in the dataset but their numbers were irrelevant compared to the two dominating categories and were therefore not visible on the graphs which shows again underrepresentation of those groups of people in the quoted speakers.  

### All right, all right, all right, are you going to tell me climate change is a matter of the old now ? 😒

{% include plots/age_plot.html %}

Unfortunately, until now it has been the case... The sample of population speaking about climate change in 2018 is rather old with a mean age of 56 years. The fact that Greta, 16 years old, starts speaking about it, is a game changer, as she stands out from the typical population in this context. We could wonder whether the movement is only aimed at old policy makers, or also at younger generations who will be the future policy makers and could therefore perdure the change.
Even though we see a peak at 21 years old, after some background checking, we've come to realise some inconsitencies in the wikidata and noticed that anyone older than 21, for whom we did not have age information, were given the 21 years old label. 

### She was quoted a lot, like a loooooot. But how much is that ?

{% include plots/greta_quoted.html %}

Greta first appeared in the media around september 2018 and the number of times she was quoted ever since is simply mindblowing. Started from the bottom in 2018 and in 2019 she was not only in the top 10 most quoted speakers of year in the climate change category, but she was number one. (This was a long sentence, sorry for that.) <br>
{% include plots/top_speakers.html %}
<br>
This simply shows how much of an issue climate change is and how her approach changed debate. Like it literally changed everything. 🤯 **Boom** there you go ! <br>
Now, the moment you've all been waiting for... The award of the 2019 most quoted quote (some many "q's" 🦆 quack). And it goes tooooo :
> *School strike for the Climate.* Greta Thunberg

It was quoted 727 times. Same quote. 727 different news media articles. Take that !
<br>

# Greta sailing over the big pond
On 14th August 2019, Greta left Plymouth on a boat in a trip to New York that lasted 15 days. Could you imagine that ? 15 days on the sea on a small boat ? That takes quite the courage ! 😱
She did this, so that she could reach the US to attend the 2019 UN Climate Action Summit and remain carbon neutral. Quite the project, huh ?
So, did Greta make America great again ? 🇺🇸

### Hello there old friend
Remember where we are (small hint : 🇺🇸) and where we came from (another hint : 🇪🇺). How do the two old friends compare in the climate change topic ?

{% include plots/europe_us_complexity.html %}
{% include plots/europe_us_sentiment.html %}

Clearly, we, Europeans (yey 🥳) find ourselves better ranked in terms of complexity of language as well as in terms of mean sentiment when talking about climate change. This could have many explanations, such as a difference in the average level of education, but we have found something interesting that could also have its impact : average quote length. Indeed, US quotes tend to be shorter and some positive correlation can be oserved between the complexity of quotes and their length.

{% include plots/europe_us_quote_length.html %}

Does this mean we can say Europeans are smarter ? 😃 Let us not jump into conclusions, but let us secretly believe in that. For now.

### The war of the home parties
Sorry to bring to you this way, but it is no breaking news the two main parties in the US (Democrats and Republicans) are two political opposites fighting against each other. It has been this way for ages and we are still far from a change. Enough blah blah, a picture is worth a thousand words, how do they reaaally compare when it comes down to climate change ?

{% include plots/republican_democratic_sentiment.html %}

The mean sentiment linked to the Democrats is on average higher than the one linked to the Republicans. We cannot say we are surprised, as climate change was not really a top priority of Donald Trump's program since 2017. As we all remember, he withdrew from the Paris climate accord on 1st June 2017, we believe that made it quite clear. 😞

### This one looks like a boxing match final round : Greta vs Trump
Now that we have some context, we can finally reach the pinnacle of comparisons, i.e. the most opposite political figures, i.e. the MVPs. Ladies and gentlemen, please welcome Greta Thunberg and Donald Trump :

{% include plots/republican_democratic_sentiment.html %}

We can safely make the statement that these results do not come as a surprise.

# After this, everything is a work in progress (in artist language we say WIP)



# Natural disaster

# Testing plots

p.s. : Climate change was quoted 57 times in this article. Do you believe us ?
<br>
<br>
p.p.s : You checked the number, didn't you ?
<br>
<br>
p.p.p.s : Thank you for reading !
