# Add a new entity client for compliance review

- At least one Control Person is required as a Significant Party.
- Documents are optional for the client and its significant parties.
- 'Other' documents can be added in the Documents list (fileName and content).
- After the client is saved, a CDD Check will be automatically triggered and executed asynchronously.

## Request
### Post
https://api.finclusive.com/customer/{customerFinClusiveId}/client/entity
