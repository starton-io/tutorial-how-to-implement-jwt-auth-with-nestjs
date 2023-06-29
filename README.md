![Starton Banner](https://github.com/starton-io/.github/blob/master/github-banner.jpg?raw=true)

# Tutorial - How to implement JWT authentication with NestJS

## Requirements

You will need :
- [NodeJS](https://nodejs.org/en) (we recommend the use of [nvm](https://github.com/nvm-sh/nvm))
- [NestJS CLI](https://nestjs.com/)
- [NestJS JWT module](https://github.com/nestjs/jwt)
- [Prisma client](https://www.prisma.io/)
- [class-validator](https://www.npmjs.com/package/class-validator)
- [class-transformer](https://www.npmjs.com/package/class-transformer)
- [uuid](https://www.npmjs.com/package/uuid)
- [cookie-parser](https://www.npmjs.com/package/cookie-parser)

## Installation

To install the project, first clone the repository and go inside project directory, then :

- With [yarn](https://yarnpkg.com/) :
    ```bash
    $ yarn install
    ```

- With [NPM](https://www.npmjs.com/) :
    ```bash
    $ npm install
    ```

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file.

* `NODE_ENV` : is a system environment variable that Node exposes into running scripts
* `DATABASE_URL` : is an environment variable that Prisma uses to connect to your database.
* `JWT_SECRET` : A random string used to sign JWTs

## Run Locally

Your project is now ready to be modified by you, for that you just have to launch the project via the command below:

- With [yarn](https://yarnpkg.com/) :
    ```bash
    $ yarn start:dev
    ```

- With [NPM](https://www.npmjs.com/) :
    ```bash
    $ npm run start:dev
    ```

## Deployment

You can deploy this service on hosting platform like Heroku.

## Documentation

Find out more on how to use Starton in our [Documentation](https://docs.starton.com/)

## Contributing

Contributions are always welcome!

See [CONTRIBUTING.md](./CONTRIBUTING.md) for ways to get started.

Please adhere to Starton's [Code of Conduct](./CODE_OF_CONDUCT.md).

## License

[Apache License 2.0](./LICENSE.md)

## Authors

- Starton [support@starton.com](mailto:support@starton.com)
- Alexandre Schaffner
