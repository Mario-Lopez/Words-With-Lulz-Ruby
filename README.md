Words with Lulz
===============

Running the Server
==================
From the `server` directory, run:

`foreman start`

Server API
==========

Create Game
-------------
POST: wwwl/game/$game

`curl -X POST -H "Content-Type: application/json" -d '{"players":["mario","matt"]}' localhost:4444/wwl/game/first_game`

Get Game Data
-----------
GET: wwwl/game/$game/player/$player

`curl -X GET localhost:4444/wwl/game/first_game/player/mario`

Output:
```
"{\"game\":[[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"],[\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \",\" \"]],\"letters\":[\"T\",\"T\",\"T\",\"T\",\"T\",\"T\",\"T\"]}"
```

Make Player Move
----------------
TBD