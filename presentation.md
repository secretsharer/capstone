Ubot Vs. You-Machine:

**Clothes: HTML/CSS  
Skin & Bones: Javascript, JQuery  
CNS: Socket.io, NodeJS  
Heart: Ruby/Rails  
Brain: Python, SciPy, TensorFlow, Flask**  

For my capstone, I wanted to try and build a chat-bot that would allow you to chat with "yourself" by training it with your own sent emails or facebook chats. So, as a study, I began with how I might create one to talk like me.  Assuming someone had already attempted something like this, I began my research. Sure enough I found and scoured Hendrik J. Weideman's project in which he trained an implementation of what's called Char-rnn, a LTSM recurrent neural network on his own facebook chats, https://hjweide.githubio/char-rnn. Char-rnn is responsible for such gems as: [Slide of paint-chips]. After study, I knew something more complete would be required for someone of my skill level, so I kept looking and found a repository called SpeakEasy, by Laura Gelston, https://github.com/gelsto/SpeakEasy-AI, which utilizes an implementation of Char-rnn built on Google's TensorFlow and is packaged as an Python/Flask API that produces text samples. My fancy plan was to "understand" everything about her repo, of course, feed it a google data archive of my sent gmail messages, train it, and presto, magically have one side of an awesome chat-bot. 

In my mind, this perfectly feasable plan broke down into 2 parts:

Front-end: Ideally this would be a real-time chat app, utilizing socketing instead of ajax requests both directions
Back-end: Deep Learning model set up as an API

That meant I would need text samples to test the front-end until I could figure out how to get the repo training and producing a model on my little cpu for the back-end. So, after building the chat portion of the app, I started on speech emulator to generate those samples. I'd say, at this point, ubot was born.

After days of drafting python libraries and different venvs to run the SpeakEasy deep learning repo and continuously running into depreciation issues that I'm simply too green to solve, my illustrious project manager encouraged me to keep building out the rails speech emulator and see what kind of quality I could get, while he helped me get the training model to run on the cloud. Which, as I did, I became increasingly pleased with the results of the emulator, and bonus: got to drive my classmates crazy by giving ubot a generic british accent and asking them to test the chat-app.

What I learned:

Just frustrating python venvs and library dependencies can be.
Just how important good documentation is.
How much Ada taught me about not only programming but trusting my instincts and abilities.
And a reminder that, having a good team to work with is pretty much the best.

On that note - Charles did get the model to train after all, which I'm very grateful for. It can take a long time to train a neural network on a data set and get any recognizable results, but, we connected Ubot to both the emulator and youmachine's API at it's current progress, so now we can play a short game of "Who said it - Ubot or YouMachine?"


Thank you.
Volunteers?




