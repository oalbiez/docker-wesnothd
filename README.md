# wesnothd-docker
Battle for Wesnoth game server


## Building

    docker build -t wesnoth .


## Running

    docker run -p 15000:15000 -e PASSWD=admin wesnoth


Environments variables are:

- PASSWD: the admin password
- MOTD: the message of the day (default to Welcome to this game server)
- REPLAYS: true or false, defines whether the server will automatically save replays of games (default to true)
- THREADS: sets the maximum number of worker threads that will be created (default to 5)

