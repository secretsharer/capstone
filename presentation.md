# Capstone Presentation
The capstone presentation highlights your application as the culmination of your work at Ada.
It should be __no more than 5 minutes__ in length and should have the following components:

Ubot

For my capstone, I wanted to try and build a chat-bot that would allow you to chat with "yourself". I began with how I might create one to talk like me.  Assuming someone had already attempted something like this and I began my research. Sure enough someone had. I studied Hendrik J. Weideman's project in which he trained his computer on his own facebook chats, https://hjweide.githubio/char-rnn, but in the end I went with an existing code repository by Laura Gelston utilizing an implementation of Char-rnn, a LTSM recurrent neural network, in this case built on TensorFlow and packaged as an Python/Flask API that produces text samples. My fancy plan was to "understand" everything about her repo, of course, feed it a google data archive of my sent gmail messages, train it, and presto, magically have a genius chat-bot. 

In my mind, this perfectly feasable plan broke down into 3 parts:

Front-end: Ideally this would be a real-time chat app, utilizing socketing instead of ajax requests both directions
Server: I was content to let this part remain a mystery until into the build.
Back-end: Deep Learning model set up as an API

I spent a great deal of time reading and researching in preparation and early on a few things became clear:
I needed some kind of text samples to test the front end while until I could figure out how to get the repo training and producing a model on my little cpu. So, I built the front in socket.io and node, then built the a Ruby/Rails speech emulator API provide those samples, and ubot was born.
After many days of building python libraries and different vens to run the SpeakEasy deep learning repo and continuously running into depreciation issues that I'm simply too green to solve, my illustrious project manager encouraged me to keep building that out and see what kind of quality I could get, while he helped me get the training model to run on the cloud. Which I did.

What I learned:

Just frustrating python venvs and library dependencies can be.
How to trace the same errors for days at a time without fliping a table.
Just how important good documentation is.
Having a team to work with is pretty much the best.

On that note - Charles did get that model to train after all, and we connect my app to its API, so now we get to play a short game of "Who said it - Ubot or YouMachine?"

Thanks you.





