---
layout: page
title: Statistical and Neural Computational Linguistics
tagline: University of Rochester (Spring 2019)
---

# Project Ideas

Below is a list of potential projects for [Statistical and Neural Computational
Linguistics](index.html) (LIN281) at the University of Rochester in Spring 2019.

## Sounds

If you are interested in doing a project looking at linguistic sound systems,
you might consider investigating models for induction of phonetic (and/or tonal)
categories or phonotactic rules.

### Phonetic and Tonal Categories

In class, we read about models for inducing phonetic categories from acoustic
measurements, such as vowels' first and second formants. Using only these
acoustic measurements filters out much of the acoustic variability inherent in
real sound. A slightly more realistic model would use richer measurements of the
entire signal, such as the signals's
[spectrogram](https://en.wikipedia.org/wiki/Spectrogram) or its [mel-frequency
cepstral coefficients](https://en.wikipedia.org/wiki/Mel-frequency_cepstrum)
(MFCCs). Indeed, MFCCs are what is often used in automatic speech recognition
(ASR) systems, like those built using the [Kaldi
toolkit](http://kaldi-asr.org/).

(Check out Eleanor Chodroff's [tutorial on
Kaldi](https://eleanorchodroff.com/tutorial/kaldi/index.html) if you're
interested in ASR. [This
tutorial](https://haythamfayek.com/2016/04/21/speech-processing-for-machine-learning.html)
on basic audio processing using the scipy stack is also nice.)

One potential project is to connect one of the phonetic category induction
models we cover in class with a model that can automatically extract features of
the acoustic signal that are relevant to phonetic categorization. My suggestion
would be to try using [convolutional neural
networks](https://en.wikipedia.org/wiki/Convolutional_neural_network) (CNNs) for
this purpose by jointly training a CNN to extract acoustic features from
spectrograms or MFCCs for different phonetic categories and cluster those
features using some sort of mixture model. This sort of model might also be
useful for inducing tonal categories in languages that have them, though
separating phonetic and tonal categories may be somewhat difficult in an
unsupervised model.

### Phonotactic Rules

In class, we read about models for inducing phonotactic rules from sequences of
phones and/or phonological feature valuations. A phone's phonological features
correspond to states of the articulators used to form the phone, but these
features must themselves be inferrable from the acoustic properties of the phone
in some way.

One potential project is to build a model for inducing phonological feature
valuations directly from segmented speech input -- i.e. audio with
transcriptions indicating where a particular phone starts and stops (or at the
very least, where a particular word or sentence starts and stops). My suggestion
would be to try using a combination of CNNs and [recurrent neural
networks](https://en.wikipedia.org/wiki/Recurrent_neural_network) (RNNs) for
this purpose by jointly training a CNN to extract acoustic features from
spectrograms or MFCCs for different phonetic categories and using those features
as inputs to an RNN predicting phones as outputs. The RNN internal states might
then be interpretable as phonological features and the RNN transition matrices,
as phonotactic rules.

## Words

If you are interested in doing a project looking at word formation, you might
consider investigating models for morphological parsing or morphological
generation. If you are interested in word semantics, you might consider
investigating models of word sense.

### Morphological Parsing and Generation

In morphological parsing, we aim to build systems for mapping input words to
their root form (or forms, in the case of compositional compounds) and the
morphological features of the bound derivational and lexical morphemes
associated with those roots; and in morphological generation, we aim to take
root form(s) and morphological features as input and produce a word. Models
relevant to this goal have been investigated extensively within the [SIGMORPHON
shared tasks](https://sigmorphon.github.io/sharedtasks/), which use the
[Universal Dependencies](https://universaldependencies.org/) treebanks and
[Unimorph](https://unimorph.github.io/) banks.

One potential project is to investigate current state-of-the-art (SOTA) models'
ability to handle morphological phenomena in different language families. I
would suggest focusing on differences in the relative
[agglutinativity](https://en.wikipedia.org/wiki/Agglutinative_language) of
different languages found in Unimorph, though other typological features of the
language could be interesting to look at. The [World Atlas of Language
Structures](https://wals.info/) would be a useful additional resource here. If
you go this route, my suggestion is to look at the relative performance of SOTA
systems as a function of those typological features.

### Word Sense

Many words have multiple potential senses. Ambiguous words like "bank" – which
has both "financial institution" and "side of a river" senses – are a typical
case of this; words that undergo *regular polysemy* are another. A classic case
of this is what is the *unit-type ambiguity* – e.g. "book" can be used to refer
either to a particular physical instantiation of a book or to the abstract
contents of a book. This latter sort of ambiguity seems to be rule-governed in
an important way – e.g. many objects that contain informational content undergo
it.

One potential project is to investigate how to capture the difference between
rule governed ambiguity and non-rule governed ambiguity in a computational
model. My suggestion is to build off current models for word sense
disambiguation (WSD) by building a notion of regular polysemy rule into the
relationship between different word senses. Two potentially useful datasets for
this purpose are the [Universal Decompositional Semantics Word Sense
dataset](http://decomp.io/projects/word-sense/), which contains annotations of
nouns in context for word sense based on the senses listed in
[WordNet](https://wordnet.princeton.edu/), and the [Universal Decompositional
Semantics Generics dataset](http://decomp.io/projects/genericity/). A
straightforward model for this might take a pretrained language model like
[BERT](https://github.com/google-research/bert) and predict word senses and
genericity based on the model's hidden states.

## Sentences

If you are interested in doing a project looking at sentences, you might
consider investigating models for predicting sentence grammaticality and
acceptability, thematic roles, or veridicality.

### Grammaticality and Acceptability

An important type of data for many generative and constraint-based approaches to
syntactic theory are acceptability judgments, which are believed to be
influenced, at least in part, by a sentence's grammaticality. One question is
how much about a language's syntactic structure we can infer from acceptability
judgments.

One potential project is to investigate models for predicting sentences'
acceptability based on features of the sentence. There are now a variety of
publicly available acceptability judgment datasets, including the
[MegaAcceptability dataset](http://megaattitude.io/), the [Corpus of Linguistic
Acceptability](https://nyu-mll.github.io/CoLA/), and various datasets collected
by [Jon Sprouse](https://sprouse.uconn.edu/) and others. My suggestion would be
to choose a particular syntactic phenomenon and analyze different neural models
ability to capture that phenomenon.  

### Thematic Roles

Thematic roles are an important component of explanations for how we map the
participants in some event or state onto structural positions relating to a
predicate describing that event or state. Such an explanation is called a
*linking theory*. A major question in the literature on thematic roles is what
kinds of data structure they are and how that affects the mapping from
participants to syntactic positions.

One potential project is to investigate models of thematic roles based in the
linguistics literature. My suggestion would be to build on previous models using
the [Universal Decompositional Semantics Semantic Protoroles
dataset](http://decomp.io/projects/semantic-proto-roles/) by implementing
different sorts of linking theories on top of these models.

### Factuality

There are many linguistic indicators of whether the events or states we are
describing in a sentence actually happened or not. One important indicators
comes from clause-embedding predicates, such as *know* and *think*. To know that
something happened, it has to have happened – so we say that "know" is veridical
– whereas to think that something happened, it need not – so we say that "think"
is not veridical. There turn out to be a lot of clause-embedding verbs with
various complex behaviors. Consider "remember": not remembering that something
happened still means it happened, while not remembering to do something means
you didn't do it.

One potential project is to investigate models for predicting how different
predicates interact with the syntactic structures that surround them to give
rise to different veridicality behaviors. My suggestion is to try training
a simple event factuality prediction model to predict the veridicality judgments
in the [MegaVeridicality dataset](http://megaattitude.io/data/) and then probe
the internal representations of that model.
