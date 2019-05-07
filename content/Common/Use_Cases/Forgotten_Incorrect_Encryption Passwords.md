+++
title = ''
solution = 'Platform'
+++

# Forgotten/Incorrect Encryption Password

If the encryption password is forgotten or is incorrect, it cannot be
modified. Conduct the following steps if the password is forgotten:

1.  Create a new secure key.
2.  Re-apply the key to the source data.
3.  Refresh the source data in Common to encrypt the legacy data with
    the new secure key.
4.  Delete the existing key.

The new key does not take effect until the source data download process
is run.
