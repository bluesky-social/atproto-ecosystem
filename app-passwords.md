# App Password

To allow users to start logging in with app passwords, you won't need to change
a thing! Users will be able to log into your client with an "app password" in
the exact same way that they log in with their account password.

App passwords have most of the same abilities as the user's account password,
however they're restricted from destructive actions such as account deletion or
account migration. They are also restricted from creating additional app
passwords.

No client changes are required to adopt app passwords. However, we strongly
encourage you to prompt users to use an app password on login and **avoid ever
entering their password**. For account creation, we encourage **redirecting a user
to the bluesky client** (https://staging.bsky.app)

We also strong encourage you to **delete all existing refresh tokens** and 
re-fetch access/refresh tokens using an app password.

App passwords are of the form `xxxx-xxxx-xxxx-xxxx`. For your users' safety, you
could run a quick check to ensure that they are logging in with an app password
and not their account password.

Some images of the flow:
![image](https://user-images.githubusercontent.com/1243164/233754422-55d600b1-b59c-41ee-a44b-898bc06f65f1.png)
![image](https://user-images.githubusercontent.com/1243164/233754430-9a5efe91-a0fd-448a-9263-0e29b6ccc5a9.png)
![image](https://user-images.githubusercontent.com/1243164/233754396-e708bb24-bdd5-46aa-b798-e67b52593275.png)
![image](https://user-images.githubusercontent.com/1243164/233754403-98e8ecce-d8a1-4e98-9b5f-7e442286deb6.png)
![image](https://user-images.githubusercontent.com/1243164/233754409-a234442c-4a93-40f0-af3e-836eaa2777af.png)
