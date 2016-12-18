# TCAINGWAQ
by uakci

## Table of Contents
1. Introduction
- 1. Design goals
- 2. Why not taking on Lojban's solution?
- 3. Licensing and forking
2. Phonology
- 1. The sounds
- 2. Syllable shape
3. Morphology
4. Basics
- 1. "Verbs" and English
- 2. Your first sentence
- 3. Me and you
- 4. More connections
- 5. The ABCs
- 6. Relation triangles
- 7. Unary connections
- 8. Numbers
5. Words' words
- 1. My name and my words
- 2. Someone's words
6. The abstract world
- 1. Events
- 2. Traits
- 3. Facts
- 4. Other uses of the patterns
- 5. Coersion
7. New things
- 1. Makeshift words
- 2. New concepts
. Lexicon
. Sample texts
--

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
Forking is the thing that keeps the language alive. Once this document lands on GitHub, you can freely fork it. (Pull Requests of good features always welcome)

## 2. Phonology

### 2.1. The sounds
There are five wovels:
/a/ <a>, /i/ <i>, /u/ <u>, /e/ <e>, /o/ <o>
(pronounced "ah", "ee", "oo", "eh", "oh"; without the extra bits English tends to add)

Two so-called semivowels:
/w/ <w>, /j/ <y>
(pronounced as "w" and "y" as in "wine" and "yet")

Sixteen consonants:
/p/ <p>, /b/ <b>, /t/ <t>, /d/ <d>, /k/ <k>, /g/ <g>
/r/ <r>
/n/ <n>, /m/ <m>, /ŋ/ <q>
/s/ <s>, /z/ <z>, /ʃ/ <c>, /ʒ/ <j>, /h/ <h>
/l/ <l>
(<q> is pronounced like "ng"; <c> - "sh"; <j> - "zh")

All the sounds can be pronounced differently, as long as they can be clearly distinguished.

### 2.2. Syllable shape
The syllables always have these parts (in order)
* all consonants expect l/n/q or a pair of consonants AND/OR an optional j/w 
* a vowel or a diphtong (pair of vowels)
* an optional l/n/q
For example: ga, bra, wo, gaun, dryauq

## 3. Morphology

There are two word shapes: verb, particle. A particle is a small word carrying not meaning, but grammatical significance.
The particle shape: one syllable without an <n/l/q> at the end
- e.g. ge, ba, brau, bryoi
The verb shape: syllable(s) with <n/l> at the end + a syllable with <q> or nothing at the end OR a syllable with a <q> at the end
- e.g. ganbei, brulfa, guljeldjenmelfelpye; daq, fryauq

## 4. Basics

### 4.1. "Verbs" and English
A Tcaingwaq verb differs greatly from an English verb. It can stand for what in English is an adjective or a noun, and works like a sentence with slots to be filled in.
Let's look at an example of a verb:
    taq - A talks to B about C
We have three slots: A, B and C. All of these slots represent objects (the talker, the one talked to and the topic) essential for the concept of talking.
Let's have a go at another verb:
    palkei - A is a potato from plant B
As we can see, this verb is more 'nouny', yet it functions as a verb.

### 4.2. Your first sentence
Now, enough talk about verbs, let's get to know how to use them.
To say that there is a thing that matches the A's of both verbs, we put them one after another. So:
(1) taq palkei
    talk.A potato.A
    "there is a thing that talks and is a potato"; "talking potato"; "a potato talks"
Now, you may wonder, is there some meaning to the word order? Does (1) signify that a talker is a potato, but not the other way? Well,
(2) palkei taq
    potato.A talk.A
    "there is a thing that is a potato and talks"; "talking potato"; "a potato talks"
no.

### 4.3. Me and you
Let's move on to some more complex sentences. What about us? Me and you, we all express our actions using words like "me" and "you". In Tcaingwaq, those are verbs too! You thought it couldn't get crazier, right? Let's introduce "wai" and "fe":
    wai - A is me, the speaker
    fe - A is you, the listener
So, you can guess how to say "I talk" or "you're a potato":
(3) wai taq
    me.A talk.A
    "I talk"
(4) fe palkei
    you.A potato.A
    "You're a potato"

### 4.4. More connections
Now, the problem with the sentences so far is that "X is Y" is the limit of what we can accomplish. Suppose we want to say, "I talk to you". In order to do that, we need to access the B of taq. But how? Let's try this:
(5)*wai taq fe
    me.A talk.A you.A
    "I talk. You (...)"
The problem here is that the verbs always group in two, so that one can conveniently express sentences one after another. Here, "wai taq" groups into one sentence, and "fe" starts another. Yet, the other part of the second sentence isn't there, so the sentence awaits completion (or is ungrammatical).
We need a way to express that B, the one to whom I talk. We need a verb for that:
    wo - repeat the preceding verb (or another "wo" if present), using the first open slot
This lets us break down a sentence into two: "I talk. You are the person talked to". The difference between this rough translation and what we're trying to say is that the two "talk"s are refering to the same relation. Let's proceed to the sentence:
(6) wai taq wo fe
    me.A talk.A *talk.B you.A
    "I talk; and the talker of that is you"; "I talk to you"
If there's more than just one thing to glue, you can repeat "wo". For example:
(7) wai taq wo fe wo palkei
    me.A talk.A *talk.B you.A *talk.C potato.A
    "I talk to you about a potato"

### 4.5. The ABCs
So, you know how to "glue". But how can you refer to the Bs and Cs individually? That's the job of a series of these particles:
    yu - use the B slot of a verb
    ju - use the C slot of a verb
These particles follow the verbs to choose the desired slot. Let's talk about potato plants:
(8) taq-ju palkei-yu
    talk-C potato-B
    "A topic of conversation is a potato"; "I'm talking about potatoes"
You may have this question now: how did that "I" slip into the translation? Vagueness. The sentence is vague, that is, the talker isn't specified. It could be me, that rock or the same potato. When a slot isn't specified, it's ignored.

### 4.6. Relation triangles
It sometimes is that we want to express a relation of three verbs. For example, while "weird potato" ("heq palkei") is a relation of two verbs, "weird talking potato" is of three. Yet, we need a way to have such a relation. In order to stick a third verb to form a triangle, use the word "roi":
    roi (ROI) - add a third (fourth...) verb to a connection
Now, "weird talking potato" would be:
(9) heq taq roi palkei
    "weird talking potato"

### 4.7. Unary connections
While we can now handle cases with two, three, four, and even more connections, we haven't yet discussed the case in which there's just one connection to be made. This is not correct:
(10)*palkei
     "potato (...?)"
In order to make a sentence "Something is a potato", we have to coerce it into a binary connection with "co".
    co (WO) - vague verb
"co" doesn't mean anything. It can stand for any verb and any relation. Now we can say:
(11) co palkei
     "something is a potato"
or:
(12) palkei co
     "a potato is something" = "something is a potato"

### 4.8. Numbers
[TODO]

## 5. Words' words

### 5.1. My name and my words
First, let's learn how to use names. How does one say "name"? In Tcaingwaq, it is:
    naiq - A is the name of B given by C
But how to quote a name to use it with naiq's A? 
There's a series of words to quote and use names:
            Name Thing named
1 syllable  mya  da
2 syllables mye  de
3 syllables myi  di
4 syllables myo  do
5 syllables myu  du
All particles from the "Name" and "Thing named" column create a verb "A is the name [name]" or "A is the one called [name]", respectively.
For example:
(1) de-Tcaingwaq
    the.one.named-"Tcaingwaq"
    Tcaingwaq; to be Tcaingwaq
Please note that there already is a word for Tcaingwaq, "tcaingwaq". (duh)
(2) mye-Suzen
    the.name-"Suzen"
    the name "Susan"
Now we can actually use "naiq" like this:
(3) naiq myo-Halesanda
    "The name is "Alexander""; "Name's Alexander"
But there are other (shorter) ways:
(4) wai di-Maruku
    "I'm Mark"
Now, what's the restriction? Well, to keep everything clean, the quoted text must be coerced into a sequence of Tcaingwaq syllables. Thus, "Alexander" has become "Halesanda", "Susan" - "Suzen" and so on.

### 5.2. Someone's words
[(quoting) TODO]

## 6. The abstract world

### 6.1. Events
It sometimes is that we want to refer to some particular event. In order to do that, it's not sufficient to put two verbs next to each other. We need a particle! This time, it is "so" of the new class SO:
    so (SO) - turns connection into verb: A is the event of [the connection]
Let's have a look at some examples:
(1) wai diaq wo so fe beq
    me.A see.A | *see.B the.event.of(you.A eat.A).A
    "I see an event of you eating"; "I see that you eat"
(2) so fe palkei heq
    the.event.of(you.A potato.A).A weird.A
    "There's a weird thing that is the event of you being a potato"; "That you're a potato is weird"
There's also a YU version of "so" for convenience, "zo":
(3) diaq kioq-zo
    see.A die-event.A
    "I see death"

### 6.2. Traits
Traits are like events, but differ in usage. They have an assumed slot for a verb to be passed in. Just like in real life, traits are possessed by things, and so a Tcaingwaq trait is possessed by all the things the verbs of which fit into the slot. Because of the nature of traits, a different syntax is used. Thus, let's introduce the class YU's member, "su":
    su (YU) - turns verb into verb: A is the trait of [verb]-ing ([verb]'s non-A places follow)
For example, if verb "taq" is "A talks to B about C", then "taq-su" is "A is the trait of talking to B about C".
Let's piece up a simple example:
(4) hyoiq-yu taq-su wo fe
    want-B talking-trait.A *talking.trait.B you.A

### 6.3. Relations
[Relations are relations (duh) of two or more objects. To express them, use the word "lai":
    lai (SO) - turns connection into verb: A is a relation of [the connection]; binds "mau" in the enclosed connection
    mau (WO) - stands for one of the related objects FIX]

### 6.3. Facts
There are things that may not be the truth, but we want to express anyway. (...)

[... will elaborate on abstractions; for now, let's forget about them and work on loanwords]

## 7. New things

### 7.1. Makeshift words
Sometimes language doesn't provide us with all the concepts we need for communication; even if it did, we'd never know them. While there may be some loanworded concepts in the dictionary already, it sometimes is required to create a word on the fly. 
Tcaingwaq provides us with a quite limited syllable structure, so words need to be reduced in the coda (the part of the syllable after the vowel) - we must put -n or -l in the middle of the word, and -q or nothing at the end. There are two patterns one can use to make a good loanword:
- ignore the codas entirely, and use whichever of -n/-l fits better; or
- intertwine the codas with vowels.
[EXAMPLES]

### 7.2. New concepts
[TODO]


## . Lexicon

### Particles:
* co (WO) - vague verb
* da (DA1) - change one-syllable name into verb: A is called [the name]
* de (DA2) - change two-syllable name into verb: A is called [the name]
* di (DA3) - change three-syllable name into verb: A is called [the name]
* do (DA4) - change four-syllable name into verb: A is called [the name]
* du (DA5) - change five-syllable name into verb: A is called [the name]
* fe (WO) - A is you, the listener
* gyu (YU) - use the D slot of a verb; this word doubled/tripled/... refers to the E/F/... place
* mya (DA1) - change one-syllable name into verb: A is the name [the name]
* mye (DA2) - change two-syllable name into verb: A is the name [the name]
* myi (DA3) - change three-syllable name into verb: A is the name [the name]
* myo (DA4) - change four-syllable name into verb: A is the name [the name]
* myu (DA5) - change five-syllable name into verb: A is the name [the name]
* ju (YU) - use the C slot of a verb
* roi (ROI) - add a third (fourth...) verb to a connection
* so (SO) - turns connection into verb: A is the event of [the connection]
* su (SU) - turns verb into verb: A is the trait of [verb]-ing ([verb]'s non-A places follow)
* wai (WO) - A is me, the speaker
* wo (WO) - repeat the preceding verb (or another "wo" if present), using the first open slot
* yu (YU) - use the B slot of a verb
* zo (YU) - turns verb into verb: A is the trait of [verb]-ing of (... [verb]'s places follow)

### Classes:
* DA - (class of classes) quote some number of syllables
* ROI - connects a connection to the following verb
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