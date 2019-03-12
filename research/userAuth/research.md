# User Authentication

While searching around for User Auth options for NodeJS, something called Passport came up a lot.

Browsing through the documentation, it looks easy enough to use. It also has options to authenticate
with Google, Facebook, etc if we would like to add that later.
Documentation on how to install and use can be found here: http://www.passportjs.org/docs/

In addition, Robert suggested we use a seprate library for hashing called pbkdf2.
You can find it and info on it here: https://www.npmjs.com/package/pbkdf2
and here: https://en.wikipedia.org/wiki/PBKDF2

Those combined should work for our purposes, but if we run into problems with it for some reason,
this could be a good fallback, assuming it isn't too complicated: https://firebase.google.com/docs/auth/