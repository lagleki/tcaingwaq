# TCAINGWAQ
by uakci

## Table of Contents

1. Introduction
  1. Design goals
  2. Why not taking on Lojban's solution?
  3. Licensing and forking
2. Phonology
  1. The sounds
  2. Syllable shape
3. Morphology
4. Basics
  1. "Verbs" and English
  2. Your first sentence
  3. Me and you
  4. More connections
  5. The ABCs
  6. Relation triangles
  7. Unary connections
  8. Numbers
5. Words' words
  1. My name and my words
  2. Someone's words
6. The abstract world
  1. Events
  2. Traits
  3. Facts
  4. Other uses of the patterns
  5. Coersion
8. Lexicon
9. Sample texts

## 1. Introduction

### 1.1. Design goals

* to be a logical language; to be based on predicate logic
* not to be a relex (like original Lojban which was basically Loglan); be a standalone loglang
* to be concise and practical in use; to be based on easy, short and universal patterns

### 1.2. Why not taking on Lojban's solution?
The answer is simple - it's against our design goals. Lojban has impractically large syllables at times, long predicates and lots of "lo" that could be removed with one swipe. Also, many solutions are counter-intuitive and still aren't resolved.
Thus, Tcaingwaq shall try it afresh.

### 1.3. Licensing and forking
I hereby declare that the language belongs to the open domain. You're free to copy and modify this document and even use the same name without any permission (but I'd like to be notified).
Forking is the thing that keeps the language alive. You are free to fork this.

## 2. Phonology

### 2.1. The sounds

There are:

* five wovels: /a/ \<a\>, /i/ \<i\>, /u/ \<u\>, /e/ \<e\>, /o/ \<o\> (pronounced approximately "ah", "ee", "oo", "eh", "oh"; without the extra bits English tends to add)
* two so-called semivowels: /w/ \<w\>, /j/ \<y\> (pronounced as "w" and "y" as in "wine" and "yet")
* sixteen consonants: /p/ \<p\>, /b/ \<b\>, /t/ \<t\>, /d/ \<d\>, /k/ \<k\>, /g/ \<g\>, /r/ \<r\>, /n/ \<n\>, /m/ \<m\>, /ŋ/ \<q\>, /s/ \<s\>, /z/ \<z\>, /ʃ/ \<c\>, /ʒ/ \<j\>, /h/ \<h\>, /l/ \<l\> (\<q\> is pronounced like "ng"; \<c\> - "sh"; \<j\> - "zh")

All the sounds can be pronounced differently, as long as they can be clearly distinguished.

### 2.2. Syllable shape
The syllables always have these parts (in order)

* all consonants expect l/n/q or a pair of consonants AND/OR an optional j/w 
* a vowel or a diphtong (pair of vowels)
* an optional l/n/q

For example: `ga`, `bra`, `wo`, `gaun`, `dryauq`

## 3. Morphology

There are two word shapes: verb, particle. A particle is a small word carrying not meaning, but grammatical significance.

The particle shape: one syllable without an -n/l/q at the end e.g. ge, ba, brau, bryoi

The verb shape: syllable(s) with -n/l at the end + a syllable with -q or nothing at the end; *or* a syllable with a -q at the end e.g. `ganbei`, `brulfa`, `guljeldjenmelfelpye`; `daq`, `fryauq`

## 4. Basics

### 4.1. "Verbs" and English
A Tcaingwaq verb differs greatly from an English verb. It can stand for what in English is an adjective or a noun, and works like a sentence with slots to be filled in.
Let's look at an example of a verb:

* `taq` - A talks to B about C

We have three slots: A, B and C. All of these slots represent objects (the talker, the one talked to and the topic) essential for the concept of talking.
Let's have a go at another verb:

* `palkei` - A is a potato from plant B

As we can see, this verb is more 'nouny', yet it functions as a verb.

### 4.2. Your first sentence
Now, enough talk about verbs, let's get to know how to use them.
To say that there is a thing that matches the A's of both verbs, we put them one after another. So:

* `taq palkei`  
 talk.A potato.A  
 "there is a thing that talks and is a potato"; "talking potato"; "a potato talks"

Now, you may wonder, is there some meaning to the word order? Does this example signify that a talker is a potato, but not the other way? Well,

* `palkei taq`  
 potato.A talk.A  
 "there is a thing that is a potato and talks"; "talking potato"; "a potato talks"

those statements are equivalent.

### 4.3. Me and you
Let's move on to some more complex sentences. What about us? Me and you, we all express our actions using words like "me" and "you". In Tcaingwaq, those are verbs too! You thought it couldn't get crazier, right? Let's introduce `wa` and `fe`:

* `wa` - A is me, the speaker
* `fe` - A is you, the listener

So, it's very easy to say "I talk" or "you're a potato":

* `wa taq`  
 me.A talk.A  
 "I talk"
* `fe palkei`  
 you.A potato.A  
 "You're a potato"

### 4.4. More connections
Now, the problem with the sentences so far is that "X is Y" is the limit of what we can accomplish. Suppose we want to say, "I talk to you". In order to do that, we need to access the B of `taq`. But how? Let's try this:

* `wa taq fe` (incorrect!)  
 me.A talk.A you.A  
 "I talk. You (...)"

The problem here is that the verbs always group in two, so that one can conveniently express sentences one after another. Here, `wa taq` groups into one sentence, and `fe` starts another. Yet, the other part of the second sentence isn't there, so the sentence awaits completion (or is ungrammatical).
We need a way to express that B, the one to whom I talk. We need a verb for that:

* `wo` - repeat the preceding verb (or another `wo` if present), using the first open slot

This lets us break down a sentence into two: "I talk. You are the person talked to". The difference between this rough translation and what we're trying to say is that the two "talk"s are refering to the same relation. Let's proceed to the sentence:

* wa taq wo fe  
 me.A talk.A \*talk.B you.A  
 "I talk; and the talker of that is you"; "I talk to you"

Here, the referentiality is marked with an asterisk (\*).

If there's more than just one thing to glue, you can repeat `wo`. For example:

* wa taq wo fe wo palkei  
 me.A talk.A \*talk.B you.A \*talk.C potato.A  
 "I talk to you about a potato"

### 4.5. The ABCs
So, you know how to "glue". But how can you refer to the Bs and Cs individually? That's the job of a series of these particles:

* `yu` - use the B slot of a verb
* `ju` - use the C slot of a verb

These particles follow the verbs to choose the desired slot. Let's talk about potato plants:

* `taq-ju palkei-yu`  
 talk-C potato-B  
 "A topic of conversation is a potato"; "I'm talking about potatoes"
 
You may have this question now: how did that "I" slip into the translation? Vagueness. The sentence is vague, that is, the talker isn't specified. It could be me, that rock or the same potato. When a slot isn't specified, it's ignored.

### 4.6. Relation triangles
It sometimes is that we want to express a relation of three verbs. For example, while "weird potato" (`heq palkei`) is a relation of two verbs, "weird talking potato" is of three. Yet, we need a way to have such a relation. In order to stick a third verb to form a triangle, use the word "ro":

* `ro` (RO) - add a third (fourth...) verb to a connection

Now, "weird talking potato" would be:

* `heq taq ro palkei`  
 "weird talking potato"

### 4.7. Unary connections
While we can now handle cases with two, three, four, and even more connections, we haven't yet discussed the case in which there's just one connection to be made. This is not correct:

* `palkei` (incorrect!)  
 "potato (...?)"

A second verb `palkei` would attach to is expected; thus, this sentence is incomplete. In order to make a sentence "Something is a potato", we have to pretend it's a binary connection by using `co`.

* `co` (WO) - vague verb

`co` doesn't mean anything. It can stand for any verb and any relation. Now we can say:

* `co palkei`  
 "something is a potato"
* `palkei co`  
 "a potato is something" = "something is a potato"

### 4.8. Numbers
[TODO]

## 5. Words' words

### 5.1. My name and my words {FIX!!!}
First, let's learn how to use names. How does one say "name"? In Tcaingwaq, it is:

* `naiq` - A is the name of B given by C

But how to quote a name to use it with naiq's A? And how to name things with their real names?

The answer is simple - make the name a Tcaingwaq verb! Examples:

* Alexander > `hanrensanda`
* [TODO]

The overall pattern is simple: disperse the name into simple syllables, then add -n to all of them (except at the end).

### 5.2. Someone's words
[(quoting) TODO]

## 6. The abstract world {FIX!!!}

### 6.1. Events

It sometimes is that we want to refer to some particular event. In order to do that, it's not sufficient to put two verbs next to each other. We need a particle! This time, it is `so` of the new class SO:

* `so` (SO) - turns connection into verb: A is the event of [the connection]

Let's have a look at some examples:

* `wa diaq wo so fe beq`  
 me.A see.A | \*see.B the.event.of(you.A eat.A).A  
 "I see an event of you eating"; "I see that you eat"
* `so fe palkei heq`  
 the.event.of(you.A potato.A).A weird.A  
 "There's a weird thing that is the event of you being a potato"; "That you're a potato is weird"
 
There's also a YU version of `so` for convenience, `zo`:

* `diaq kioq-zo`  
 see.A die-event.A  
 "I see someone's dying"; "I see death"
 
While `kioq` is "A dies by standard B", `kioq-zo` is "A is B's dying by standard C". That makes it mean "someone's dying/death" in this context.

### 6.2. Traits
Traits are like events, but differ in usage. They have an assumed slot for a verb to be passed in. Just like in real life, traits are possessed by things, and so a Tcaingwaq trait is possessed by all the things the verbs of which fit into the slot. Because of the nature of traits, a different syntax is used. Thus, let's introduce the class YU's member, `su`:

* `su` (YU) - turns verb into verb: A is the trait of [verb]-ing ([verb]'s non-A places follow)

For example, if verb `taq` is "A talks to B about C", then `taq-su` is "A is the trait of talking to B about C".
Let's piece up a simple example:

* `hyoiq-yu taq-su wo fe`  
 want-B talking-trait.A \*talking.trait.B you.A  
 "I want (to have the) trait of talking to you"; "I want to talk to you"

### 6.3. Facts
There are things that may not be the truth, but we want to express anyway.

## . Lexicon

### Particles:
* co (WO) - vague verb
* fe (WO) - A is you, the listener
* gu (YU) - use the D slot of a verb; this word doubled/tripled/... refers to the E/F/... place
* ju (YU) - use the C slot of a verb
* na (YU) - signifies that the preceding verb is actually a name
* ro (RO) - add a third (fourth...) verb to a connection
* so (SO) - turns connection into verb: A is the event of [the connection]
* su (SU) - turns verb into verb: A is the trait of [verb]-ing ([verb]'s non-A places follow)
* wa (WO) - A is me, the speaker
* wo (WO) - repeat the preceding verb (or another "wo" if present), using the first open slot
* yu (YU) - use the B slot of a verb
* zo (YU) - turns verb into verb: A is the trait of [verb]-ing of (... [verb]'s places follow)

### Classes:
* RO - connects a connection to the following verb
* SO - turn following connection into verb
* WO - act just as verbs
* YU - modify preceding verbs

### Verbs:
* beq - eat - A eats B
* diaq - see - A sees B by means C (relation of A and B)
* gwaq - language - A is a language that expresses B (idea) as C (quote)
* heq - weird - A (event) is weird to B because of its C (trait)
* hyoiq - want - A wants B (event/trait, not object)
* koiq - die - A dies by standard B (trait determining death)
* naiq - name - A (quote) is the name of B given by C
* taq - talk - A talks to B about C
* tcaingwaq - Tcaingwaq - A is of Tcaingwaq in trait B
* tcaiq - different - A is different than B
* palkei - potato - A is a potato from plant B
* sfuq - trait - A (trait) is a trait of B; B is A-ish
* syoq - happen - A (event) happens

## . Sample texts
* Pepper & Carrot
* a poem
* a story
