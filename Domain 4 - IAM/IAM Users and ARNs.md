# IAM Users and ARNs

**IAM users are an identity used for anything requiring `long-term` AWS access e.g. `Humans`, `Applications`, or service accounts.**

* Principal: Identity trying to access an AWS Account
  * People
  * Computers
  * Services
  * Group
* Principal -> IAM (Authentication) -> Authenticated Identity

* Authentication Methods
  * Username, Password
  * Access Keys


### Amazon Resource Name (ARN)
**Uniquely indentify resources within any AWS Account.**
```sh
arn:partition:service:region:account-id:resource-id`
arn:partition:service:region:account-id:resource-type/resource-id
arn:partition:service:region:account-id:resource-type:resource-id
```

Similar but different ARNs
```sh
arn:aws:s3:::catgifs <- References the actual bucket and not the objects
arn:aws:s3:::catgifs/* <- References the objects within the bucket
```

## Limitations
* `5,000` IAM Users per account.
* IAM Users can be a member of `10` groups.
* This has system design impacts.
  * Internet scale applications
  * Large orgs & org merges
  * IAM Roles and Identity Federation (Fix for design impacts)