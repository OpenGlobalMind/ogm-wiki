# TheBrain 15 with Harlan Hugh

*A conversation between Jerry Michalski and Harlan Hugh, recorded on Zoom October 30, 2026*

## Chapters

```
0:00 How we met: TheBrain's first press briefing (1997)
2:41 From TheBrain 14's AI to Cerebro in TheBrain 15
7:25 Onboarding, and why connections beat containers
9:55 Persistence: a memory outside your head
13:18 Second brains: notes-first vs. context-first
15:32 A thought from 1997: buddy lists and PDAs
18:20 HyperCard could have been the web
19:37 Ship of Theseus: three rewrites of TheBrain
22:12 The new business model: TheBrain is free
24:44 Sync as sharing, and the new web version
26:50 Power users, scripting and the new API
29:55 First look at Atlas
37:26 How to get the most out of Cerebro
42:00 Atlas on 650,000 thoughts
46:49 Substack Pubs and Cleo Abram
50:14 Atlas timeline and 3D views
55:26 Knowledge should accumulate: our amnesic society
57:21 Prezi, and looking for a storytelling tool
59:52 Snip!, and building story paths in Atlas
1:03:35 Where TheBrain fits: infrastructure for people and AIs
1:06:13 Maps as boundary objects between humans and AIs
1:10:59 Saving AI conversations into your Brain
1:12:28 Jerry's Brain after Jerry, and thanks
```

## Linked Items

- [2026-10-30 TB15 with Harlan Hugh](https://bra.in/5vBBBa) (the hub thought for this call in Jerry's Brain)
- [Harlan Hugh](https://www.linkedin.com/in/harlanhugh/)
- [TheBrain 15](https://thebrain.com/products/thebrain/thebrain15)
- [TheBrain 15.0.637.0 (2026, tons of features)](https://bra.in/3j4PPG)
- [Cerebro (2026 GenAI in TheBrain)](https://bra.in/6jMbbe)
- [Building a Second Brain (BASB)](http://www.buildingasecondbrain.com/)
- [Gassée Almost Killed HyperCard. Said No Developers Would Develop because Users Would Write Their Own.](https://bra.in/8vPmmJ)
- [HyperCard Could Have Been the Web](https://bra.in/4pdzVj)
- [Atkinson Had to Threaten Apple to Get Them to Bundle HyperCard with the Mac](https://bra.in/3jrwJ5)
- [Ship of Theseus](http://en.wikipedia.org/wiki/Ship_of_Theseus)
- [Major TheBrain Software Migrations (rewrites)](https://bra.in/4jrzz5)
- [TheBrain's Platform Evolution](https://bra.in/7qnPP9)
- [GitHub Flavored Markdown (GFM)](https://bra.in/9jrzz5)
- [Atlas View (2026 in TB15)](https://bra.in/2pdLLV)
- [Errolson Hugh](https://bra.in/5vmmmZ)
- [Yikes More Weblogs](https://bra.in/4jgDa2)
- [Substack Pubs](https://bra.in/8qV7mJ)
- [Cleo Abram (channel)](https://www.youtube.com/c/CleoAbram)
- [Contrarians Who Make (or Made) Sense](https://bra.in/4jrdQp)
- [Knowledge Should Accumulate](https://wiki.openglobalmind.com/projects/jerry's_nuggets/knowledge_should_accumulate)
- [Many Links (Attached to Thoughts) in My Brain Are Broken. Please Use the Wayback Machine to Retrieve Them.](https://bra.in/3p75kM) (opinion)
- [We Are an Amnesic Society](https://youtube.com/shorts/buzLBikvhNM?feature=share)
- [Ways We Snipped Long Term Relationships in Finance, Paving the Way for the GFC](https://bra.in/7j3PNr)
- [Snip! Examining the Subprime Crisis (and Cascading Failure)](https://youtu.be/Z3bog8-vbG0)
- [Planning with Agents: Divided Worlds, Boundary Objects, and Thicker Interfaces](https://maggieappleton.com/planning-agents) by Maggie Appleton
- [Conceptual Maps as Boundary Objects for Humans and AIs](https://bra.in/2jMbbe) (opinion)
- [What If TheBrain Were the OS for Linux Laptops?](https://bra.in/2pKKbr)
- [JB>J (2026 JBafterJ or Jerry's Brain after Jerry)](https://bra.in/6j4PPG)

## Transcript

**Jerry Michalski:** I am sitting here with [Harlan Hugh](https://www.linkedin.com/in/harlanhugh/), CEO of [TheBrain.com](https://TheBrain.com). I guess it's just TheBrain LLC, or what's the official name?

**Harlan Hugh:** The Brain Technologies is how we go by, but the legal entity is The Brain Technologies LP.

**Jerry Michalski:** LP, excellent. We first met almost 30 years ago, when we were both a little bit younger, and I think I was the first stop on your launch press tour.

**Harlan Hugh:** That is correct, yep.

**Jerry Michalski:** Which was one of those good universal coincidences, or moments of serendipity, at least insofar as my life is concerned. Your CEO at the time was at the head of our little board table, thumbing a paper deck, about to go into the deck, and I remember him saying, "I have this feeling we should just go straight to the demo." And then you opened your laptop. I think you were sitting to my left. You started showing your software, and my wet brain was like *this*. You just started downloading it into me.

And the weird thing is, I was halfway done writing an issue of Release 1.0, the newsletter I was writing at the time, about bookmark or link management and mind mapping, concept mapping, whatever you want to call it. I had this vague idea that the cool new thing on the web was links, because we had multimedia before on CD-ROM and that whole thing. Links were really important, and nobody had a place to keep their links. Everything I had seen up to that moment was not satisfying me at all. I was halfway done writing this issue, I was frustrated, and then you show up.

**Harlan Hugh:** It is kind of amazing timing that you should be writing on that topic the day we arrive.

**Jerry Michalski:** It was. There was some kind of kismet, some cool thing going on in the universe that day.

**Harlan Hugh:** Yeah. I had been working on the Brain at that point for, I think, four years, three of them in Los Angeles as part of the company with Don Block, our CEO at the time, who helped finance the whole venture. For you to be the first person who was going to publicly talk about the company, and for me to just open up my laptop, and it was like you knew everything I was going to say, and you were like, "Oh hey, yeah, that's exactly what I want!" I was like, oh, this is amazing.

**Jerry Michalski:** Love that. And here we are almost 30 years later, and you're on [version 15](https://thebrain.com/products/thebrain/thebrain15). In version 14 you added some AI into the Brain for the first time, I think, and the ways you added it in 14 were interesting to me, but not that useful to me. You could create a note and tell it, "Add some text here about the thoughts that are nearby," which was useful. You could also start to populate the Brain a bit, but I need to check for redundancy, because I hate duplicate entries. That meant I couldn't really use it. The demo you were using at the time was Nikola Tesla, and you had the Brain create a bio of Tesla with his inventions and his lifetime and so on. And I'm like, I put Nikola Tesla in my Brain a couple of decades back, including most of his inventions. I probably didn't catch them all, but how do I…?

And then 15 is like [two or three revs all at once](https://bra.in/3j4PPG). 15 came out, I was using the early beta, and it was good. Then all of a sudden you drop [Cerebro](https://bra.in/6jMbbe) into the middle of it, and everything changes, because now AI is deeply integrated, and the harness you have on Cerebro really knows how to curate a brain. It took me having a conversation with Cerebro to negotiate with it: "Hey, I hate duplicates, so whenever we do something, check first before you…" et cetera. And then I felt like, wow, this is super powerful. Can you elaborate on what's happened?

**Harlan Hugh:** I guess the evolution of AI, at least from the consumer, your favorite word, from the end-user perspective, has gone from this thing you can talk to, to this thing that can generate images, now videos, and then it can do your banking and shop for you, and do more and more stuff. Each modality, each way of working, has opened a new frontier in terms of what you can achieve with it.

What we did in version 15 with Cerebro is enable the AI to think of the Brain as another way of working. Instead of generating a picture, it's generating your brain. Instead of analyzing a picture, it's analyzing your brain. It has all the tools it needs to operate the software just like you as a person, but at super speeds, and in combination with all the knowledge about the world baked into it, as well as being able to reach out and query the internet and search your Brain.

Normally when you're talking to an AI, you're talking to it about the history you have with it, plus the internet and its training data. When you talk to Cerebro, it has another layer on top of that: it can query and understand all the connections in your own digital brain, and use that to filter what it needs to do and what you want it to say. And not only can it speak to you, it can generate things for you, double-check your work, create new work based on all of your other work. All these things that were science fiction not too long ago.

**Jerry Michalski:** Yeah, yeah.

**Harlan Hugh:** And in addition to being able to leverage AI for one-off tasks, when you're like, "Oh, I want to go do this," we've also enabled some pretty sophisticated scripting, so you can say, "Here's the thing I want my AI to do for me on a regular basis." You add it into the Brain, and it becomes part of the software. You create features by describing what you want them to do. You create a button for it, choose your own icon, put it on the toolbar, assign a keyboard shortcut to it. People used to write in with feature requests like, "Hey, I want the Brain to attach a Wikipedia article for me," or "find this thing on Amazon for me." Now you just click the button and there you go.

**Jerry Michalski:** Exactly. Historically, I think your biggest challenge has always been uptake: how do we onboard people to understand the software and use it quickly? A weird thing happened the moment my wet brain first saw you demo it, which was that I didn't need training, coaching or a manual. I kind of knew what to do with this thing. It helped that at the time I was a tech industry trends analyst, so I needed to track who's invested in whom, who competes with whom, and so on. I went straight there and created a little tech taxonomy, mostly software, because I wasn't a box counter like some of the analyst houses. I cared about things like instant messaging. All of a sudden I could see that this little instant messaging company had these investors. A reporter would call me, and I would quietly look up the section of my Brain on whatever topic they were talking about. My unaided recall might be half a dozen items, but suddenly I could see everything in that realm. So it worked well. And Cerebro just blows the doors off onboarding or uptake. People still need to understand what it is and what the possibilities are, but now there's this intelligence in the product that can do that really elegantly.

**Harlan Hugh:** Yeah. One of the things some people asked about the Brain, even on that very tour where I met you, was: what's the difference between this and just asking Google to get me stuff? It's two extremes. Somebody who relies on Google to do everything is asking the world, "What do you know about X topic?" And it brings back all that information. It's extremely good at that, and that's useful in a lot of cases. But some people want to know what *they* know about it and what *they* think about it. And unfortunately our memories are not perfect. That was the concept of the Brain from the very beginning: how do you transfer the connections you make in your head into a medium where they can be fed back to you just when you need them? You can share them, and you can decide when you want to forget something, as opposed to it just filtering out over time.

**Jerry Michalski:** What you just said is something I want to come back to later in the conversation. I call this phenomenon persistence. I think humans need a persistent memory outside their heads. Some people have really good, reliable memories, but mostly our memories are fallible. I'll often ask an audience, "Who saw something interesting on the internet today?" And 90% of the hands go up. Then I'll ask, "Who has a place to put the link to that thing where they know they'll find it again next time?" And it's guffaws and groans, every time. Everybody's like, "Geez, I've got a big spreadsheet," or "I have a private Pinterest board, or my own personal Insta that I don't show anybody." They're using a whole bunch of hacky things that don't really work. And the Brain is perfect for that.

**Harlan Hugh:** Yeah. The problem with most of the solutions out there is that you can save stuff, and maybe even categorize or tag it, but you can't connect it. They're not designed around connections, they're designed around containers. Back in 1998, when I was giving that little press tour, we always talked about the metaphor of the desktop, files and folders, and how that biased people toward thinking of their computer as a way of putting things in boxes. When really, the way your mind works is associatively, by making connections. So instead of separating things, we're connecting things.

The ability to connect things means that instead of just having a list of all the instant messaging companies, you can have that list because they're all connected to instant messaging, but you can also have a list of the people connected to instant messaging, and all the VCs who have funded stuff in instant messaging, and the products being used in different capacities around it. All these different contexts get created automatically from the connections. Not that the connections are created automatically: you create the connections, and from that network arises all this other value. And despite it being the year 2026, that still kind of doesn't exist. You can design a database to do that yourself, but most people aren't going to, and it doesn't have a user interface, and you can't share it, et cetera. So that's the heart of the Brain: how do you make connections and store them in a way that you can easily update and access them again whenever you like? And we have a visual layer on top of that, which hopefully makes it enjoyable.

**Jerry Michalski:** There's a whole bunch of people working on second brains, basically external brains. People like [Tiago Forte](http://www.buildingasecondbrain.com/) and a few others make a living coaching people through "here's my workflow," with intellectual models and frameworks for both process and structure, and how to add metadata. They'll use Obsidian or Notion or whatever. Some of those can be highly productive, and metadata is super powerful. But there's something about what you just said about connections and visualization. I am no physicist, but I believe matter is just energy trapped in fields. And the problem is our whole world only cares about matter, about the objects. Whereas we actually live in relationship with one another. April and I were just at a conference where we heard a lovely woman talk about Ubuntu, which is "I am because we all are." It's about how relationship is fundamental to existence, to identity. And I think that's true of stuff, too. Stuff exists in relation.

Most of these tools that do a second brain of some sort show you one thing at a time. I love wikis. I love Wikipedia and all wikis, though I'm sorry that Wikipedia kind of ate the wiki space. I thought we would all be collaborating with one another in wiki spaces. But a wiki shows you one page at a time with a bunch of links in it, and you're not seeing what's behind any of the links, or any of the context. The interesting, cool thing about the Brain is that it's sort of context-first.

**Harlan Hugh:** Yeah. There are ways, of course, to link things, and modern note-taking software lets you link stuff, but the links aren't a first-class citizen in the system.

**Jerry Michalski:** Exactly.

**Harlan Hugh:** The system wasn't designed around the links, whereas in the Brain, that was the main focus.

**Jerry Michalski:** Since we're talking about it, I figured I'd share my screen. I mentioned that a reporter would call and I would look up buddy lists, and this is what would happen. Suddenly I had all the buddy lists I'd ever heard of, and I could see at a glance that ChaCha is a buddy list from Palm Software. Palm did the Palm Pilot, one of the personal digital assistants back in the day. This is a thought I put in in 1997. Okay, so this is one of the first thoughts I put into my Brain, because I think you let me use it a little before general availability.

**Harlan Hugh:** Yeah, we visited you sometime in December of '97.

**Jerry Michalski:** It was December of '97. So on the 19th I added Personal Digital Assistants. That's kind of cool.

**Harlan Hugh:** That is bananas.

**Jerry Michalski:** And here are all the PDAs I saw at the time. Then there's a little subcategory, Ultra Mobile PCs, with Microsoft's Origami project, and here's Microsoft. Just so people get an idea of the contextual nature of this thing, because we're not looking at the content of a page. I think I'm a little unusual among Brain users in that I don't use the notes field very much. I'm all in on the nodes and the context, not so much the content of the pages. Some people use the notes field very intensely, and then it's more like navigating across a wiki that lets you see the rest of the world around the pages.

**Harlan Hugh:** It's interesting that you bring up Obsidian and Notion and things like that. I guess they call them connected notes?

**Jerry Michalski:** Richly connected context mapping tools, Markdown editors. "Integrated thinking environments" is also a name.

**Harlan Hugh:** Okay. But all those things are notes-first, so to speak.

**Jerry Michalski:** Yes.

**Harlan Hugh:** And what you're doing… I don't know if you have the note icon enabled, but almost all your thoughts don't have any notes on them.

**Jerry Michalski:** Right. The note icon is enabled, but there aren't many.

**Harlan Hugh:** So your Brain is really all about the structure and the nodes themselves, as opposed to the content inside the notes.

**Jerry Michalski:** Here's a note icon, because this is the agenda for our call, so I have where we might go as a note. And it reminds me that I was going to ask you about the Ship of Theseus, so we should go there.

**Harlan Hugh:** But one more point on this: you couldn't do what you're doing here inside Obsidian or Notion. It would be extremely clumsy at best.

**Jerry Michalski:** I was a huge HyperCard fan back in the day. The Brain equivalent for me, for maybe a decade, a long time ago in the early Mac days, was HyperCard, and I was programming simple stuff in HyperTalk. If Apple had understood the power of HyperCard, and if [Gassée and others hadn't been afraid of it](https://bra.in/8vPmmJ), they [could have invented the web](https://bra.in/4pdzVj). HyperCard plus the domain name system and URLs could have been HTML and everything else.

**Harlan Hugh:** I remember when HyperCard was the thing, and I was so excited about it, and somehow it just dropped off the end.

**Jerry Michalski:** Well, [Bill Atkinson had to coerce Apple to ship it](https://bra.in/3jrwJ5) for free. He had to threaten them. There wasn't really open source software at the time, but he was going to just share it out on disks, I guess. And Apple always saw it as competitive, not integrative or syncretic with what they were doing. Weird. One of those really dumb business decisions back in the day, I think.

**Harlan Hugh:** Somebody didn't have the vision.

**Jerry Michalski:** Exactly. So you've [rebuilt the Brain's code base at least three times over](https://bra.in/4jrzz5). The [Ship of Theseus](http://en.wikipedia.org/wiki/Ship_of_Theseus) notion is that you can completely rebuild a ship over time by replacing different parts while it's still functioning as a ship on its way, which feels like what you've done. And this last rebuild has given you magic superpowers, I think, because it coincided with the arrival of LLMs and AI as a genuine power-tool partner. That combo has been really good for you.

**Harlan Hugh:** Yeah. Version 15 is the third rewrite of the software, I believe. The version I showed you in 1997 was C++-based, and we stuck with that code base up until version 4. Back in version 3, the software infrastructure space was much different. We had to write everything ourselves: the database, the visualization, the user interface, the editor, everything from scratch.

**Jerry Michalski:** Yeah.

**Harlan Hugh:** In version 4 we rewrote everything in Java, and it was like, oh, we have a database, this is amazing, we don't have to write one. It was crazy. Then in version 9 we went to C#. Those were all complete rewrites, of course, because we were switching languages. And version 15 is also C#, but we replaced the entire front-end layer. That process started, gosh, I don't remember exactly, probably about three years ago, and we didn't release version 15 publicly until about a year ago. So each time it's taken multiple years. And each time it's been harder, because we have to compete with ourselves. The previous version always has deep functionality. Twenty-something years' worth of development adds up after a while.

**Jerry Michalski:** It does. It's kind of crazy. And with 15 you've also changed the business model, the pricing scheme. Can you describe it?

**Harlan Hugh:** Yes, absolutely. Back in the day when we started, we sold software, and we even made CDs. These days things are a little different, and we decided to make a pretty big shift in version 15. We've stopped selling the software, so now the Brain is free. Anyone can use 100% of the functionality on their desktop. The main thing we used to sell is completely free. The way we see it, we want as many people to use the software as possible, and people who really use it a lot will probably find it convenient to use our services too. The services being the ability to sync your brain from one device to another, back everything up, collaborate with other people, and use AI. You can actually use AI on the free version too, you just can't use a lot.

**Jerry Michalski:** There's a small budget.

**Harlan Hugh:** Yes, yeah.

**Jerry Michalski:** And you can do a little bit of syncing, too, with a small budget for it, so you can try out the advanced features. But to really use them you have to pay, which is great, because it means you're going to still be alive. I like that.

**Harlan Hugh:** Yeah, you can use 100% of the features. The thing you can't do is sync a lot of stuff privately. Technically, I think everything you're doing, you could do for free. You can have a brain of any size, as long as it's public, and you can share all of it. But if you want more than, I think it's a thousand thoughts that are private, then you have to pay to use our sharing services.

**Jerry Michalski:** I've got 650,000, so I think I'm a little past that waypoint.

**Harlan Hugh:** Yeah, but most of your Brain is public.

**Jerry Michalski:** Yes, yes.

**Harlan Hugh:** So that would qualify as free.

**Jerry Michalski:** Oh, that's so crazy. Now, what I'm about to say came up some years ago. I think you've always seen sync across platforms as a personal, private thing. There's also TeamBrain, which was collaboration in a group, but sync, I think, you always saw as a way to get the Brain on your laptop connected to your iPad, connected to your phone, whatever. And I've always seen sync as how I share my Brain with other people. When I'm adding anything to my Brain, I only ever do it on the laptop, never on the iPad. I'll occasionally look at it on the iPad, but I'm really a laptop-first kind of guy with the Brain. That might be changing because of some of the novel features you're adding. But I love sending people a direct link to a particular thought in my Brain, and I think that works pretty well. And because you've rewritten the platform, it now looks more like my own experience when people go look at it on the web.

**Harlan Hugh:** Yeah, that's one of the main reasons we rewrote things for 15. There are lots of reasons, but one was to enable [almost the same functionality and the same user experience regardless of the platform](https://bra.in/7qnPP9). With version 15 it's on Windows, Mac, Linux, Android, iOS and web, and the web version is virtually indistinguishable from the desktop version. I kind of forget even when I'm using it. I'm like, oh, I'm on the web. What we've been able to accomplish with this new technology stack is miles and miles ahead of where we were in version 14. It's really a completely different piece of software.

**Jerry Michalski:** It's super cool. And I'm excited to hear what other people are doing with it. One of the things that struck me years ago: I had a call where four of us, way-advanced lead Brain users, got together, and we were each using the Brain in very different ways, ways that were weirdly almost mutually incomprehensible. One fellow was using every macro and every script and every power tool and every meta-whatever. At one point he said, "Oh yeah, I can do GTD." And I said, "Great, so create a new item in your Getting Things Done Brain vocabulary." And he ran a macro that did something I didn't really understand. I thought, wow, this is strange, and I felt a lot of empathy for you, because you're trying to listen to your user base.

**Harlan Hugh:** Right.

**Jerry Michalski:** And we're apparently pretty quirky and different from one another in many ways, and you're trying to create a common platform that'll serve everybody with power tools.

**Harlan Hugh:** Right.

**Jerry Michalski:** That must have been hard.

**Harlan Hugh:** As I said earlier, the Brain is fundamentally all about connections, a platform for building and storing them. When you're doing something that fundamental, naturally there are lots of different ways to apply it. Your experience is probably at the extremes, in that the way you use it is mostly unique to you. There are other people who use it similarly, of course, but most people take advantage of file attachments and notes and thought types and tags, all the layers and layers we've added on top of the base functionality.

In version 15, we already talked about how you can extend it with AI through Cerebro, but we also have an API now, and there's a local version of the API that runs on your machine. So you can do a lot of cool stuff in terms of automating things, having it create things, reaching out to other systems and integrating them, all that magic. Version 15 has really opened the doors to so many things at that scale. We've even pushed the limits on ways to import data, export data, and even a new way of visualizing data that I might be able to show you today.

**Jerry Michalski:** Oh really? I'm interested.

**Harlan Hugh:** Okay. Well, let me share my screen, if I can do that. Here we go.

**Jerry Michalski:** Yep, it's there.

**Harlan Hugh:** Okay. I've got a couple of brains open here. This is the brain about the Brain, which we built recently. It's got all the information about how to use the Brain. If I move this over here, these are the notes, Jerry, in case you've never seen them before.

**Jerry Michalski:** Yep.

**Harlan Hugh:** This is another thing that's new in 15: a full Markdown editor with support for [GFM, GitHub Flavored Markdown](https://bra.in/9jrzz5). It's really nice. If I were doing a pitch about the Brain, this is one of the things I'd focus on for version 15. But we'll ignore that for now.

This is a conventional brain with different topics, organized with parents and children and jumps and so forth. But sometimes you want to see a little more of your brain, not just what's in the immediate area of what you've selected. We've had multiple ways of doing this in the past. One is what we call the Expand All view, where I can select a thought and see two generations out. In addition to the active thought and its parents and children, I can see the parents of parents, the children of children, and so on. But that's still just a few generations. If we want to see everything, we have a brand-new view coming, which right now we're calling [Atlas](https://bra.in/2pdLLV). Atlas shows everything in your brain. So here's the home thought…

**Jerry Michalski:** It doesn't explode when you give it my Brain data?

**Harlan Hugh:** Well, we're going to get there.

**Jerry Michalski:** All right.

**Harlan Hugh:** This is 179 thoughts, which is a lot, but not that many in terms of scale for a brain. Most of our users are well into the thousands of thoughts, or tens of thousands, and there's a handful into the hundreds of thousands, like yourself. If I want to focus on a particular area, I can click, double-click and zoom in, click over here, zoom in here, and you get the feeling for this.

To take another step up, I'll go over to my own brain. I've been using it, like you, since the mid-to-late '90s. In the Atlas view, we're going to see about 20,000 thoughts. And you're going to see there are a lot of different ways you can click into this. This is my…

**Jerry Michalski:** That's your brother?

**Harlan Hugh:** Here's [my brother](https://bra.in/5vmmmZ). Let me go back here. This is brand new; we just set this up. There's my home thought, and the thoughts you can see lit up are the ones directly connected to it. If I click off of this, you can see what the algorithm has automatically built as the hubs, the main sections.

**Jerry Michalski:** Basically context clusters.

**Harlan Hugh:** Clusters, yes, exactly. My brother happens to be one of the things that's very connected, and Google, for whatever reason, has a lot of influence in my brain. If you click into any one of these, you'll see where it is and what it's connected to. Then you can do a bunch of different things. I can zoom out and see the information organized differently. Right now it's colored by the regions it picked up automatically, but I can also color it by age. Now the newer things are the lighter, bluer things, it's a red shift, and the older stuff is clustered over on this side. There are lots of different cool things you can do with this. And at any time I can click into something and say, "Just show me this topic and what's related to it." So now I've gone into Google.

**Jerry Michalski:** So this is the same view, but first degrees from a particular thought?

**Harlan Hugh:** This is two degrees out from the thought I've selected.

**Jerry Michalski:** Cool.

**Harlan Hugh:** I don't want to click around in here too much, because this is my private brain and I'm not used to sharing it. So now we'll make the jump and go over to your Brain.

**Jerry Michalski:** Oh, man.

**Harlan Hugh:** Oh boy, here we go. This is a brand-new interface, as I mentioned, so I'm not an expert at using it yet, and there's a bunch of things to tweak still. But this is 650,000 thoughts, and it's going to take a moment to get it all set.

**Jerry Michalski:** The whole thing.

**Harlan Hugh:** Yes, it's loading the entire thing. To analyze the clusters and so forth, it has to bring everything into memory. For most people this is going to be pretty close to instant. You saw my brain had 20,000 items.

**Jerry Michalski:** You were brave to do this on a live podcast.

**Harlan Hugh:** Yeah, I did test this before, and it went a little faster than this. I don't know why it's taking quite so long this time, but I guess that's the way demos go. This is just one of the many things we've been able to take on, thanks to the new code base and, of course, the advent of AI being the magic sauce.

**Jerry Michalski:** While it's sorting itself out, do you want to talk a little more about Cerebro and what it enables? I think I've only barely been able to explore a few aspects of it, because I'm so grooved into physical habits of how I curate that even offloading some of those habits is difficult. I have to retrain myself. How should someone look at Cerebro?

**Harlan Hugh:** Well, if you have a brain already, probably the most interesting thing is to ask it questions about your brain, or about yourself. I think the first demo we did with you was asking it what you'd worked on in the last month, or something like that. It has access not just to the network, but also to the metadata about the network, the history, what's been happening. So it can do things you technically could do, but that would take you a very long time.

The way I like to think about Cerebro is as a person who can operate your brain for you at super speed. Instead of thinking of it as, "Oh, it's going to write a paragraph for me, check my spelling, or reorganize this little section of text," it can analyze your *entire* brain, go find stuff for you, and suggest new connections. The more ambitious you can be with it, the more you'll be able to take advantage of it. The main way I see people missing out is by not being ambitious enough. We're using the AI to build entire brains, and not play brains, useful brains. The Brain help I showed you earlier was basically all built by AI, and it's become the main knowledge base for how to use the Brain. That would have taken us many months of work.

**Jerry Michalski:** It's amazing. And if you've already got a brain and you've been using it a while, Cerebro can also help you refactor and change how you're curating. It'll suggest, "Hey, this part would work a little better if you had a parent thought labeled this, and we could move this over here." And you can say, "Please do that for me," and it knows how.

**Harlan Hugh:** It does indeed. It knows how to use your brain, and it knows best practices for how things should be organized and connected. It understands parents and children and jumps, putting things into multiple categories, all that magic.

**Jerry Michalski:** We're getting closer. We're like 15% from done, I think.

**Harlan Hugh:** I would not have clicked on this if I'd known it was going to take this long. Literally right before the call I clicked on it, and it was like five seconds.

**Jerry Michalski:** Maybe that memory didn't get flushed and now it's struggling to figure out where to put it. I don't know.

**Harlan Hugh:** I don't know, but this is the way it happens. We're very close. I promise this is going to be worth it.

**Jerry Michalski:** No worries.

**Harlan Hugh:** One of the reasons I wanted to show you this is that one of the things we're trying to accomplish with Brain 15 is for people to be able to pull more value out of the brains they've already built, where they already have everything in there. Okay, here we go. Holy moly. So this is 648,000, 649,000 thoughts, colored by region. You can see it's very dense.

**Jerry Michalski:** Yeah.

**Harlan Hugh:** Some of the things it's pulled out are the most connected ones. And this has changed over time. I'd looked at your Brain a few years ago, and the connections were different. I'm just randomly clicking around in here, and you can see there are so many things and so many connections that it's a little overwhelming. But if I right-click on one of these things, it pulls out everything that thing is connected to, plus one more generation. In this case I've come into an actor, and I've right-clicked, and now I'll right-click again. And now we have this movie, the director, the actors and so forth. Each time I right-click, it's this thing plus one more generation out. I can also go to search and say, "I want to see Google." And now it's showing me Google: all the things you know about Google, and the ways you have it interconnected.

**Jerry Michalski:** The Google diaspora. These are all ex-employees.

**Harlan Hugh:** Yes.

**Jerry Michalski:** Zooglers.

**Harlan Hugh:** Zooglers, yes, ex-Googlers. I know one of the things you have in your Brain is alumni from various places, and here we have Google alumni. We can see everything that's connected here. I can zoom in, and as I zoom in I can see all these different people, and if I click on any one of them, we can follow that in. I haven't played around in here exactly, so I don't really know where to go, but if you're curious about anything…

**Jerry Michalski:** Jason Goldman, right there in the middle.

**Harlan Hugh:** Here we go.

**Jerry Michalski:** Go follow him.

**Harlan Hugh:** So here we have Jason Goldman.

**Jerry Michalski:** He was one of the early co-founders at Twitter, so he's under Twitter alumni.

**Harlan Hugh:** From here I can see two layers out, and we have 495 thoughts. But if I want to see more, I can click this button, and it does one more generation out. It's exponential growth, of course, so now we're all the way out at almost 7,000 thoughts. And each time you do it, it re-clusters things and builds new categories based on where you are.

**Jerry Michalski:** It's doing it very quickly. I love that.

**Harlan Hugh:** Yeah, normally it's very fast once you're into the system. And you can see these interesting patterns forming. If I go down here, what's this? This is Weblogs.

**Jerry Michalski:** [The big list of all the weblogs I've seen](https://bra.in/4jgDa2), yep.

**Harlan Hugh:** Yeah. This pattern you see here is the items that only have one connection in the current view. In this filter, these are leaves in this section of the network.

**Jerry Michalski:** Could you go up to search and look for Substack Pubs? Just "pubs." There you go. This is the modern equivalent of Yikes More Weblogs, because everybody's moved over to Substack. As I see interesting Substacks, I add them to [Substack Pubs](https://bra.in/8qV7mJ), so this turns into the big compendium. Not that I read all of these, by no means; there's a whole lot more here than I could possibly ever read. But it's the cutting floor. A couple of these I actually curate: every episode that comes out, I'll add under that particular Substack's name, and then I'll connect that episode to the books it references, or whatever. So for some people whose thinking I follow, I'm actually weaving their material into the Brain.

**Harlan Hugh:** Yeah. I did browse through your Brain, and I was shocked when I came across [Cleo Abram](https://www.youtube.com/c/CleoAbram). There were like a hundred thoughts underneath her. I was like, oh my god, how does he track all that?

**Jerry Michalski:** It's easy enough, and you gave me a really nice shortcut for adding things to the Brain, so the gesture for adding something is easier than it used to be, which is great. Cleo is a science popularizer, and she's really, really good at explaining what she's explaining. For me that's really important, because the dry concepts and the scientific papers interest some small subset of people, but the popularizers are the ones who actually communicate this to the rest of us. That's why I really like them.

**Harlan Hugh:** Here we go, Science Popularizers.

**Jerry Michalski:** Exactly.

**Harlan Hugh:** The interesting thing about this layout is that it gives you a different way of looking at your brain and seeing what it's really about.

**Jerry Michalski:** Search for "Contrarians who…" There. "Contrarians Who Make (or Made) Sense," the second one. That one. This is [my little pantheon of heroes](https://bra.in/4jrdQp).

**Harlan Hugh:** Oh, cool. So from here, hopefully you're seeing things that maybe you didn't know.

**Jerry Michalski:** Yeah. The clustering is very interesting, and it clearly means I have a lot there, that I've linked them up to a lot of stuff.

**Harlan Hugh:** Yeah. The things shown automatically, which right now we're calling clusters, are not things you've consciously gone out of your way to mark as most important. They're just clusters that come out of the data based on how connected they are, more or less. And they'll change based on where you're focused at the moment.

One of the other neat things you can do is this timeline at the bottom. Oops, sorry, I've got a Zoom control sitting right over the button I want to click. If I click this play button, you can see the content in this area of your Brain building over time.

**Jerry Michalski:** So you're just taking the creation date of each thought and playing them in order.

**Harlan Hugh:** Yes, yes. It's the playlist of this area.

**Jerry Michalski:** That's a really cool animation.

**Harlan Hugh:** And you can drag through it. There are other ways to visualize the same type of data. Right now there are three dimensions. I've often said that three dimensions don't work well in a two-dimensional UI, but in this case it does provide some extra information. Right now we're seeing the head-on view of the data, but if I click and drag, I can turn it in three dimensions, and the depth can be assigned to different properties.

**Jerry Michalski:** Could you do the age of the thought as the depth?

**Harlan Hugh:** Indeed.

**Jerry Michalski:** Look at it. Right there is a variable for age.

**Harlan Hugh:** So here we are looking at it straight on, and as I turn it left…

**Jerry Michalski:** Oh, that's very cool.

**Harlan Hugh:** You can see the older things are at the back and the newer things are at the front.

**Jerry Michalski:** You can see the origins of the universe right there in the back.

**Harlan Hugh:** Exactly. You can see your thought for My Beliefs is one you created a long time ago; it's at the back there. And I can click on it, and whatever I have selected serves as the rotation point.

**Jerry Michalski:** Yeah.

**Harlan Hugh:** So there are lots of cool little things we're working on, and this is very early on.

**Jerry Michalski:** This temporal thing is very eye-opening. I know you save the metadata for date created and date last modified, but I never really go in and use it, and I haven't been doing many brain tours lately. I just sort of forgot it was there. So I'd kind of given up on using the age metadata, and you just made it super handy.

**Harlan Hugh:** Yeah, this view is really able to leverage a lot of metadata you wouldn't have noticed before. Another way of doing it is with link count. Now the most-linked things are closest to us, and the things with fewer links are further away. Another way of pulling stuff out. Here we can see Doc Searls has the most connections.

**Jerry Michalski:** Oh, he's such a prolific writer. He and Cory Doctorow, for example.

**Harlan Hugh:** Did you see him here?

**Jerry Michalski:** Cory, you can look him up. I didn't see him pop up, but I have a lot of Cory's writings in my Brain. There you go.

**Harlan Hugh:** You can see how that pulls him out at the top there.

**Jerry Michalski:** And Cory should be under Prolific Writers. I don't see it popping out, but I'm sure it's there.

**Harlan Hugh:** If we switch back to the Plex, of course…

**Jerry Michalski:** Exactly. Then it should be right above. Bam.

**Harlan Hugh:** One of the things we'll keep evolving is different ways of pulling out the data and referencing it. This is just the first way. There's another thing I won't show today that I've been working on for quite a long time, which will give yet another, kind of opposite, approach to viewing and browsing your data. A lot of people will be very happy about it, I think.

**Jerry Michalski:** Can you go to "Knowledge should…"? It's either accrue or accumulate. Accumulate is fine. Good. I wanted to talk a little more about persistence. [Knowledge should accumulate](https://wiki.openglobalmind.com/projects/jerry's_nuggets/knowledge_should_accumulate). What's cool is that I can find stuff that eludes other people. One of the things I like is that if I put a link in 10 or 12 years ago and it didn't get a lot of inbound love, it falls out of Google search. You can go to Google and look for it and it won't show up there. Sometimes the website is down, and I thank God that Brewster Kahle and company are at the [Wayback Machine](https://bra.in/3p75kM) and the Internet Archive, because I can rescue the site that was there. Just because something is 15 years old doesn't mean it's not brilliant.

So one of the things I love is that in my Brain I've been collecting the best of stuff. My first threshold is, is this worth remembering? Is it worth putting into the big ball of spaghetti that is my context for how I see the world? I'm having such a good experience of persistence and the ability to find things. Search for "we are an amnesic civilization." Just "amnesic." There we go: [We Are an Amnesic Society](https://youtube.com/shorts/buzLBikvhNM?feature=share). Perfect. When I try to make this point to people, most of them are drowning in the information torrent, and they don't have a reliable memory, so they don't have a lot of empathy for "hey, it's really useful when you can remember things and hook them up with each other and then show them as a narrative, as a story." And I think that's a piece of what tools like the Brain are extremely good at.

We talked earlier about Microsoft Office and its structure. There was another storytelling tool called Prezi, which is still around, I think. I was a very avid early Prezi user. Originally they had a funny circular zebra menu, and it was one of those tools where you could zoom in and out and chain together a path through thoughts. They had two big makeovers. In the first, they made it look more like PowerPoint: all of a sudden they had a slideshow, slides as the stages and so forth. That was still perfectly functional. I was like, okay, the zebra menus were apparently freaking too many people out. Then the second makeover lost the endless whiteboard, and I stopped using it. They took a sharp left turn, and I fell off the back of the truck. Which was bad, because Prezi was my favorite storytelling tool. The Brain is okay for storytelling, but I can't hide things. Right now there are so many things on screen, a ton of stuff.

**Harlan Hugh:** Well…

**Jerry Michalski:** So part of me is looking for a new storytelling tool I can use like I did Prezi. Because we want to curate the collection of things, see the context, and then discover things, and I've been discovering things because of how I curate in the Brain. But then we also want to tell the stories.

**Harlan Hugh:** Yeah. The way the Brain works now, you can think of it as a data store. I can throw all my links in here and bring them back later. To some extent, if you have a brain you built for a specific topic, you can make a presentation out of it. But if you have a brain of all your stuff and you want to make a presentation about just one topic, you might overwhelm people.

**Jerry Michalski:** Yep.

**Harlan Hugh:** Without giving away too much, the other thing we're working on is the ability to tell a story with your brain.

**Jerry Michalski:** Sweet.

**Harlan Hugh:** So a lot of what you're saying is lighting up areas of my brain that are already reasonably well developed.

**Jerry Michalski:** Can you go to "snipped finance"? Snipped, the past tense of "to snip." S-N-I-P-P-E-D. It's not showing up yet. Try "snipped" with… there we go. "Ways We Snipped Long Term Relationships in Finance," that one, the second one. This is a story I recorded as a screencast, a braincast, back during lockdown, in 2020 I think. Where you see the two YouTube links, like [Snip! Examining the Subprime Crisis](https://youtu.be/Z3bog8-vbG0), that's part of a three-video playlist where you'll see the Brain and hear my voiceover trying to explain [the causes of the subprime crisis](https://bra.in/7j3PNr). All the evidence I collected is in here. And just recently, years after posting these, I used Cerebro to go deeper into one part of it, and I was astonished at how good that was. Wow, it really improved a piece of the argument. But again, those videos and this argument are constrained by the complexity of the map I'm showing at the time. It's overwhelming, in the sense of so much information on screen. So wherever you're pointing, I'm interested.

**Harlan Hugh:** Yeah. One of the things you can do with Atlas, which maybe I'll be brave and click the button again, is take a subsection of your brain and show just that. Earlier we were going from one thing and then a couple of generations out. But you can also say, "I want this thought and this thought, and maybe all these thoughts," and let's say this is the core of the story I want to tell. When you go into Atlas now… oh, it worked this time. Here we have our 12 thoughts. I can say, okay, I want to show just these 12 thoughts. Here are all the things I want to talk about. But then I also want to go one layer out from those. So you can build a path through your brain, and then say, "Show this, plus the context around each one." This gives you some idea of what we're thinking about in terms of pulling sections of your brain out and organizing them in a way that makes more sense for presentation or sharing.

**Jerry Michalski:** Love that. Thank you for doing the Atlas demo. I really appreciate it. It's very cool.

**Harlan Hugh:** Happy to do it. It's one of the features we're really excited about, but, as I said, it's not quite done yet.

**Jerry Michalski:** It worked. The second pass on my Brain just took a little longer, but it's early software. There we go. Anything else you want to reflect on, about where you are now, where the Brain is, and how it fits in the universe?

**Harlan Hugh:** How it fits in the universe, that's a good way of thinking about things. I keep coming back to this, but the original vision for the software was: how do we enable people to think about the computer as a way of capturing everything that's in your head, instead of just a way of filing things away? We wanted to create a workspace that mirrors the way you think, so you're not adapting your thinking to the way your computer presents information; the computer presents things the way you think about them.

Over time that's evolved from being all about the single individual, to being able to share it, as we've been talking about, and collaborate on it. And now, in a different world with AI, it's becoming more of a piece of infrastructure. You can use it not just as a user interface, but as a data store that you can query via AI, or via an API, or export to a variety of formats. We're building systems at the company to automate more and more things, and as you can imagine, we've got the Brain at the center of all of that. I think the evolution of the Brain and these kinds of functionality is ideally toward becoming a foundation not just for individuals but for companies and organizations, for the primary knowledge they want to leverage everywhere. And increasingly, the audience for that store is going to be not just people, but also AIs.

**Jerry Michalski:** That goes right toward something I wanted to end on. Maggie Appleton recently wrote an article, [Planning with Agents: Divided Worlds, Boundary Objects, and Thicker Interfaces](https://maggieappleton.com/planning-agents). I'm not done reading and curating it yet, but I think she's pointing where I think I'm pointing. The way we're all interacting with AIs right now is basically in chats, in little apps or on your phone. Over time you collect a whole bunch of chats, more than you can remember having, and you're like, "God, where was that really interesting idea?" It's buried in one of those chats over on the side.

And I'll be doing a separate post about what I'm saying now, so I'm just thinking out loud. When we train up these LLMs, they create some kind of internal representation of what they've learned, through reinforcement learning and all the other algorithms they use. They have some human-incomprehensible internal map in tensor-n-space, whatever that is. Wouldn't it be great to have a boundary object, meaning a thing where we can meet, a map or a drawing or a rendering of a landscape where we can meet and talk, both across humans and between humans and AIs? And for me, [the Brain is a really interesting boundary object](https://bra.in/2jMbbe), because I can say, "It's like this." We were just looking at my heroes, my contrarians, and the context there. If other people fed into that and connected to it, we would have something to return to next time.

Because one of our problems is that every conversation is brand new. We have really intelligent note-taking systems now that give us AI summaries of every Zoom and every Teams meeting, except they're disconnected from each other. They don't live in a context. They don't live as if we were always working on the same sort of stuff and just wanted to make it better. Which is part of the reason to have a boundary object.

And then I came to the Thought Desktop alternatives, because I remember talking to you years ago, when a couple of people were trying to sell Linux laptops that wouldn't have Microsoft or Mac OS loaded, just Linux. At the time, KDE and GNOME, the alternatives for Linux laptops, were ugly, and I think I tried to convince you: [why don't you sell the Brain as part of the file system](https://bra.in/2pKKbr)? Basically replace the file-folder metaphor with this as where things are. And from day zero you've been able to connect things in your Finder or Explorer into the Brain, so that part was done. So just keep going there. Anyway, I think seeing the landscape together is clarifying in ways that just talking with bots, and talking with one another all the time, is going to run out of depth.

**Harlan Hugh:** Yeah. The way we're not storing or organizing our interactions with AI today is much like when we first started using computers and people just put everything in one place. I used to make the analogy that you'd ask somebody, "Hey, where's this document?" And they'd say, "Oh, that's in Word."

**Jerry Michalski:** What do you mean it's in Word? Yeah. I remember, when I lived and worked in New York, visiting an exec at Edelman PR. At one point in our conversation he said, "Whoa, whoa, whoa, I've got the perfect document to show you." And I proceeded to sit next to him for five to seven minutes while he looked through the SharePoint file system, with no good search, trying to find this document. He finally gave up. We both just went, "Nope, guess we're not finding that thing."

**Harlan Hugh:** Yeah. I'm sure it's going to get better, but at the moment we're in very, very early days.

**Jerry Michalski:** But I'm interested in the Brain, and things like the Brain, as the conversational objects that help us communicate better over time.

**Harlan Hugh:** Yeah, we definitely want to be a part of that. We've integrated AI into the Brain, and the way it currently works is at the transitional layer. We talked a month or so ago about temporal versus reference information: things that matter in the moment versus things that matter in the long term. Today we treat conversations with AI, for the most part, as chats. They matter while you're talking, and then they go away.

**Jerry Michalski:** Yeah.

**Harlan Hugh:** But we've started to add some features for capturing that data longer-term in the Brain. Right now, if you have a long conversation with Cerebro, there are ways of getting back to it, just like in every other UI: there's a history, you can search it, all that. But you can also take the conversation and say, "Hey, make a thought for this," and it puts it into your brain. Then you can say, "Connect this up," and it will connect it to all the things related to what you talked about. I think that's a very first, early step in how these things are going to go.

**Jerry Michalski:** Love that. Harlan, thank you. This has been awesome. I'm thrilled you demoed Atlas for me. I hadn't seen it before and didn't suspect you were working on it. It's very, very cool, and I'm looking forward to it.

**Harlan Hugh:** My pleasure. And thank you for always being an enthusiastic Brain user.

**Jerry Michalski:** Well, you really changed my life. Almost 30 years ago, you and your software showed up in my life, and there's Jerry pre-Brain and Jerry after Brain. In fact, there's a thought in my Brain called [Jerry's Brain After Jerry](https://bra.in/6j4PPG). What happens to my Brain and Brain data when I die? That's a conversation for a different moment. But April and I did our wills and all that, and we don't own any Picassos, unfortunately, and no Maseratis, nothing of real value. The thing I've got of value is 30 years invested in this.

**Harlan Hugh:** Yeah. There are a lot of people, probably a higher proportion than for most software, who, when you talk to them, say, "This is the number one thing I do on my computer," or on my phone. The software is a little bit extremist, in that the people who get it are all about it.

**Jerry Michalski:** So my hat's off to you. Thank you for doing something so interesting, and for sticking with it. I remember a call where you demoed Brain version 7, which you were about to release, and it looked nothing like the Plex. The pressure on you to mainstream it and make it look like Office, something more people could understand, was so great that you were leaving the Plex behind. And I was like, "What are you doing? What are you doing?" Fortunately, you stuck with it.

**Harlan Hugh:** Yeah, I remember the call you're talking about. We did try to make a version where the primary interface was not the Plex. There's still merit to it.

**Jerry Michalski:** Well, you have the Card view, and a couple of alternative views still there.

**Harlan Hugh:** Yeah. We need the full menu of ways of interacting with the data.

**Jerry Michalski:** Cool. Thank you very much.

**Harlan Hugh:** Thank you, Jerry.

**Jerry Michalski:** I'll post this, and see you online some more.

**Harlan Hugh:** Very good. We've got lots more cool stuff coming. Thank you for sharing your Brain.

**Jerry Michalski:** Thank you. Peace, bye.

**Harlan Hugh:** See ya.
