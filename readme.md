# Deebees
Dockerized version of your favorite databases. A shell command is also added to easily start `deebee` anywhere much like `docker` or `docker-compose`. You just need to add it in your path. See the **commands** section for more details on what you can do.

## Who is this for?
TBH, I dunno, seriously, just use [Tighten's Takeout](https://github.com/tighten/takeout), its more powerful and maintained by one of the best companies around Laravel. But if you only want a quick way to install databases then this is for you!

## Supported
- MySQL (5.7 and 8)
- Redis
- Memcached
- MariaDB (Planned)

## Requirements
- Docker
- Docker Compose

## Setup
- Clone this repo or download it and extract it
- `cd` into it and run `docker-compose up -d` as detached or `docker-composer up`
- Use the companion shell command to run the it anywhere by putting `/path/to/deebee` command in your path like so:
```
export DEEBEEPATH=/Volumes/Devferoxide/Workspace/docker/deebee
export PATH=$PATH:$DEEBEEPATH
```

### Commands
The `deebee` command is a proxy to the `docker-compose` command except for few commands like: 
- `deebee mysql57` will connect you to the MySQL 5.7 version database
- `deebee mysql58` will connect you to the MySQL 8.0 version database


#### Notes
This project is heavily inspired from [Tighten's Takeout](https://github.com/tighten/takeout) and [Laravel Sail](https://github.com/laravel/sail). Go check this projects out!
