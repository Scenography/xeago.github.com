---
layout: simple
title: Time management
---

Taking the [development process] into account, I find it unsuitable to plan precisely. New discoveries can have a big impact on cycle-to-cycle activities. A detail planning should, therefore, be made from development cycle to development cycle. Constructing a detail planning should take no longer then 1 hour.

# Time estimates
Below is a table of activities and their estimated times. It is expected that this list will grow and will not be complete at any given point in time.

Activity                                    | Hours | Notes |
|-------------------------------------------|-------|-------|
Introduction elasticsearch and tire.rb      |   20
Working in ruby (inexperience)              |   30
Service architecture of VideofyMe           |   30
Basic search                                |   20
Getting used to projects (code-structure)   |   10
Tag search                                  |   10
Improving Tag search                        |   15
Design search                               |   10  |   recurring
Design architecture                         |   30  |   recurring
Performance plan                            |   40
Team building                               |   15
Documentation for school                    |       |   a lot of hours
Extended abstract                           |       |   a lot of hours
Failover/Discovery in [Tire]\(-[contrib])   |   140 |
Ruby, (monkey-)patching                     |   10  |
Learning ES query language                  |   100 |
Implementing search for videos              |   30  | recurring


# Preliminary work
<small>See the [first status report].</small>  
In the first few weeks I worked on several things supporting the deprecation of the old search and moving towards the new system. I was pleasantly surprised how easy it was to get elasticsearch active and populated. Once that was up and running I added support for pagination through the API. I now felt that I had a clear idea of what I will be doing and defined my concrete [internship assignment]. I send this for approval and got positive feedback.  
I experimented with different [lucene analyzers] to provide a short term solution for searching with spaces, keyword filter doesn't tokenize. Following this there was a deadline from the App-team, requiring search on hashtags. I implemented hashtag-search, and worked on my [performance plan]. Borrowing some of the functionality I created earlier, hashtag-search was easy to implement, though it had its quirks. I continued with the performance plan.  
Hell, this plan was a lot of more work than I expected. I am still awaiting feedback from Rianne, but have gotten approval from Patrick. I also set up a proposal for my [development process].  
*I have not recorded timerecords during this period. I was still setting up tooling to do so and felt getting my internship assignment and related documents clear was more important.*

# 24 September - 6 October
During this week I will be working on improving hashtag-search and unifying the current code base. I also reserve some time to validate documents made last week with my supervisors.

# 7 October - 21 October
In this timeframe I will refactor the old code to provide a more solid, re-useable implementation. As my [internship assignment] does not state an end-clause I will write a document about this. If time allows I will investigate more on how to patch existing Ruby code and possibly attempt to implement a minor feature in [tire-contrib].

# 29 October -  11 November
Implementing the design is nearly complete. I will add a component to do hashtag search within the design. I haven't managed to get to write about the end-clause about my internship — I will have to do this before the mid of my graduation.

[first status report]: status-reports.html
[development process]: development-process.html
[internship assignment]: graduation-assignment.html
[lucene analyzers]: http://lucene.apache.org/core/old_versioned_docs/versions/3_0_1/api/all/org/apache/lucene/analysis/Analyzer.html
[performance plan]: performance-plan.html
[tire]: https://github.com/karmi/tire
[tire-contrib]: https://github.com/karmi/tire-contrib
[contrib]: https://github.com/karmi/tire-contrib
