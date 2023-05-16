#IAM Policies

**Identity Policies are attached to AWS identities and either ALLOW or DENY access to AWS resources.**

* Policies contain one or more statements
  * Sid = statement id (optional description)
  * Effect = Allow / Deny
  * Action = Operation
  * Resource = AWS ARN to perform the action on
  * **Explicit Deny always take priority over Allow**
  * Default Deny = Implicit

* Multiple Policies assoicated
  * AWS Collects all policies together and evaluates them all at the same time. Deny  (Explicit) -> Allow (Explicit) -> Deny (Implicit)

* Two types of policies: inline and managed
  * Inline: Applied to each account individually (Special or Exceptional Allow or Deny)
  * Managed: Own object applied to multiple accounts or groups.
    * Reusbable
    * Low Management Overhead