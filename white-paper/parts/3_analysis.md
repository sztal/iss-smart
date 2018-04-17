
# Analysis

## Data preparation
First, the data will be prepared for the main analysis. For each country corpus
a subset of documents related to politics, economy and social issues
(as opposed to articles on topics such as science and technology, culture or fashion)
will be determined.

## Sentiment analysis
Each document will have a sentiment score assigned to it. Bipolar positive-negative
scoring will be used, so every document will be described not only in regard
to what topics it discusses but also in regard to emotional valence of its content.
It is most likely that dictionary-based sentiment analysis techniques will be used.

## Topic modeling and narrative discovery
Document corpuses will be used as input data for topic modeling procedures.
We plan to use _Latent Dirichlet Allocation_ (LDA) as our main algorithm for topic
discovery. This is a modern and industry tested technique that can cope with
most of the technical difficulties typical for topic modeling problems
(such as word polysemy) [@Blei2003; @Kosinski2016].

It is quite likely that the first step of the analysis based on LDA will lead to
discovery of wide arrays (tens, hundreds or even thousands) of particular
topics that are too specific to be considered narratives. In such a case
an additional step will be introduced and data dimensionality will be reduced
using the PCA algorithm [@P.Murphy1991].
As a result much smaller sets of higher-order topics will be discovered
and these topics could justifiably be considered narratives.

## Narratives interpretation
Discovered narratives will be subsequently interpreted. This part of the analysis
will be based on mixed methods approach. First, quantitative summary reports
will be prepared for every narrative. The reports will focus on basic high-level
summarizations such as distributions of words and phrases, also presented
graphically via word clouds and/or semantic networks. Additionally informational
measures such as `tf-idf` [@Anand2011] will be used to identify words and phrases
that are most specific and descriptive for a given narrative.

The final stage will be dedicated to qualitative analysis of random samples of
texts typical for specific narrative by experts with a sound knowledge of politics,
social issues and media landscape of a given country. Their work will be facilitated
by quantitative reports which are supposed to provide useful hints for
interpreting narrative data.

## Estimating shared and conflictual parts of discoursive spaces
Description of narratives will serve as a starting point for additional analysis
that will focus on identifying the most conflictual and shared narratives.
Every actor (publisher) will be described in regard to every narrative in terms
of importance of this narrative (i.e. how often the actor discusses it,
its popularity in social media etc.) and sentiment towards it
(what is the emotional attitude to it). This will enable
identification of clusters of actors that tend to think similarly and
differently about a given issue/narrative.
