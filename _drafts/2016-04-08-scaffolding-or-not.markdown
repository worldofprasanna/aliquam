---
layout: post
title:  "Scaffolding (or) From scratch"
date:   2015-10-30 22:21:54 +0530
categories: programming practices
---

---
I always felt uncomfortable in having generated code in the repository, it all started from the stub & proxy generation for soap service in Java world. Ugly, pure ugliness. I felt its similar to `Waste paper theory`. That first waste paper in a place, will attract more and over period of time it ll be garbage. Once we have some piece of code which we don t understand how it works, but somehow it works will attract more such pieces and it ll be very difficult at maintenance phase.

Also I feel `In Development` phase is the most relaxed phase when compared to others, because there is no external dependency. Once the story is moved to QA or worst case rolled out to production, then every second ticks. Someone will sit on your head or atleast will be asking about the status and the only option we would have is to complete / fix the bug ASAP. Lets assume that at development we somehow completed / generated the code, moved the story to QA and if suppose a bug comes then the situation won t be similar to In dev phase coz,

* We are blocking some other person s work
* Our work is also blocked and we have to switch context between current story and this new bug
* There would be some internal pressure, coz we did that story and we can t convience ourself to learn and do it now
* Apart from moving the story to QA we didn t grow, get matured there.

Also each and every piece of the code we write should have our style. I feel that with generated code, we would miss that.

Am not saying that we should not use any library and write everything on our own, but the code which resides in our repository should have our seal to be there.

But there would be lot of features which we are not aware of, which could reside there in scaffolded code. I feel we should generate scaffolding and checkout the features and handpick the ones we want. By this way we will know what comes into our repo and we could consciously avoid the ones which we don t need.
---
