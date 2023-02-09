# IAM Access Keys
![IAM Access Keys](images/access-keys.png)

## Access Keys
Access keys are how the AWS Command Line Tools (CLI Tools) interact with AWS accounts.

* Long-Term Credentials that are assigned to an IAM User.
    * Don't change automatically or regularly
* Username and Passwords are used for console access (GUI).
* Access Keys are used for AWS Command Line Tools (CLI).
* IAM User can have up to `two access keys`
* Access keys can be `created`, `deleted`, made `inactive` and made `active`

## Formation
AWS provides both access key id and secret access key. Secret Access Key is only displayed once. Store it safely and securely.

Example:
1. Access Key ID: AKIAIOSFODNN7EXAMPLE `(Acts like a username)`
2. Secret Access Key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY `(Acts like a password)`

## Rotating Keys
1. Create new access key.
2. Update applications with new keys
3. Delete old set of keys.

## Security
*Do not apply access keys to the ROOT user*

*IAM Users are the only idenity that uses access keys*