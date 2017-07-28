Ubot/YouMachine:

**Clothes: HTML/CSS  
Skin & Bones: Socket.io, Javascript, JQuery  
CNS: NodeJS  
Heart: Ruby/Rails  
Brain: Python, SciPy, TensorFlow, Flask**  

For my capstone, I wanted to try and build a chat-bot that would allow you to chat with "yourself". So, I began with how I might create one to talk like me.  Assuming someone had already attempted something like this, I began my research. Sure enough I found and studied Hendrik J. Weideman's project in which he trained an implementation of what's called Char-rnn, a LTSM recurrent neural network on his own facebook chats, https://hjweide.githubio/char-rnn. Char-rnn is responsible for such gems as: [Slide of paint-chips]. However, after studying, I realized something more complete would be required for someone of my skill level, so I kept looking and found and existing code repository by Laura Gelston called SpeakEasy, utilizing an implementation of Char-rnn, built on Google's TensorFlow and packaged as an Python/Flask API that produces text samples. My fancy plan was to "understand" everything about her repo, of course, feed it a google data archive of my sent gmail messages, train it, and presto, magically have an awesome chat-bot. 

In my mind, this perfectly feasable plan broke down into 2 parts:

Front-end: Ideally this would be a real-time chat app, utilizing socketing instead of ajax requests both directions
Back-end: Deep Learning model set up as an API

After much reading in preparation and early on a few things became clear:
I would need text samples to test the front-end as I built....until I could figure out how to get the repo training and producing a model on my little cpu. So, I built the chat portion of the app with socket.io and node, and then built a speech emulator as Ruby/Rails API to generate those samples. At this point, ubot was born.

After days of drafting python libraries and different venvs to run the SpeakEasy deep learning repo and continuously running into depreciation issues that I'm simply too green to solve, my illustrious project manager encouraged me to keep building out the rails speech emulator and see what kind of quality I could get, while he helped me get the training model to run on the cloud. Which, as I did, I became increasingly pleased with the results, and bonus: got to drive my classmates crazy by giving ubot a generic british accent and asking them to test the chat-app.

What I learned:

Just frustrating python venvs and library dependencies can be.
How to trace the same errors for days at a time without fliping a table.
Just how important good documentation is.
How much Ada taught me about not only programming but trusting my instincts and abilities.
Having a team to work with is pretty much the best.

On that note - Charles did get the model to train after all, which I'm very grateful for. I connected Ubot to youmachine's API, so now we can play a short game of "Who said it - Ubot or YouMachine?"

Thank you.
Volunteers?




