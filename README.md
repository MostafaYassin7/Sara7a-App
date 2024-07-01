# Sarahah Clone

This project is a clone of the Sarahah website, developed as a backend service. It allows users to create accounts, validate their email with an OTP, sign in with JWT authentication and authorization, handle errors, validate inputs, retrieve messages, and share profile links.

## Features

- **User Registration and Authentication**
  - Create an account with email validation using OTP
  - Sign in with JWT-based authentication and authorization

- **Message Handling**
  - Retrieve all messages for a user
  - Send anonymous messages to a user
  - Delete specific messages

- **Error Handling and Validation**
  - Comprehensive error handling and validation using Joi schema

## Endpoints

### Authentication

- **Sign Up**
  - `POST /auth/signup`
  - Registers a new user and sends an OTP for email validation.

- **Sign In**
  - `POST /auth/signin`
  - Authenticates a user and returns a JWT token.

- **Verify Email**
  - `PUT /verify/:otp`
  - Verifies a user's email using the provided OTP.

### Messages

- **Retrieve Messages**
  - `GET /messages`
  - Retrieves all messages for the authenticated user.

- **Send Message**
  - `POST /messages/:id`
  - Sends an anonymous message to the user with the specified ID.

- **Delete Message**
  - `DELETE /messages/:id`
  - Deletes a specific message by its ID.
