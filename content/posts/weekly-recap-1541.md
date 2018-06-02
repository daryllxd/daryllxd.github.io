---
title: "Weekly Recap, 1541, Technical Exam, Event Sourcing"
date: 2018-05-25T03:13:40+08:00
tags: ["weekly-recap"]
---

- Reading: [When Coffee and Kale Compete.](http://www.whencoffeeandkalecompete.com/)
- Reading: A bunch of stuff about event sourcing.
- Watched: [Take a Step Backwards to Take a Step Forward for the Rest of Your Life.](https://www.youtube.com/watch?v=WkJtsjv9ICc)
- Coding: Technical exam.
  - [Sagas pattern.]((https://www.youtube.com/watch?v=xDuwrtwYHu8)
  - [RailsConf 2017 Panel: Performance, Performance](https://www.youtube.com/watch?v=SMxlblLe_Io)

---

# Technical Exam at "TG Company"

So I'm taking a technical exam right now. I'm still trying to figure the right approach to the problem at hand, but I'm honestly a bit happy about my progress. It's hard to explain, but in software development and programming, you always have to take several factors into consideration. There's the speed of the program, the size in memory, and the time it takes for you to code a solution.

Let's say we have to present an NBA box score to the users. How do we store the game data? We can choose to store the states of a game, or the changes in states of a game. Each of those is different, because if we choose to store the states, then it would be faster to query game state because you just look for the nearest timestamp, but because you have the entire game state in memory, it would take up more hard drive space. Contrast that to storing the events, then you'd have less space in memory, but in order for you to regenerate a game state, you'd have to replay all the events.

This isn't even taking into consideration the developer's time in creating a system and orchestrating the thing. Not to sound too presumptuous but there really is a lot of different things you have to think about when creating a system. Sometimes, this can lead to analysis paralysis, but for me the solution is to just give myself a time limit to make a decision and follow on through. I also have to consider if it is actually possible to take a step back and undo the decision just in case it wasn't the smartest one. Anyway. I still have to crystallize these thoughts, but this is like in the weed territory of programming and systems design. And I believe that to become a decent and competent and possibly even great programmer, you have to love these types of conversations.

Anyway. Still working on my solution. I have a prototype up now, but I'm still figuring out what the use cases for the client are.

---

# Musings

- I haven't been cycling as much as I should have. That's okay, but I should get back to it. I'm trying to just get 1 hour a day, 30 minutes if there really isn't time. But honestly for me I think when someone says "not enough time", I think they have to qualify it first. Don't say there's not enough time and browse social media and watch Youtube videos instead. Just say that "I don't want to do it because I'm not in the mood" or something else. Yeah, that includes me. Have to get better!
- I've watched ["Take a Step Backwards to Take a Step Forward for the Rest of Your Life."](https://www.youtube.com/watch?v=WkJtsjv9ICc) 5 times already, especially the part near the end. This part really resonated with me because I've lived through that. I took a "step backwards" (going out of UP and looking for a job) to figure out the value of money and what my purpose in life is. Fortunately, it worked: I'm a successful programmer now. Right now, I'm also in the "step backwards", as I quit my job last November to figure out my next steps. I hope I take a big step forward if I pass my interviews.
- One of my friends, M, is buying a motorcycle, and that's awesome. It's hard to explain the high that I get from two-wheeled vehicles. I feel like it's just so human. You can feel the wind in your face and the undulations of the road. I'm just really fearful of the road nowadays. I'm very careful when it comes to cycling, and that's precisely the problem: even if you are super-careful and do everything right, it's still possible for you to die. There's no protective covering that a car affords you. For me, it's just something that I risk every time I go outside and ride my bike. Sometimes I ask myself why I do this when I can so easily die. Oh well.
