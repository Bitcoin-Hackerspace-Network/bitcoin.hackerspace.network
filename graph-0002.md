```
GRAPH: 2
Title: Upgrade Temp Schema from graph-0001
Status: Active
Author: Bryan Nonni <bryan@atlbitlab.com>
Created: 2023-09-06
License: Creative Commons Zero v1.0 Universal (CC0)
```
## Abstract
This GRAPH proposes reducing the size of the credential schema from [graph-0001](./graph-0001.mediawiki).

## Specification

- [Member Schema](./graph-0002/schemas/Member.json)

```json
{
  "name": "Bitcoin Hackerspace Network (BTCHackNet) - Membership",
  "issuer": "did:key:z6Mkgza8PyhXaCKYZr7ebHczB6mQs1JxvQkkQC5ZMnmFyKrq",
  "verificationMethodId": "did:key:z6Mkgza8PyhXaCKYZr7ebHczB6mQs1JxvQkkQC5ZMnmFyKrq#z6Mkgza8PyhXaCKYZr7ebHczB6mQs1JxvQkkQC5ZMnmFyKrq",
  "description": "JSON schema for a verifiable credential issued to a member of a bitcoin hackerspace containing details about the member's membership to the issuer hackerspace and network of hackerspaces.",
  "schema": {
    "$schema": "https://json-schema.org/draft/2020-12/schema",
    "type": "object",
    "properties": {
      "required": [
        "name",
        "email",
        "membership"
      ],
      "name": {
        "type": "string",
        "description": "Member name."
      },
      "email": {
        "type": "string",
        "description": "Member email."
      },
      "website": {
        "type": "string",
        "description": "Member website."
      },
      "telegram": {
        "type": "string",
        "description": "Member telegram handle."
      },
      "x": {
        "type": "string",
        "description": "Member twitter handle."
      },
      "npub": {
        "type": "string",
        "description": "Member nostr npub."
      },
      "nip5": {
        "type": "string",
        "description": "Member nostr nip5."
      },
      "membership": {
        "type": "object",
        "required": [
          "network",
          "hackerspace",
          "title",
          "tier",
          "description",
          "benefits"
        ],
        "properties": {
          "network": {
            "type": "string",
            "description": "Issuing hackerspace network name."
          },
          "hackerspace": {
            "type": "string",
            "description": "Issuing hackerspace name."
          },
          "title": {
            "type": "string",
            "description": "Membership title."
          },
          "tier": {
            "type": "number",
            "description": "Membership tier."
          },
          "description": {
            "type": "string",
            "description": "General information about membership."
          },
          "benefits": {
            "type": "array",
            "description": "Amentities, benefits and/or restrictions associated with the membership."
          }
        }
      }
    }
  }
}
```

TODO: Diagram

## Implementation

- [Member Credential](./graph-0002/credentials/)

```json
{
    
}
```