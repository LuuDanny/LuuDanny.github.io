---
layout: essay
type: essay
title: "Ask Smart, and You Shall Receive"
# All dates must be YYYY-MM-DD format!
date: 2023-01-22
published: true
labels:
  - Smart Questions
  - StackOverflow
---

<img width="300px" class="rounded float-start pe-4" src="../img/smart-questions/rtfm.png">

I’m sure we've all encountered a problem at some point in our lives that we couldn't solve on our own. After struggling for hours and trying to find a solution through brute force, it's natural to turn to Google for help and hope that someone has already encountered a similar situation. However, what happens when none of the results are applicable to our situation or our situation is entirely unique and no one has asked the question yet? At this point, the best course of action is to simply ask for help, as our teachers often said, "there is no such thing as a stupid question." Unfortunately, they never told us that there were “stupid” ways and “smart” ways of asking questions. 

## What is the Smart Way?

Often, when asking questions on popular forums like StackOverflow, it isn’t uncommon to find yourself on the receiving end of some hostile comments. You may come to the conclusion that all “hackers” are simply rude and condescending; however, the more likely cause may simply be in the way in which your question was asked. It’s important to understand these public forums are largely volunteer work and thus in order to receive sincere feedback, you have to demonstrate that you actually put in effort to understand the problem and have a clear idea of what you want by asking “smart” questions.

In their essay, How To Ask Questions The Smart Way, Eric S. Raymond and Rick Moen outline several characteristics that make a question “smart” vs “stupid.” 

1. Use meaningful, specific subject headers.
   - When users are scrolling through the forums, the first thing that they will notice is your header. Everyone knows that you need help and so in most cases including lines like "Urgent" or "Help Me" will only be counterproductive as you end up attracting their ire and turn off any potential helpers. Having a meaningful header will allow users to quickly have a general understanding of your situation and make the determination of whether or not their expertise would be helpful.  
2. Don't post screen-shots, copy and paste instead.
  - If you are experiencing issues with your code, rather than posting a screen-shot, it is much better to copy and paste the code as most people do not want to waste their time hand-writing your code. By purposely making your code difficult to access, you are like to receive responses the provide general solutions or ones that scorn you for not properly posting your code. 
3. Accurately detail your problem in a clear and consise manner.
  - When describing your problem, it is important that you provide detailed information about what the issue is, what environment you are using, what research have you already done, and what diagontics steps have you taken. Doing so demonstrates that you actually did you homework and will allows user's to replicate your error and provide a helpful solution. Of course, being accurate does not mean writing a 5 page essay about the issue as no one has the time or is willing to put in the effort to read your question.
4. Be respectful.
  - At the end of the day, you are not entitled to receive any help and any help that you do receive is voluntary. If you cannot properly demonstrate respect, how can you ever others to reciprocate the same. 

## What a Smart Question looks like

```
Q: python date of the previous month

I am trying to get the date of the previous month with python. Here is what i've tried:

str( time.strftime('%Y') ) + str( int(time.strftime('%m'))-1 )

However, this way is bad for 2 reasons: First it returns 20122 for the February of 2012 (instead of 201202) 
and secondly it will return 0 instead of 12 on January.

I have solved this trouble in bash with:

echo $(date -d"3 month ago" "+%G%m%d")

I think that if bash has a built-in way for this purpose, then python, much more equipped, should provide something 
better than forcing writing one's own script to achieve this goal. Of course i could do something like:

if int(time.strftime('%m')) == 1:
    return '12'
else:
    if int(time.strftime('%m')) < 10:
        return '0'+str(time.strftime('%m')-1)
    else:
        return str(time.strftime('%m') -1)
        
I have not tested this code and i don't want to use it anyway (unless I can't find any other way:/)

Thanks for your help!
```

While the heading of his question could be better, it does convey what he’s trying to figure out. Usually something as brief as “python date of previous month” is what other users would enter in as search terms on Google, making it easily found. Another good thing about the question is that it’s not just a question. The asker shows what he or she has done and that he or she has put in some effort to answer the question. And while it may not be as important as the question itself, the asker shows courtesy, which does increase the chance of getting an answer.
