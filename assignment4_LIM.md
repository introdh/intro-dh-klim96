## Describe the data you selected for your analysis. Assume the reader is unfamiliar with the data.
The data I selected for my analysis are the winners of the Tony Award for Best Original Score and the year they won their award. The data is the awardees from the past 20 years (2017-1997).  Therefore, my nodes are composer/lyricists and years and my edges are “won the award in…”

According to [Wikipedia](https://en.wikipedia.org/wiki/Tony_Award), “The Tony Awards are considered the highest U.S. theatre honor, the New York theatre industry's equivalent to the Academy Awards (Oscars) for film, the Emmy Awards for television, and the Grammy Awards for music." The winners composed their musical’s score and/or wrote the lyrics. To qualify for the Tony Award, the musical must have opened within the past show season which is [typically April-April](http://www.tonyawards.com/en_US/multimedia/calendar/index.html). In addition, [Wikipedia](https://en.wikipedia.org/wiki/Tony_Award) also says that “the score must be written specifically for the theatre and must be original; compilations of non-theatrical music or compilations of earlier theatrical music are not eligible for consideration.”

## Explain the questions/arguments your network generates about your data.
I originally chose this data because in the arts, especially on Broadway, many musicians collaborate with one another. My original goal was to see which musicians have worked with each other and how connected all these famous artists are (“the degrees of separation” on Broadway). For example, the current Best Original Score holders are Benj Pasek and Justin Paul—known professionally as Pasek & Paul—for *Dear Evan Hansen*, but they also wrote the music for *A Christmas Story: The Musical*, which they were nominated for in 2013, and *La La Land*. Musicians do not necessarily have to collaborate with the same people, though; for example, Alan Menken has worked with Jack Feldman (*Newsies*, 2012), Glenn Slater (*Sister Act*, 2011), and many others. 

However, when I ran my initial network in R, my network was not a network at all: it was clusters. Musicians clustered around musicals and a few artists worked with the same people. The driving force behind the clusters, however, was that many musicians had been nominated only once; these are mostly represented as straight lines (edges) with two or three nodes. For example, a few popular artists—Sara Bareilles, Cyndi Lauper, Dolly Parton—have written music for musicals, but their show was their only Broadway project.

![alt text](https://github.com/introdh/intro-dh-klim96/blob/master/Screen%20Shot%202017-12-01%20at%2012.10.27%20AM.png)

Despite the clusters, my first network can be taken as a positive finding. This could suggest that there is not a bias in which composers/lyricists are nominated for the award since there has been a large variety of people who have been nominated instead of the same few people. However, it could also suggest something in the opposite direction: it could mean that some Broadway musicians get their one claim to fame but cannot get nominated again due to industry biases towards certain, more famous artists. The second conclusion may be more plausible because within this past season, many shows have been overly concerned with sales. Earlier this year, Panic! at the Disco frontman Brendon Urie took on the lead role in *Kinky Boots* and singer and Tony-nominated composer/lyricist Sara Bareilles played the lead in *Waitress*; both of their runs [increased their show's ticket sales](http://www.playbill.com/article/grosses-analysis-brendon-urie-gives-kinky-boots-a-lift). *Natasha, Pierre, and the Great Comet of 1812* recently closed due to a [racial controversy](https://www.huffingtonpost.com/entry/great-comet-of-1812-close-casting-controversy_us_598aad74e4b0a66b8bafa576) in which black actor Okieriete Onaodowan, who had just begun his run as Pierre, was going to be replaced with white, award-winning actor Mandy Patinkin in an effort to drive sales after Josh Groban’s departure. Therefore, some composers/lyricists may have received only one nomination because Broadway producers are turning to more famous artists to write music so the show can be financially successful.

Since the composer/lyricist-musical data created clusters, I ran the code with the composers/lyricists and award year. With this data, I found a more fascinating, connected network. There are still clusters, as seen in the top right corner, but these are now anomalies. Now, I can see who has been nominated, how frequently they have been nominated, and who they competed against.
![alt text](https://github.com/introdh/intro-dh-klim96/blob/master/Screen%20Shot%202017-12-01%20at%2012.12.10%20AM.png)

**Some Questions I Can Ask**
- Who is the most frequently nominated composer/lyricist in the past 20 years?
- Which year had the most people nominated for Best Original Score?
- Are there any composers/lyricists who have competed with each other multiple times?
- How long does it take for a composer/lyricist to get “rehired”? (Or, in some cases, reinspired to write a new musical?)

One of the most interesting findings from this network is in regards to the first question. In the past 20 years, Jeanine Tesori has been nominated more times than Alan Menken, John Kander, and Fred Ebb. Tesori has been nominated five times while Menken, Kander, and Ebb have each been nominated four times. Interestingly, Menken, Kander, and Ebb are famous composers and well-known on Broadway; seeing their names multiple times on this list was not surprising to me and I knew who they were before researching the Best Original Score winners. However, I had not even heard of Tesori before this project. Due to their level of fame and familiarity, Menken, Kander, and Ebb most likely had more nominations before 1997. Therefore, this could indicate that Tesori is a star on the rise, which is especially significant since she is a woman in theatre; *Waitress*, which arrived on Broadway in 2016, is the first musical created by an all-female team. Again, this finding could also have a negative conclusion: it is possible that despite all her nominations, Tesori is not a well-known artist because she is a woman. Regardless, Tesori may be part of a movement on Broadway to include more women in the creation of musicals.

![alt text](https://github.com/introdh/intro-dh-klim96/blob/master/Screen%20Shot%202017-12-01%20at%2012.11.19%20AM.png)

## Drawing on the constraints, critiques and ideas in our readings, discuss the possibilities and limits of network analysis as applied to your network and for network analysis generally. Make sure to cite the readers.