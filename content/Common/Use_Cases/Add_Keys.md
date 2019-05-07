+++
title = 'Add Keys'
solution = 'Platform'
+++

# Add Keys

A secure key defines the encryption algorithm and password used to
encrypt and decrypt legacy data. As many keys can be defined and reused
as necessary for the needs of the project. For example, a single key can
be shared by a Migration Team to encrypt all the data for an object or a
single key can be defined and used on only one column by one team
member.

Team members that export and load data into the target system do not
need to know the password in order to encrypt the data. The password can
be set up by one person who is administrating the data. The password in
the table must be encrypted by using the DSP® encryption processes in
data sources. The decrypt process runs automatically with only the
person who set up the process knowing the password.

To add keys:

  - [Encrypt CranSoft Data Source
    Password](Encrypt_CranSoft_Data_Source_Password.htm)

  - [Create a Secure Key](Create_a_Secure_Key.htm)
    
    Additionally, information is provided about [Forgotten/Incorrect
    Encryption
    Password.](Forgotten_Incorrect_Encryption%20Passwords.htm)
