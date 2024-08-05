# GoAuth

This is a microservice that handles Authentication and Authorization for my Postgres Database hosted in a Heztner Machine with Coolify.

It'll implement both endpoints:

    · Login -> Checks the creds and returns a JWT token to authenticate the user.
    · Auth -> This endpoint will receive a Token, check if it is valid.

eg: My API for accesing information developed in NodeJS with Typescript will add a middleware for those routes that MUST BE PROTECTED, and this middleware with call the GoAuth service to check for credentials before executing the operation.

## Reasoning behind this microservice

1. Centralizing logic and not repeating myself (DRY), following this principle allows me to focus on side-project development without thinking too much about Authentication/Authorization in the future.
2. Learning Golang, this language seems really nice, and i love learning and in the end this is an excuse to continue learning and leveling up as a developer.

## Tecnologies

1. Golang -> The main back-end language
2. Go std library -> This is the standard library for handling HTTP requests, there are multiple third party libraries that increase the DX of API development but i really want to learn the language and i want to implement this myself (probably goes wrong).
3. Postgres -> Main DB, we have both local db spun up with Docker, and a cloud one which is private and you'll have no access to.

## Environments

### Additional tools used

I came upon MelkeyDev, Twitch Streamer who also works for Twitch, he does Golang content and he was a really good source of knowledge to start a project.

Melkey has a open-source tool which is a CLI tool, this tool scaffolds your project with the selected frameworks and templates to set you up for success.

You can find this tool here: <https://go-blueprint.dev/>

> Make sure to check the repo in github and install process and give the man a star, he really is the heart of Golang content creation and really helps the community.

### Why open-source?

I'm making this project open for everybody so anyone can download it, plug it into their own DB and use it in a fast and reusable way, i love helping the community and if anyone comes upon this repo and wants to use it, you are free to do so.

I will try to make all the code clear and heavily documented so you can easily and quickly spun it up to suit your needs.
