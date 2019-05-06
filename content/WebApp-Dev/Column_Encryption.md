# Column Encryption

Column-level encryption is used to deny unauthorized users and users
with access to the underlying database visibility to information of a
sensitive nature.

## Terminology

  - FIPS 197 Compliance – Federal Information Processing Standard 197 is
    a US Government standard that provides best practices for
    implementing crypto algorithms, handling key material and data
    buffers, and working with the operating system.
  - Decrypt/Pass – When reading data from an encrypted column, the
    decrypt mechanism is designed to look at the data, find the magic
    marker and attempt to decrypt the data. If the magic marker does not
    exist, there is no attempt to decrypt the data and the data is
    preserved as is.

When encrypting a column:

  - All encryption and decryption is performed at the application level.
    Data entered into the database outside of the DSP®-specific
    mechanism will be seen as plain text because this is
    application-level encryption and decryption.
  - Triple DES or AES-256 is used.
  - Encryption Keys are stored in the database. Each instance of DSP®
    can have one or more encryption keys that can be used to encrypt one
    or more columns.
  - Proprietary keys are protected by a Site Master Password (which is
    system-generated if one is not specified) that must be identical
    across all servers for a specific instance. The Site Master Password
    is stored in web.config. The system-generated Site Master Password
    is based on the server name and the database; therefore, all host
    files or DNS aliases must be in place and identical across machines.
  - Users only need rights to view the page to view the encrypted data.
  - Encryption is available to developers through the plugin API with
    encrypt and decrypt/pass. To use API, the KeyID must be known
    (located in the Key table, GUID).
  - Encrypted columns must be nullable and be configured with data type
    nvarchar. The size of the column must be between 128 and 256.
  - WebApps with encrypted data must be decrypted before a CTS package
    is built. Move the package, then re-encrypt.
  - Database-level mechanisms cannot be used to read or write encrypted
    data. These operations must be performed by plugins or through the
    DSP® front end.
  - Joins, search or indexing are not supported on encrypted columns.
  - Once data is encrypted with a specific key, the key cannot be
    deleted until the data is decrypted.

This section contains the following topics:

  - [Encrypt a Column](Encrypt_a_Column.htm)
  - [Decrypt Data](Decrypt%20Data.htm)
