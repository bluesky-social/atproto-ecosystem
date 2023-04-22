# App Password

To allow users to start logging in with app passwords, you won't need to change
a thing! Users will be able to log into your client with an "app password" in
the exact same way that they log in with their account password.

App passwords have most of the same abilities as the user's account password,
however they're restricted from destructive actions such as account deletion or
account migration. They are also restricted from creating additional app
passwords.

No client changes are required to adopt app passwords. However, we strongly
encourage you to prompt users to use an app password on login and avoid ever
entering their password. For account creation, we encourage redirecting a user
to the bluesky client (https://staging.bsky.app)

You should also delete all existing refresh tokens and re-fetch access/refresh
tokens using an app password.

App passwords are of the form xxxx-xxxx-xxxx-xxxx. For your users' safety, you
could run a quick check to ensure that they are logging in with an app password
and not their account password.
