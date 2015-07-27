# This is a web app to chart your relationship with a person by analysing your emails or text messages.

It was made using Ruby on Rails, Backbone, and the APIs for sentiment.vivekn.com, Google Sign In, and Gmail.
B64.js was used for converting uint8 encoded messages to base64 arrays.
LeanModal.js was used to aid the creation of the login modals.
jQuery.flot.js was used as a lightweight graph tool with non-discrete time interval graphing.


## Uploading:

### Selecting upload via gmail:
 - Automatically syncs 50 of your most recent emails and hangout chats.
 - Generates contact models for these 50 emails, and strips the text from them.
 - The sentiment api returns a JSON object of emotional scores.
 - The scores are saved to the database, and returned in graph form.

### Selecting upload via text:
 - Back up your texts with any number of companion apps.
 - The same process as above occurs, but the contacts are now listed with TXT appended to their name.

No personal data or message content is ever stored in our database, and no user contact data is displayed to the end user other than the one signed-in. All data is stored as completely anonymous numbers of ranging from positive to negative, with a confidence value in that result.
