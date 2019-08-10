## Bible Mailer

I host an instance of this at [bible.kaiserapps.com](https://bible.kaiserapps.com), feel free to go and register for notifications there.

However if you are the super-privacy kind or would just like to run it yourself, follow the below developer instructions.

### Developer Instructions

This application is built with deployment to dokku / heroku in mind. For those you will need to set the following environment variables:

#### Environment variables

```
SMTP_URL=smtps://user%40gmail.com:pass@smtp.gmail.com
SENDER_EMAIL=user@gmail.com
```

If you would like to use the direct mail transport, then there is no need to set `SMTP_URL`.

#### Running in Docker + Docker Compose

```
bin/go
```

And you're done! Good to go! try it out on http://localhost:3000

#### Without Docker

You'll need:
- Node.js 8
- Mongodb running

then execute

```
yarn
APP_URL=http://localhost:3000 npm start
```
