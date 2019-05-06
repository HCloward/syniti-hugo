# Field X is not an input field.

This message is confusing because the field is an input field. A
possible cause of this error is that the user recorded the transaction
and made a mistake in the recording but did not realize the mistake was
made until they had entered data in other fields. They received the
error, then went back and corrected the data. This is not a good
practice for recording because when the data is posted, it posted
correctly, then SAP will try to go back into the field to correct the
data and it will no longer be an input field.
