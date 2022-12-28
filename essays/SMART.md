---
layout: essay
type: doNotShow
title: SMART goals and SMART questions
# All dates must be YYYY-MM-DD format!
date: 2021-01-27
labels:
  - questions
  - answers
  - goals
---

After reading Eric Steven Raymond and Rick Moen's essay [*How to Ask Questions the 
Way*](http://catb.org/~esr/faqs/smart-questions.html), I realized how similar the guidelines were to SMART goals. The essay is a long write up of how to formulate good questions to ask hackers and developers on online forums, chat rooms, or through email. SMART goals are a general guideline for how to make effective goals, SMART is an acronym that describes good goals: specific, measureable, achievable, relevant, and timely. I thought the advice given in the essay was very similar and mirrored the ideas in the SMART goals acronym. 

## More Specifically...

The SMART goals acronym in the most general sense is trying to stop you from making goals that are too big and open ended to act upon. Instead it guides you into making smaller (and probably multiple) goals which are more actionable. The essay on how to ask questions follows a similar idea. It tries to steer you away from asking questions that are too open ended and general, and really get to the heart of what you are asking. Rather than asking "How do I implement [insert complicated feature here]?" you should start working on that feature and ask a more specific and smaller question that comes up along the way, like "X issue is coming up when I do Y on Z, what am I doing wrong?". 

## Example of a "bad" question

[This question](https://stackoverflow.com/questions/65930525/error-converting-result-java-lang-nullpointerexception-and-json-parser-error-pa) at first appears to be quite similar to my example of a good, small, specific question, its first line reads:

```
I keep getting the following error in my logcat whenever
i try to click on "login" or "signup" on my virtual device
<long error message ommitted for length>
```

This is all reasonable, but it takes more than one line to make a good question (unless the question is rather simple). After this introduction the author should take time to talk about what he has tried, and what he was able to gather from his error message and research. But after reading past the first line (or reading the title), many red flags from the essay come up. First of all, the title is so long that it gets cut off by stack overflow, the title is just the long error message that is already pasted into the body. No one is going to read that title and think "I want to help this person". The author then committs the biggest cardinal sin of asking for help online: showing that they did no research on the topic themself, and instead simply dumping their source code for someone else to painstakingly comb through. The post does not even ask a direct question; it simply states the error is happening and dumps the code on you. That's bad enough, but they don't just dump one long function on the reader, they take it one step further by pasting the body of *three* different files. Just to recap, the entire body of this author's question is:

```
I keep getting the following error in my logcat whenever
i try to click on "login" or "signup" on my virtual device
<long error message>
Please help!
<entire body of 3 files>

```

Unsurprisingly, the author has not yet gotten a response. 

## Example of a SMART question

[This](https://stackoverflow.com/questions/2003505/how-do-i-delete-a-git-branch-locally-and-remotely) is a great example of a succinct, helpful question. It gets straight to the point right from the title and the author has the courtesy of showing what they tried themselves before asking:

```
(title) How do I delete a Git branch locally and remotely?
<failed command line attempts>
What should I do differently?
```

There is really not much to say here, it's a very effective question. It also helped many other people due to its very clear title being easy to search for. It sits as one of the highest upvoted posts on stack overflow, and has been viewed over 8 million times.

## Conclusion

It is very important to value the time of and respect other people online (and in general!) - especially those who are volunteering to help you. Acting entitled to being handed a solution is a great way of being ignored or insulted even. Websites like stack overflow are fantastic for allowing us to quickly find solutions to issues and resolve them without having to do hours of testing or combing through a manual. But it can also be used lazily as a personal tutor. It's critical to remember to ask smart questions, as they can often resolve the issue before you even finish typing them.
