- what is hubot?
  - gif summoner
  - annoying POS
  - Awesome CI helper
  - chat bot with a DSL built on top of node.js server
- node.js 
  - Node.js® is a platform built on Chrome's JavaScript runtime for easily building fast, scalable network applications. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient, perfect for data-intensive real-time applications that run across distributed devices.
  - chat is data-intensive, real-time, and distributed :)

- coffeescript
  - it's just javascript
  - watch out for indentation!
  - You don't have to use it

- hubot scripts
  - DSL
    - respond vs hear
    - regular expressions
    - msg.send
    - globbing with msg.match for parameters
    - built in random
    - leverage npm dependencies

- How does it work?
  - for each chat message, check against all regular expressions
  - fire all matches
    - .img that

- local setup
  - Use homebrew!
    `brew install node redis heroku-toolbelt` (this also includes npm)
    `git clone git@github.com:detroit-labs/hubot-badger.git`
    `npm install`
    `bin/hubot`
  - environment variables
    - use these to store API keys, passwords

- adapters
  - Shell is just another adapter
  - On heroku, the hipchat adapter is used
- redis
  - Key/Value persistence
  - No relational schemas
  - you can store whatever you want, but you have to use your own keys
    - I've had success with a prefix and the room name (msg.envelope.room)
- deploying
  - keep alive

- questions?
