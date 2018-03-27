---
title: "Weekly Recap, 1531: Deploying Transcripto, Women Who Code: Her 2.0, First Century Ride in 2018."
tags: ["weekly-recap"]
date: 2018-03-25T23:07:44+08:00
---

On the 1531st week of my life, I:

- Read: [Domain-Driven Design, by Eric J. Evans.](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215) Nearly finished, I hope!
- Read: [Little Bets: How Breakthrough Ideas Emerge from Small Discoveries, by Peter Sims.](https://www.amazon.com/Little-Bets-Breakthrough-Emerge-Discoveries/dp/1439170436)
- Read: [Linchpin: Are You Indispensable?, by Seth Godin.](https://www.amazon.com/Linchpin-Are-Indispensable-Seth-Godin/dp/1591844096)
- Read: [So Good They Can't Ignore You: Why Skills Trump Passion in the Quest for Work You Love](https://www.amazon.com/Good-They-Cant-Ignore-You-ebook/dp/B00FOVTOMA/)
- Read: [Eloquent Ruby, by Russ Olsen.](https://www.amazon.com/Eloquent-Ruby-Addison-Wesley-Professional/dp/0321584104)
- Reading: [The E-Myth Revisited: Why Most Small Businesses Don't Work and What to Do About It, by Michael E. Gerber](https://www.amazon.com/Myth-Revisited-Small-Businesses-About-ebook/dp/B000RO9VJK/)
- Reading: [The Well-Grounded Rubyist, by David A. Black.](https://www.amazon.com/Well-Grounded-Rubyist-David-Black/dp/1617291692)
- Reading: [Full Stack React.](https://www.fullstackreact.com/)
- Watching: [A Cloud Guru AWS Software Architect Online Course.](https://acloud.guru/learn/aws-certified-solutions-architect-associate)
- Went to: [Women Who Code, Her 2.0 - Capable. Confident. Courageous.](https://www.meetup.com/Women-Who-Code-Manila/events/248092880/)
- Wrote: A blog post on how I use the Pomodoro technique.
- Writing: An article on journaling.
- Biked: 278 (!) km.
- Coding:
  - Back-end/Ruby/Rails: I as able to deploy Transcripto via AWS. While I've done this before, this is the first time I used `webpacker` to manage the front-end assets. Webpacker ended up causing most of the delay, as I need to upgrade, then add a step in Capistrano to install `npm`.
  - I provisioned 2 instances because I felt like there was a problem with my `npm` installation in the first one. Because I have a lot of projects in my head, this is where I'm feeling the pain of creating these dev boxes. I'm now choosing between Chef and Ansible: the book I have, [Reliably Deploying Rails Applications](https://leanpub.com/deploying_rails_applications), has examples in Chef, but my homies use Ansible. In the end, those are probably just DSLs, so learning one would make it easier for me to learn the other.
  - Other language/Elixir/Phoenix: Wasn't really able to do much, as I was busy during the weekend, but I was able to read up on [Ecto](https://github.com/elixir-ecto/ecto). I'd say I'm struggling a bit because my mind is always in Railsland, and so I end up trying to do things like `User.first` in the Elixir command-line.
  - Front-end/ReactJS: Not that much in coding, but I learned a lot about the theory of React. Still at the router part of Full Stack React. I also browsed the philosophy of Redux, and I like what I'm seeing. I'm still getting over the fear of JS and my PTSD of callback hell and Angular 1 documentation!
  - Database normalization, had a deeper understanding of Redis and its data types, and I used Ruby's performance tools, `ruby-prof` and `flamegraph` to cut down Pomodoro display time. It's still a work in progress.

---

## Women Who Code/Future Transcription Person, Lol.

Last Saturday, I went to Women Who Code: Her 2.0 to transcribe the learnings from the event. It was the first time I went to a tech event where women severely outnumbered men (there were probably <10 guys and 100++ ladies).

While I can never be a woman in tech (though who knows? Lol), that experience made me relate more to some of the struggles that they might face. I felt like an outsider, even though there should be no reason for me to do so. We're all programmers, anyway. That's what I kept telling myself, but I can't help feeling a little bit uncomfortable being in the minority.

Is this what a lady programmer feels like when she's surrounded by men, or is this what a black guy would feel if he was the only black guy in the company? Possibly. It's hard to explain because it's something that you feel, not just something you read about. While I've read a few articles on diversity, being in an actual minority position, even for a few hours, was more impactful.

I have to ship this weekly recap, but the people I met in that event were so cool. I'm still working on the transcripts for the event, but thank you Joy, Mich, and Women Who Code!

---

## Tidbits:

- I started a new bike workout plan last week. On Tuesday, [I took a functional threshold power (FTP) test](https://support.trainerroad.com/hc/en-us/articles/201993760-FTP-Testing-The-Cornerstone-of-Training). While my power definitely increased (thanks training), the test results weren't honest. When you're trying to get your FTP, you want a steady effort for the allotted time. I was looking to [negative split](https://en.wikipedia.org/wiki/Negative_split) it, so I tried not going as hard for the first 10 minutes, then going all out on the last 5. That was bad, as I got a heavily skewed result (higher than the number I'm supposed to be at). It was only good for my ego, not for my performance gains.
- I paid for that effort with my Thursday result. I couldn't even finish the first interval because my legs were screaming in pain. In interval training, you shouldn't be bonking on the first set! This was very much a sign of a miscalibrated FTP. After lowering my power to a more reasonable number, I was able to get on with the workout. I still imploded on the later intervals, but that's fine. I'll be continuing the training this week, let's see if I'm still at too high of a power level.
- On deployment: The difference between ops and programming is the feedback loop I think. When something goes wrong in ops, like my deployment, it's sometimes hard to diagnose because you have to wait for the deployment process to finish. This is where deep learning and problem solving skills really come into play. Just to give an idea, what I did to solve deployment issues were:
  - Upgrading `webpacker`.
  - Adding `capistrano-npm`.
  - Changing an `nginx` config file.
- I will be very honest-there is a bit anxiety brewing over me right now. By leaving Sourcepad, I left a ton of money on the table. I've learned a lot in these few months about myself and about the world but I would be lying if I said that I don't completely regret the decision to leave. There's no real point in pondering over the decision anyway, since it's done, but yeah. It's true.
