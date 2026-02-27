---
title: "Builders Unscripted: Ep. 1 - Peter Steinberger, Creator of OpenClaw"
url: https://www.youtube.com/watch?v=9jgcT0Fqt7U
channel: "OpenAI"
date: 2026-02-24
duration: 31m28s
model: "scribe_v2"
provider: "elevenlabs"
transcription_id: "ljm91isO0tulS2obqbki"
entity_count: 0
tags:
  - transcript
  - youtube
---

# Builders Unscripted: Ep. 1 - Peter Steinberger, Creator of OpenClaw

_Transcript span: 00:00:11 - 00:31:28. Word-level timestamps are in the companion JSON._

## Transcript

### Romain Huet

_00:00:11 - 00:00:12_

Peter, welcome to OpenAI.

### Peter Steinberger

_00:00:12 - 00:00:13_

Thanks for having me.

### Romain Huet

_00:00:13 - 00:00:19_

We've known each other online now for many years, uh, but I'm so happy to finally get the chance to spend more time with you in person.

### Peter Steinberger

_00:00:19 - 00:00:21_

Likewise. Beautiful office, by the way.

### Romain Huet

_00:00:21 - 00:00:36_

Thank you. Thank you. You had a crazy couple of weeks. We first had the idea of doing a video, video together a month ago. If we had done it then, I would have had to intro you. I guess you don't even need an intro anymore. Uh, it's not often that an open source project makes the Wall Street Journal.

### Peter Steinberger

_00:00:36 - 00:00:36_

Nice.

### Romain Huet

_00:00:36 - 00:00:39_

Uh, so congrats on all the success. How are you feeling?

### Peter Steinberger

_00:00:39 - 00:00:55_

Slightly sensory overload on all points. But also, you know, when I, when I started out this year, like messing with AI, I wanted to, like, inspire people, and I feel like this is the final form. So I'm, I'm, I'm proud.

### Romain Huet

_00:00:55 - 00:01:05_

It's been amazing. You've been in SF for the past week, uh, and you attended some events like the Codex Hackathon, but you also had ClaudeCon, like an event dedicated to OpenClau.

### Peter Steinberger

_00:01:05 - 00:01:07_

Well, it also was created by the community.

### Romain Huet

_00:01:07 - 00:01:07_

Yes!

### Peter Steinberger

_00:01:07 - 00:01:32_

I created this Discord channel about meetups. After, people were like: "We need to have a meetup." And I'm like: "Sure!" And then I came to ClaudeCon, and there were, like, a thousand people, and I was just blown away by, like, the creativity, the, the, the colors. Like, there were so many things, so many people excited.

### Romain Huet

_00:01:32 - 00:01:40_

I mean, that's how you realize that you've built something magical. Like, the project did not even exist a few weeks ago, and now you have, like, thousands of people embracing it-

### Peter Steinberger

_00:01:40 - 00:01:40_

Yeah

### Romain Huet

_00:01:40 - 00:01:43_

... using it, gathering to meet you in SF. It's pretty-

### Peter Steinberger

_00:01:43 - 00:01:43_

Even, even-

### Romain Huet

_00:01:43 - 00:01:44_

... incredible.

### Peter Steinberger

_00:01:44 - 00:01:51_

Even in Vienna next week, we have, like, already three hundred people, and it's by far not as much of a tech scene-

### Romain Huet

_00:01:51 - 00:01:51_

Wow

### Peter Steinberger

_00:01:51 - 00:01:53_

... as, as San Francisco.

### Romain Huet

_00:01:53 - 00:01:54_

It's now worldwide.

### Peter Steinberger

_00:01:54 - 00:01:54_

So now it's-

### Romain Huet

_00:01:54 - 00:01:55_

It's a phenomenon.

### Peter Steinberger

_00:01:55 - 00:02:01_

Yeah, that's amazing that, that this reaches different continents, different cultures.

### Romain Huet

_00:02:01 - 00:02:09_

Indeed. And, and so how has the conversation been with, like, the community here? You spent time with the community, some of the maintainers also that you've-

### Peter Steinberger

_00:02:09 - 00:02:09_

Yeah

### Romain Huet

_00:02:09 - 00:02:11_

... kind of like brought into your project.

### Peter Steinberger

_00:02:11 - 00:02:11_

Yeah, yeah.

### Romain Huet

_00:02:11 - 00:02:14_

Um, how has that been for you this week?

### Peter Steinberger

_00:02:14 - 00:02:15_

It's been quite something.

### Romain Huet

_00:02:15 - 00:02:15_

Yeah.

### Peter Steinberger

_00:02:15 - 00:02:35_

Um, a lot of people love it, and a lot of people have this expectation of this enterprise-ready final product, when for me, for the longest time, it was like my, my little playground. I mean, the whole year, I'm just marveling at what's possible now. If you're a builder, this is like, what a time to be alive.

### Romain Huet

_00:02:35 - 00:02:46_

Yeah. What, what do you think is the most interesting thing about building-- like, actually building, being a builder at this moment in time? Like, the, it's a very interesting time where, like, the entire tool chain is changing.

### Peter Steinberger

_00:02:46 - 00:02:47_

Yeah.

### Romain Huet

_00:02:47 - 00:02:50_

The definition of what it is to be a developer is also changing, and anyone-

### Peter Steinberger

_00:02:50 - 00:02:50_

Right

### Romain Huet

_00:02:50 - 00:02:51_

... can build anything.

### Peter Steinberger

_00:02:51 - 00:03:24_

When I, when I started playing with, with this new tech, I got a dopamine hit every time. Back then, I started with Cloud Code, when it got something right, and it was, like, maybe thirty percent or forty percent chance, but I-- to me, it was like, like, literally mind-blowing because I had this realization that now I can just build anything. And it, um...

You know, usually, you're so time-constrained because software is hard, and software is still hard, but you're so much faster now.

### Romain Huet

_00:03:24 - 00:03:35_

I agree. Uh, so if we take, um, a few years back maybe, and rewind a little bit. So you-- I, I got first got to know your work back, I think, in twenty eleven or twenty twelve when you built PSPDFKit.

### Peter Steinberger

_00:03:35 - 00:03:36_

Yeah.

### Romain Huet

_00:03:36 - 00:03:50_

And from the outside, it's interesting because it feels like you've achieved the dream of every developer. You're gonna solve a problem, you created a, a great solution for it, you built a company around it, you scaled it, you sold it. But I'm sure that journey is never that easy.

### Peter Steinberger

_00:03:50 - 00:04:16_

I mean, I didn't wake up one day and thought, "I'm gonna build a PDF framework." That is, like, minus one hundred on my interest list. Uh, so it kinda, kinda just happened, like a weird butterfly effect from being at the Nokia development days to having friends that needed it, uh, and an American visa taking too long kinda emerged to me creating a company.

### Romain Huet

_00:04:16 - 00:04:22_

What I find interesting is, like, after that company, uh, you, you built, you kinda took a break for a little while.

### Peter Steinberger

_00:04:22 - 00:04:23_

Yeah.

### Romain Huet

_00:04:23 - 00:04:24_

So what brought you back?

### Peter Steinberger

_00:04:24 - 00:05:09_

At the end, I, I was just really burned out. Like, I was running on high steam for thirteen years. Running a company is hard. Being a founder is hard. It's-- and I also didn't really... It's my first one, so I didn't really have the, the knowledge how to, how to mitigate those things. So I was just burning a bit too bright, and I needed to decompress. So I still followed the tech news.

I, I saw, I think, the very early things of GPT Engineer, or whatever it was called, of ChatGPT, and I was, uh, it was kinda cool, but didn't really excite me. It's... You always have to experience new technology. Just by reading from it doesn't really convey the power.

### Romain Huet

_00:05:09 - 00:05:09_

Mm.

### Peter Steinberger

_00:05:09 - 00:05:46_

So, so even though that tech didn't really click, and only when I was ready, when I felt the need for, like, okay, I, I wanna build something again, and then I, I didn't wanna build it in Apple tech anymore 'cause I, I'd done this for such a long time, and the world kind of moved on a little bit, you know? You need to-- things need to be built first.

And I, I kinda had the hinge back then, but it's so hard when you go from when you're such an expert in one field and you move to another field. Hard is even the wrong word. It's, it's more like painful.

### Romain Huet

_00:05:46 - 00:05:46_

Mm-hmm.

### Peter Steinberger

_00:05:46 - 00:06:17_

'Cause then you're like, you have all this, this broad knowledge of how to build things, but to really do that without agentic engineering, you need to still learn a lot to, to move your knowledge over....

And then I thought like, "Oh, let's, let's check out what this AI stuff is." The moment where it, it blew my mind was I, I took this project that was halfway done, that where I just-- yeah, it burned out before finishing it, basically.

### Romain Huet

_00:06:17 - 00:06:24_

It's often the case that, like, for us developers, we love having new ideas and starting projects, but getting them to the finish line is the hard part.

### Peter Steinberger

_00:06:24 - 00:07:24_

Oh, yeah, I see it all the time. It's, it's, it's, it's really hard, and I even sometimes fail. But for this one, I, I wanted to continue, but I also wanted to rewrite it. So I, I took the whole thing, I made one huge markdown file, like, I don't know, one point five megabyte, with all the files. I dragged it into Gemini Studio, two point five at the time.

I said, "Write me a spec," and then I had, like, this four-line spec, then I dragged it into Cloud Code, and then I wrote build. And then I, I did other stuff on the main screen. It was just, like, running on the side screen for hours. It was, it was-- things were quite a bit rough back then.

And at one point, it t- it told me, "I'm one hundred percent production ready," you know, like the, the sacrilegious, uh, Opus three point five or whatever it was, and I tried it, and it crashed. And then I, like, hooked up, um, Playwright, I think one of the few MCPs that I would actually use, and told it to, like, build the login stuff, um-

### Romain Huet

_00:07:24 - 00:07:25_

And check the work along the way.

### Peter Steinberger

_00:07:25 - 00:07:32_

Yeah, it was something for Twitter. And then one hour later, it, it actually worked, and it did show me some stuff.

### Romain Huet

_00:07:32 - 00:07:32_

Mm-hmm.

### Peter Steinberger

_00:07:32 - 00:07:47_

I mean, it was, like, the worst slop, but to me, this was, like, the moment where it really clicked, 'cause, like, this is, like, just process-wise, I got, like, goosebumps for, like, the possibilities, and that was kind of the moment where I couldn't really sleep anymore.

### Romain Huet

_00:07:47 - 00:07:47_

Yeah.

### Peter Steinberger

_00:07:47 - 00:07:58_

'Cause by now, then, then, like, my head exploded with all the things that I, I always wanted to build that I just couldn't before, and then I just really went into the rabbit hole.

### Romain Huet

_00:07:58 - 00:08:11_

A lot of people have seen, like, OpenClau as an overnight success for you. But what I love and I-- what I find fascinating in your story is kind of how it's a culmination of so many projects that you've been working on for the past, like, nine or ten months, right?

### Peter Steinberger

_00:08:11 - 00:08:11_

Yeah.

### Romain Huet

_00:08:11 - 00:08:16_

Like, when you look at your GitHub profile, there's, like, forty-plus projects you've built, um-

### Peter Steinberger

_00:08:16 - 00:08:18_

Half of them I use in the project, yeah.

### Romain Huet

_00:08:18 - 00:08:22_

Yeah, and I think, like, many of those, yeah, you, you combined them all inside OpenClau.

### Peter Steinberger

_00:08:22 - 00:08:23_

Yeah.

### Romain Huet

_00:08:23 - 00:08:29_

Can you tell us more about this journey, about, like, how all of these ideas and projects made their way to OpenClau?

### Peter Steinberger

_00:08:29 - 00:08:48_

I wish I could say that I had the unified plan in the beginning, but a lot of it was just exploration, and I wanted things, and those things didn't exist, and, and I just yield them, or let's say I prompted them into existence. Why? You know, it's like: Okay, let's build it.

### Romain Huet

_00:08:48 - 00:08:48_

And then, like-

### Peter Steinberger

_00:08:48 - 00:08:49_

And, and, and it was, like-

### Romain Huet

_00:08:49 - 00:08:50_

Step by step

### Peter Steinberger

_00:08:50 - 00:09:12_

... step by step, just because I, yeah, I wanted my agent to, like, do some stuff for me. I still-- I didn't have the, this, this, this unified vision yet. I, I had a... It's funny how it goes full circle, 'cause I, I wanted to have something that would look at, for example, my WhatsApps, and then I built-- I even got the, the domain for that. I built a prototype, but then I thought-

### Romain Huet

_00:09:12 - 00:09:12_

Yeah

### Peter Steinberger

_00:09:12 - 00:09:57_

... "All the big labs are gonna build it." And I was like: I just wait a little bit. I focused on other stuff. I just experimented a lot. I-- my mission was kinda like to have fun and inspire people. And then by November, I, I built a few versions of what I wanted, but nothing really good. And by November, I was like: Am I still-- Why did no lab still build any of that?

You know, like, what the, what the heck are they doing? And then I, I built the first version that became OpenClau. We're at name number five now. Um, still didn't fully click for me. It was like, "Oh, this is cool." Like, took, like, one hour to, like, build the first prototype, 'cause you just, you just yield things into existence now.

### Romain Huet

_00:09:57 - 00:09:59_

Mm-hmm.

### Peter Steinberger

_00:09:59 - 00:10:35_

And then where it really clicked was where I was at this, uh, weekend trip in Marrakech, and I, I found myself using it way more because it was so convenient, you know. Like, there was no, there was no really good internet, so WhatsApp was... WhatsApp just works everywhere.

Um, and it was just so convenient with like, I mean, pictures for, for to, to translate stuff, to, like, find me restaurants, but also, like, look up stuff on my computer. It was really cool. And I showed it to friends, and I, I made it, like, send mess- text messages for me, and, and they wanted it, you know? And I'm like: "Yeah, you, you shouldn't use it. You don't get that." It's too dangerous for now.

### Romain Huet

_00:10:35 - 00:10:39_

These are the early signs of like, you know, uh, product market fit. If your friends already want-

### Peter Steinberger

_00:10:39 - 00:10:39_

Yeah

### Romain Huet

_00:10:39 - 00:10:45_

... what you have, even though you're gonna never design that for them, it was more, like, reserved for the technical, like, peers that you have.

### Peter Steinberger

_00:10:45 - 00:10:55_

Yeah. And then when it really clicked for me was, I used it so much, and at some point I sent, like, a voice message, and, and then I was like: Wait, this shouldn't work.

### Romain Huet

_00:10:55 - 00:10:58_

Oh, yeah, tell me more about that story, 'cause I think we talked about it the other day.

### Peter Steinberger

_00:10:58 - 00:10:58_

Yeah.

### Romain Huet

_00:10:58 - 00:10:59_

That's fascinating.

### Peter Steinberger

_00:10:59 - 00:11:18_

Yeah. It showed me how good those models are in problem-solving. You know, like, we built these things for atten- for attending engineering, but really, the skill is, like, more abstract. Like, it's... If you wanna be a really good coder, you need to be a really good problem solver, and that just maps in any domain, really.

### Romain Huet

_00:11:18 - 00:11:19_

Yeah.

### Peter Steinberger

_00:11:19 - 00:12:03_

So I, I sent this voice message, and the typing indicator appeared, and, and I'm like: I'm, I'm very curious what happens now. This is-- I didn't build this. Can't work. And then the model just replied to me, and I was like: How did you do that? You know, it's just like, ask the model, like: W- how? Why? This should not work.

And the model was like: "Yeah, you sent me a, a message, but it was just a file with no file ending, so I just looked at the file header and found that it's Opus, the, the audio codecs. So I used FFmpeg on my computer to convert it, and then I wanted to, to transcribe it, but it didn't have Whisper installed.

So I found-- I looked around, and I found an OpenAI key, and I used Curl to just send the file to OpenAI and got the text back, and here I am."

### Romain Huet

_00:12:04 - 00:12:11_

... this is incredible. I mean, like, that's the power of, like, giving tools and the complete access to a computer to these, like, agents.

### Peter Steinberger

_00:12:11 - 00:12:11_

Yeah.

### Romain Huet

_00:12:11 - 00:12:16_

And now they can just, like, actually come up with the solutions themselves, even though you never programmed them at all.

### Peter Steinberger

_00:12:16 - 00:12:39_

It's funny, like I, I told a story, and then people are like: "Oh, my God, it just used your key, like, this is madness!" I'm like: "No, like, I put it in, in the environment exactly for that reason." If it's- it's kind of like a script that should access my OpenAI key, like my bot works in the same, in the same environment. Of course, it should access my OpenAI key. Like, I put it there for that reason.

This is not bad. This is exactly what I wanted.

### Romain Huet

_00:12:39 - 00:12:39_

Yeah.

### Peter Steinberger

_00:12:39 - 00:12:57_

Yeah, that's, that's- I had my little moment, and then every time I, I show it to friends, I put them in a little group chat. Uh, and I like to be- to be frank, like, this, this thing is designed for one-on-one communication, right? So if you put it in a group chat, pick someone that you trust.

### Romain Huet

_00:12:57 - 00:12:57_

Really trust, yes.

### Peter Steinberger

_00:12:57 - 00:13:05_

Yeah, because it was not designed for, "Oh, let's just put it out there, and it'll always do the right thing," you know. It, it is your personal assistant, uh-

### Romain Huet

_00:13:05 - 00:13:35_

Yeah, when I set it up, I was also very intrigued. I was like, "This is a weird setup." I'm like: Where is this gonna take me? Uh, but I had to also a few, like, aha! moment, where, like, the more access you give it, the more tools and skills you give it, the more impressed you can become. You also give it like a Vercel skill, and then you ask it to build a website or application even for an event you want to host.

Not only is it building the app, it's also using your OpenAI key to, like, make some AI features into it. It's deploying it to Vercel. There's already a link you can share with friends.

### Peter Steinberger

_00:13:35 - 00:13:35_

Yeah.

### Romain Huet

_00:13:35 - 00:13:42_

It's a kind of, like, mind-blowing step-up change versus just like: "Oh, I'm augmenting myself to write code."

### Peter Steinberger

_00:13:42 - 00:14:33_

So throughout November and December, I was, like, hooked on this, and I... I mean, I, I still did some other projects, but, like, most of my time went there. But on, on Twitter, people wouldn't get it, and I was like, I've got very muted responses. And I'm like, every time I show it to a friend, they wanted it, and I'm like: "No, no, it's not ready yet," you know?

So then I was like: "Okay, what's the most insane thing I can do to, like, show people how cool this is?" So I created a Discord and just put my, my bot in there without any security because back then I didn't even had sandboxing built in. It was just very early, and I just worked in the open. I basically built now OpenClaw vs OpenClaw and debugged it, and then asked the model.

I was like: "Oh, do you see this tool called?" "No, I see nothing." It's like: "Oh, yeah, check, check your own source code," and, and, and, and, and did a whole bunch of other stuff, and people saw it, and then they understood.

### Romain Huet

_00:14:33 - 00:14:42_

And when you, uh, put it in Discord like this, what kind of access did you give it? Did you also give it, like, all your tweets, for instance? Like, what kind of, like, knowledge did, did it have about you?

### Peter Steinberger

_00:14:42 - 00:15:11_

Not all my tweets. It's too many, um, but a lot of my memory stuff, yeah. So I actually was monitoring it very quickly because, yeah, prompt injection is unsolved, but also the latest generation of models is really good. So I have, like, one canary, my soul.md, that kind of defines what are my values, h- how do I want the model to, to work, to operate, to think, what's important to me. That's secret.

### Romain Huet

_00:15:11 - 00:15:11_

Yeah.

### Peter Steinberger

_00:15:11 - 00:16:02_

And, and people really wanted that. And, and then random people came in and tried to, like, prompt inject it and pasted, like, huge blocks of code, and the model was like: "I'm not reading this." So it was basically mocking them, but I was still not very confident, right? So, uh, the first night was like- got me a whole lot of interest, and then I, I turned it off, went to bed, slept, like, ten hours, woke up.

There was, like, eight hundred messages on, on, on Discord. My agent was replying to every single one. I freaked out. Like, I turned it off again. I read through every single thing, and, and at some point, I chilled out because it actually didn't-- it didn't do anything malicious. It didn't manage to get my soul.md out. I'm not saying this is...

I'm sure prompt injection is possible, but it's not as easy as people think it is.

### Romain Huet

_00:16:02 - 00:16:05_

Right. In the grand scheme of things, it was actually performing the way you wanted it to.

### Peter Steinberger

_00:16:05 - 00:16:09_

Yeah. My big mistake was I, I disabled it, but I forgot that I actually had a launch daemon.

### Romain Huet

_00:16:09 - 00:16:09_

Mm.

### Peter Steinberger

_00:16:09 - 00:16:15_

What, what's the, the main thing a launch daemon does? If this thing crashes or is killed, it restarts it.

### Romain Huet

_00:16:15 - 00:16:15_

Yeah.

### Peter Steinberger

_00:16:15 - 00:17:02_

'Cause you want a reliable service, and like, Apple built this to be a reliable service, and I, I just didn't think about it. So I killed it, and it restarted it in five seconds while I went to sleep. Now I know better, but now I'm also-- I also put in sandboxing, so... He was so proud that it, it's in his next studio. It calls it the castle, and then I put it into a little, little set container.

But, you know, those models are so creative. Like, the first time I, I, I made a-- I made an Alpine Docker container, and there's, like, nothing in it, and I, I, I told now Multi, like: "Hey, can you check out this website?" And, and it was like: "There's not even curl. There's nothing in here." And I'm like: "Be creative." So it built, it built, um, Lobster Curl, just by like-

### Romain Huet

_00:17:02 - 00:17:03_

Its own tool?

### Peter Steinberger

_00:17:03 - 00:17:14_

... It just built its own t- its own curl, by, like, using some, some TCP socket, and, like, there was, like, a C compiler, and then it had, like-- it built, like, a crappy version of curl, so it could actually access the website, and it worked.

### Romain Huet

_00:17:14 - 00:17:14_

Crazy.

### Peter Steinberger

_00:17:14 - 00:17:18_

So, like, those things are so resourceful. It's incredible.

### Romain Huet

_00:17:18 - 00:17:31_

Yeah. You had some challenges, too, with like, you know, people really, like, uh, taking a look at, like, the security p- issues potentially, and expecting you to have, uh, everything so robust from day one, although you were just putting an open source project out there.

### Peter Steinberger

_00:17:31 - 00:17:45_

I always laugh when people ask me, like: "Oh, yeah, can you put me in with, like, the CEO, or human resources, or some other member of my team?" And I'm like: "It's just me hacking from my cave, basically."

### Romain Huet

_00:17:45 - 00:17:45_

Uh-

### Peter Steinberger

_00:17:45 - 00:17:48_

But, like, but you... That, that's where you see the dissonance, right?

### Romain Huet

_00:17:48 - 00:17:48_

Yes.

### Peter Steinberger

_00:17:48 - 00:17:59_

This would have not been possible by any human, any one human. Uh, yes, I have maintainers now, and I get PRs, but essentially, I built this.

### Romain Huet

_00:17:59 - 00:18:00_

Yeah.

### Peter Steinberger

_00:18:00 - 00:18:08_

Even a year ago, it wouldn't have been possible. There is no model for, like, something like this could be built by one person.... so it's not even, they don't even consider that.

### Romain Huet

_00:18:08 - 00:18:37_

Right. Yeah. Let's actually touch on that. Like, I think, um, on, on your, like, productivity, 'cause I'm sure, like, many developers must be wondering, like, how is Peter so productive? And I was looking at your, uh, GitHub again this morning, and I saw it's like 90,000 contribution on more than 120 projects just this past year.

But what's also interesting is, like, you know, the past year started very white on the GitHub activity graph, and then light green, and then in the fall, around October, November, it's very dark green.

### Peter Steinberger

_00:18:37 - 00:18:37_

Yeah.

### Romain Huet

_00:18:37 - 00:18:37_

Um-

### Peter Steinberger

_00:18:37 - 00:18:38_

That's where-

### Romain Huet

_00:18:38 - 00:18:40_

What happened in the fall?

### Peter Steinberger

_00:18:40 - 00:19:12_

I switched to Codex. Like, uh, with every generation they got better, but it's not just that the agents got better, the harnesses got better, also my understanding of how to approach this and my workflow got better. You know, there's these people that they write software in the old way, and the old way is gonna go away. And they try... They call it vibe coding. I, I think vibe coding is a slur.

And then they try AI, but they don't understand that it's a skill.

### Romain Huet

_00:19:12 - 00:19:12_

Mm.

### Peter Steinberger

_00:19:12 - 00:19:53_

You know, you, you pick up the guitar, you're not gonna be good at the guitar on the first day. So they're gonna have a bad experience, and then they, they're like, "Oh, no, it's not gonna work." While if you approach it more like playful, it- you have to learn, you have to, like... I have a gut feeling now for, like, which prompt will-- and how long it'll take.

And if it takes longer, I'll, I reflect, "Oh, maybe I made a mistake, maybe my architecture is wrong, my thinking was wrong, or maybe something else." Just as with code, if you, if you, if you write code and, and you have a feeling of, "Oh, this is, this naturally goes into my architecture," or, "This is, this is... I'm fighting the, the system." And it just takes time.

### Romain Huet

_00:19:53 - 00:20:01_

And so if people want to become more like you, uh, what is your Codex setup today? 'Cause I think you famously said, like, "Most people overcomplicate their setup."

### Peter Steinberger

_00:20:01 - 00:20:58_

I mean, I also overcomplicated my setup. I, I call it the agentic trap. From your first touch point in a new technology to, like, becoming really effective, a lot of people get stuck in there trying to, like, super optimize their setup. Doesn't really make you more productive, but it feels like you're more productive. So, like, I put out this one blog post that was also very controversial, but I just talk to it.

Like, you just approach it like a conversation. Like, your model is, like, your... It's not really pair programming, uh, it's something different. You know, it's, it's, it's a conversation. I basically tell what I want. I always ask the model: "Do you have any questions?" For some reason, like, there's always questions.

But the model by default is trained to just solve your problem, and then would just make assumptions. The default assumptions might not always be the best ones, especially you have to remember, it's trained with a lot of code and also a lot of older code. "Do you have any questions?" is, like, a very important-

### Romain Huet

_00:20:58 - 00:20:58_

Yeah

### Peter Steinberger

_00:20:58 - 00:21:04_

... question. People don't realize that the model usually starts with a blank slate, 'cause they don't learn like us.

### Romain Huet

_00:21:04 - 00:21:04_

Mm-hmm.

### Peter Steinberger

_00:21:04 - 00:21:13_

Like, every new session is like: I know nothing about this code base, and I'll just search and find the little things that you ask me to, and then try to solve it.

### Romain Huet

_00:21:13 - 00:21:14_

Mm.

### Peter Steinberger

_00:21:14 - 00:21:42_

But they don't see usually the whole picture. If you do this properly, you have to have the full picture in your head, and you have to, like, help the model a little bit to motivate it to, like, look here, look there. And Codex is just much better at taking a broad look first. I used a very, a very basic approach. I don't even use work trees; I just have, have check out one to ten, basically.

Keeping it simple helps me to focus more on the actual problem.

### Romain Huet

_00:21:42 - 00:21:43_

Yeah.

### Peter Steinberger

_00:21:43 - 00:21:55_

So I don't even want to deal with branches or work trees, I just focus on different problems. Ideally, that gets easier if the project becomes a little bit larger, then you can work on different things that don't fight each other so much.

### Romain Huet

_00:21:55 - 00:21:58_

You used Codex a ton to build OpenClaw.

### Peter Steinberger

_00:21:58 - 00:21:58_

Yeah.

### Romain Huet

_00:21:58 - 00:22:00_

Um, how has Codex changed the way you work?

### Peter Steinberger

_00:22:00 - 00:22:29_

Well, I tried a lot of tools, and what I like about Codex is that my trust in it building what I want from all the tools right now is the highest, and the number of things that just work is really high. And what-- I don't think what people realize is that with GPT 5.2, it was again like a quantum leap in terms of, "Yeah, this will just work." I'm still amazed how well this already works.

### Romain Huet

_00:22:29 - 00:22:32_

That's fantastic. We can just build things. Uh, this is pretty incredible.

### Peter Steinberger

_00:22:32 - 00:22:35_

Yeah. Like, people need to give this a try.

### Romain Huet

_00:22:35 - 00:22:39_

You famously said also that, like, you're shipping code now that you're not even reading.

### Peter Steinberger

_00:22:39 - 00:22:39_

Yeah.

### Romain Huet

_00:22:39 - 00:22:40_

How has that changed?

### Peter Steinberger

_00:22:40 - 00:22:41_

Most code is boring.

### Romain Huet

_00:22:41 - 00:22:41_

Mm.

### Peter Steinberger

_00:22:41 - 00:23:21_

Like, most code just transforms one shape of data into another shape of data, and eventually the user sees it or it goes somewhere else. So, like, on most, most code it writes, I'm-- I have a pretty good understanding of what it writes, and it's enough to, like-- that I, I see the stream, uh, and see that, okay, like, the mental model I have in my head of what it creates is approximately what it creates. I was...

I led a team before, right? I had a lot of software engineers under me, and that also requires accepting that they will not write exactly the same code that I want. In the end, you, you should optimize a code base so agents can do their best work- ... which is not always the same as humans can do their best work.

### Romain Huet

_00:23:21 - 00:23:22_

Right.

### Peter Steinberger

_00:23:22 - 00:23:36_

It also means accepting that maybe the code is not exactly how I would like it, how I would write it, and I, I could push the model towards that. But oftentimes, there's so many ways how you can structure something that often it doesn't matter. If it becomes a performance problem, you just focus on that, you make it better.

### Romain Huet

_00:23:36 - 00:23:49_

And your point that you just made on, like, you kind of like you-- the value of code and how you approach code is also changing a lot how you approach open source, right? Because, like, I was looking at, like, OpenClaw. You now have, like, two thousand PRs open right now.

### Peter Steinberger

_00:23:49 - 00:23:50_

Yeah, you're crazy.

### Romain Huet

_00:23:50 - 00:24:05_

You know, before, before we had, like, AI, you know, you would have to read all of these PRs because there was value in the code being created. But sometimes now you refer to that as, like, not a pull request, but a prompt request almost-

### Peter Steinberger

_00:24:05 - 00:24:05_

Yeah

### Romain Huet

_00:24:05 - 00:24:10_

... 'cause, like, more the idea or the intention behind the PR that's more important than the code itself.

### Peter Steinberger

_00:24:10 - 00:24:14_

PRs actually sometimes take me longer than if I would approach it myself.

### Romain Huet

_00:24:14 - 00:24:14_

Mm-hmm.

### Peter Steinberger

_00:24:15 - 00:24:51_

... because my trust in the model not being malicious is much higher than an external contributor that I never heard of before and where we had no discussion before. So I have to scrutinize it a little bit more.

But then if I see a PR, my-- like I, I start to review it, and my first question to the model is, "Do you understand the intent of the PR?" Because I don't really care about the code, I care about what is the person actually trying to solve. You know, it's, it's more like an issue with like a, "Here's my attempt of a solution." But first of all, many, many people still don't really know how to yield the agent.

### Romain Huet

_00:24:51 - 00:24:51_

Mm.

### Peter Steinberger

_00:24:51 - 00:25:41_

And then often it's just a very localized solution because they, they don't have the full system in their head. The hard part is, how does this little new feature fit into my whole, my, my bigger system? Or how does this little fix-- okay, this little fix fixes a tiny thing, but is it even the right fix? Sh- is it, is it... It's probably often is like a more systemic or an architecture issue.

So the model is actually really good if you, you just have a conversation. And then, and when I say, "Okay, now build this," then it will start to build this. So I ask the model: What's the, what's the intent? Is that the most optimal solution? Sometimes it says yes. Most often it would say no. Then I would start to explore what would be the, what would be the, the best fix. Is this like an architectural problem?

Is this something that is... Let's say it's, it's a problem in message handling. Does this only affect WhatsApp, but maybe also, I don't know, Signal?

### Romain Huet

_00:25:41 - 00:25:42_

Yeah.

### Peter Steinberger

_00:25:42 - 00:25:58_

So, so should we, uh, should we solve this in a more general way? Is this a new feature? Do we even want a new feature? Um, so sometimes this discussion go on for like ten, fifteen minutes. I, I use like voice because it's literally like you, you talk to a very smart coworker.

### Romain Huet

_00:25:58 - 00:26:01_

Easier to give tokens of a voice than, like, typing.

### Peter Steinberger

_00:26:01 - 00:26:26_

Yeah. When, when I'm happy, then I, I have like one slash command, like Glenn PR, that explains the whole procedure to like actually create a branch, do all the changes, get the PR merged. I, I wanted to create a community, so I, I try to still credit the person that created it, even though the whole thing takes me longer than if I would just write it all myself.

### Romain Huet

_00:26:26 - 00:26:26_

Right.

### Peter Steinberger

_00:26:26 - 00:26:31_

Um, but I appreciate that people want to be part of this.

### Romain Huet

_00:26:31 - 00:26:47_

What's your vision for OpenClaw now, going forward with all of these contributors that are kind of like surrounding the project? And, and do you see yourself as kind of a trailblazer for this idea of like a, what a personal AI agent should look like, so that, you know, a billion people can one day use something like that?

### Peter Steinberger

_00:26:47 - 00:27:19_

Yeah. I want to find the balance between this is something that my mom can install, but also this is something that's fun and hackable, which is difficult. You know, most open source projects, you like download the package, but for the longest time, my default install was Git clone, build, run. And then you literally have the source code on disk, and the agent sits in the source code and is aware of the source code.

And if you don't like anything, you, you literally prompt the agent, and it would change itself.

### Romain Huet

_00:27:19 - 00:27:19_

Mm-hmm.

### Peter Steinberger

_00:27:19 - 00:28:07_

Like, like actual self-modifying software. So a lot of people that never sent me a PR sent me a PR. That- that's also why it's more like a prompt request, because they just like the understanding of how to build software that lasts. And at the same time, the whole world is, is...

or the whole security industry is like putting their eyes on it, which has been interesting and also a little bit frustrating 'cause it, it misses some nuance, right? For example, the, the web server that I have, that's meant for you. Initially, I built it for debugging, and then I made it pretty, but it's only meant to be accessible in your network, in your trusted network.

But because it should also be like a hacker's pla- a hacker's paradise, there is an option how you can, like, change that.

### Romain Huet

_00:28:07 - 00:28:07_

Right.

### Peter Steinberger

_00:28:07 - 00:29:06_

Because, like, some people have weird setups, maybe they use, like, Ngrok, maybe they use reverse proxies. So there is a reason why I didn't want to, like, limit that. But now we have, like, people that put it on the open internet, even though I'm screaming in a security document, "Please don't do that.

That's not, that's not what it's intended for." And then I have the security people that point out that, "Oh, yeah, it doesn't have login limitations," you know, like it doesn't have all these things that you need when it's on the public internet. And like, yeah, I didn't build it for that, with that intention, but because it is configurable, it totally counts as a, as a CVS S10.

Uh, so yeah, I, I, I struggled a little bit with that, uh, but now I, I brought on actually a, a security expert. That's the main focus. I, I realize I cannot stop people from using it in ways it was not intended, so my, my big focus now is to, like, support all these use cases and help people not shoot themselves in the foot.

### Romain Huet

_00:29:06 - 00:29:12_

Right. That's the beauty of open source. People can embrace it and, like, come up with ideas that you didn't even think about.

### Peter Steinberger

_00:29:12 - 00:29:14_

Yeah, that's the beauty and the madness of it.

### Romain Huet

_00:29:14 - 00:29:34_

Yeah. Zooming out maybe for a second beyond OpenClaw, like, I've talked to a bunch of developers this week, um, who knew you were coming to the CodeX hackathon, and they told me, like, "How many... Like, how come does, like, Peter come up with all these great ideas?

Like, how does Peter come up with so much creativity?" I don't know if you have any answer to that, or if it's more like your own curiosity that you're following.

### Peter Steinberger

_00:29:34 - 00:29:55_

It's more like this realization that stuff's easy now. So even if I find an open source thing that maybe solves my problem to seventy%, I'll just build it myself, which would have been absolutely impossible a year ago even. And now it's just like, I just prompt it, then it's on a second screen, and, and code works.

### Romain Huet

_00:29:55 - 00:30:12_

We're both from Europe. When I travel outside of SF, and I go back to Europe, I'm sure you feel the same way, like, many developers and engineers have not embraced CodeX and agentic tools just yet. What would be your advice for them, like, as they get started and, like, should rethink the way they work and their workflow?

### Peter Steinberger

_00:30:12 - 00:30:37_

My first advice always is, like, approach it in a playful way. Build something that you always wanted to build. I, um, if you are at least a little bit of a builder, there has to be something on the back of your mind that you want to build. Like, just, just play. You just have to approach this, this, this thing playful.

'Cause like, I think the NVIDIA, NVIDIA CEO said that in the near term, you're not gonna be replaced by AI, you're gonna be replaced by someone who uses AI.

### Romain Huet

_00:30:37 - 00:30:38_

Which is, yeah, better than you, yeah.

### Peter Steinberger

_00:30:38 - 00:30:49_

But if your identity is, "I wanna, I wanna create things, I wanna solve problems," if you're a high agency, if you're smart, you will be in more demand than ever.

### Romain Huet

_00:30:49 - 00:31:01_

Yeah. Well, it's such a great time for builders who embrace these tools, shape their curiosity, and really can bring any ideas to life, the exact same way you've done with all of these great projects and, and OpenClaw.

### Peter Steinberger

_00:31:01 - 00:31:04_

I think in a year, this is gonna, this is gonna explode.

### Romain Huet

_00:31:04 - 00:31:10_

Yeah, twenty twenty-six will be an interesting one. I think it's a fantastic way to end. Thank you so, so much, Peter, for your time.

### Peter Steinberger

_00:31:10 - 00:31:11_

Thanks for having me.

### Romain Huet

_00:31:11 - 00:31:28_

Uh, wonderful to spend time with you. We all at OpenAI love your work. We love supporting builders like yourself, and honestly, you're a true inspiration for the broader developer community. Thanks again, and we can't wait to see what you're gonna work on next.
