---
layout: post
title:  "Devops days India"
date:   2017-09-16 02:21:54 +0530
tags: devopsdays conference
---

I was here in Bangalore to attend the Devopsdays India 2017 something which I was eargely waiting for few months to attend. Things which attracted me are Kubernetes, Nathan Harvey, workshop, lots of Docker related sessions.

![With Nathan Harvey !!! :-)]({{ site.url }}/resources/images/with_nathan_harvey.jpeg)
---
**Keynote by Nathan Harvey**

Nathan Harvey s keynote was awesome. But I think he mostly touched upon the basic Devops stuffs starting from having the code in version control system (not using the .bak method), unit tests, ci, cd and lots of gnans around learning, continous improvement, and some tools which chef developed in recent days,

These were those tools,

* [Habitat](https://www.habitat.sh/) - I asked this question of How Chef will be in the market when Docker is trying to take up the whole Configuration Management space? He said you can use something like Habitat which makes creating the container as a code though I couldn t figure it out what it is. Only thing which I got is, It makes the process of container creation simple and it can co exist with Docker

* [Inspec](https://www.chef.io/inspec/) - Having the compliance itself as code

Apart from mentioning about these products, this is the summary of gnans which he gave (I only remember things which I feel are relevant to me)

* Communities are the key thing to learn and grow. There is a slack team for Washington DC with different channels for different technologies.
* Be the practioner. Try to take lots of code to production ASAP.
* Meet more people and get to know their problems, how they solutioned it, how you will solution it. Have lunch with different people daily.
* Make your work visible to the outside world.
* Measure your progress through some means and always ensure there is Continous Improvement in the things you do.

---
**ML expert s view of Devops**

The session about problems faced by Machine Learning scientist when doing devops work was somewhat useful. He mentioned about the problems he faced in serverless architecture, monitoring & logging problems with distributed computing.

* Using serverless architecture coz they thought they don t need to maintain the servers. It caused problems in monitoring, logging. That too they had distributed servers to process large amount of data.
* How he used nohup to avoid 5 mins execution time of lambda - thought of looking at this.
* Using AWS Config to have compliance for the servers
* AWS X-Ray to aggregate logs from different servers

Somehow I had the feeling that he had done lots of stuff with AWS, eventhough he is a just a ML expert. That easy AWS would be.

---
**Lightning talks**
There were many lightning talks, but 2 of them got my attention,

1. (kedge)[https://github.com/kedgeproject/kedge] - Declarative kubernetes application.
2. (kompose)[http://kompose.io/] - convert docker compose files to kubernetes resources.

---
**Kubernetes workshop**
Kubernetes workshop was the eagerly waited one, but I find it disappointing coz it just ended like following the tutorials in [Kubernetes by Example](http://kubernetesbyexample.com).

---
Apart from this I couldn t find any other session to be useful / worth mentioning it here. I got to meet few folks from GoJek and checked with them about their devops practices and how they are handling this much scale.

Somehow I got the feeling that if I focussed my learnings and if I come out of my comfort zone, I can also take sessions in conference.
