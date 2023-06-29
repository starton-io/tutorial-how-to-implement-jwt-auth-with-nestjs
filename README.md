## Description

This project is an example of how to create a JWT-based authentication system with NestJS.

## Installation

```bash
$ yarn install
```

### Setting your .env fie

You need to create a `.env` file in the root of your project and add the following variables:

```
DATABASE_URL="DATABASE_CONNECTION_URL"
JWT_SECRET=your_secret_here

```

`DATABASE_URL` specifies the connection URL to connect to the database, and `JWT_SECRET` is the secret used to sign the JWTs. You can generate a strong secret by running the following command in your terminal:

```bash
node -e "console.log(require('crypto').randomBytes(256).toString('base64'));"
```

Once you have generated a strong secret, add it to your `.env` file as `JWT_SECRET`.

## Running the app

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev

# production mode
$ yarn run start:prod
```

## Usage

1. Start the server: `npm start` or `yarn start`
2. Use a REST client like Postman or Insomnia to send requests to the server:
   - Send a `POST` request to `/user/auth/sign-up` with the following JSON payload:
     ```
     {
       "email": "johndoe@example.com",
       "password": "P@ssw0rd"
     }

     ```
   - Send a `POST` request to `/user/auth/sign-in` with the same JSON payload
   - Send a `GET` request to `/user` to get the user data (requires authentication)
   - Send a `POST` request to `/user/auth/revoke-token` to revoke the JWT token (requires authentication)

## Test

```bash
# unit tests
$ yarn run test

# e2e tests
$ yarn run test:e2e

# test coverage
$ yarn run test:cov
```

## Support

At Starton, our goal is to provide you with excellent support. If you have any concerns or questions regarding this project or any other project, please reach out to us for assistance. Our team of experts is available to help you with any questions or issues you may encounter. We're committed to providing timely and effective support to ensure your success with our products and services.

To contact us, send an email to [support@starton.com](mailto:hello@starton.com) to submit a support request. We'll respond to your inquiry as soon as possible.

Thank you for choosing Starton as your trusted partner for your software development needs.

## Stay in touch

- Author - [Alexandre Schaffner](https://github.com/delicious-mango)
- Website - [Starton](https://starton.com/)
- Twitter - [@starton_com](https://twitter.com/starton_com)

## License

Nest is [MIT licensed](LICENSE).
