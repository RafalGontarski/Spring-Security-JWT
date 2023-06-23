# Authentication, Authorization and Refreshing of Tokens from JWT for Administrator and Manager

Our authentication and authorization system based on JSON Web Token (JWT) provides secure and effective access management for various user roles, such as Administrator and Manager. Thanks to the additional token refresh mechanism, we can ensure secure user sessions for a longer period of time, without the need for frequent logins.

Functions:
1. **Authentication**: A secure login process that generates a unique JWT and refresh token for each logged-in user.
2. **Authorization**: Using a user role stored in the JWT to grant or deny access to specific resources.
3. **Token Refresh**: Secure token refresh mechanism to keep sessions active for longer periods of time.
4. **Admin Role**: Full access to all system resources and functions.
5. **Manager Role**: Limited access to selected resources and functions, in accordance with the given permissions.
6. **Security**: All tokens are securely stored and transmitted, ensuring user privacy is protected.

## How it's working?

1. The user logs into the system using his username and password.
2. After successful authentication, the system generates a JWT and a refresh token. The JWT contains a unique user ID and his role (Administrator or Manager).
3. Tokens are returned to the user. The JWT should be sent as the 'Authorization' header in every request to the server. The refresh token should be stored securely and only used to refresh the JWT.
4. When the JWT expires, the user can apply to the relevant endpoint with the refresh token to receive a new JWT.
5. The server verifies the token on each request and uses the information contained in the token to authorize the user to perform the requested action.

Remember to always treat your JWTs and refresh tokens as sensitive data and never share them. Tokens should be stored securely and only transferred over secure connections.

![image](https://github.com/RafalGontarski/Spring-Security-JWT/assets/106514250/aa22e3f7-e677-4fa3-96c0-29e840965b9f)

# Technologies
![image](https://github.com/RafalGontarski/Spring-Security-JWT/assets/106514250/b151b382-caed-4e6b-8f32-37ce5a7631e2)


#### Special Thanks to Amigoscode for many tutorials.
