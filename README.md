# Node Starter

> A Node server boilerplate.

A good starting point for a Node server. It uses Redis for cache management and Postgres as relational database — both easily removable and interchanged.

Folder structure tries to follow the [SOLID](https://khalilstemmler.com/articles/solid-principles/solid-typescript/) principles.

[**PLEASE READ THE WIKI**](https://github.com/angelod1as/node_starter/wiki).

There's a lot of information there.

# Running/Installing

First, you have to create two docker containers, one running Redis and other Postgres.

```
docker run --name postgres -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
docker run --name redis -p 6379:6379 -d -t redis:alpine
```

Run `yarn` then:

### Scripts

- `build`: parses typescript into `dist` folder
- `dev:server`: development server
- `start`: runs server
- `test`: runs `jest` tests
- `typeorm`: runs `typeorm` commands, like creating and running migrations

## Contributing

1. Fork it (<https://github.com/yourname/yourproject/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

[wiki]: https://github.com/angelod1as/node_starter/wiki

# About this readme and the wiki

I've written A LOT of information for personal usage, as a huge folder structure and explanation of what *each* package does. So, [**PLEASE READ THE WIKI**](https://github.com/angelod1as/node_starter/wiki).

It took me about 9 hours to finish this project.

This code is based on [Rocketseat](https://rocketseat.com.br/) bootcamp.
