# tbhong

The home for the source of [tbh.ong](https://tbh.ong)

## Development instructions

Set up the DB with docker by running the following commands in the root of the project. Make sure you have docker installed.

```bash
docker compose up -d
```

then, update the `DATABASE_URL` environment variable in `.env` and then run the following:

```bash
yarn prisma db push
```

now your DB is in sync with your prisma schema and you are ready for development.

Run the following command to start the Next server.

```bash
yarn dev
```

### Environment variables

Learn more about how environment variables are setup and used [here](https://create.t3.gg/en/usage/env-variables).
