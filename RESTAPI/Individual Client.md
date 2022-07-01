# Add a new individual client for compliance review

- Individual Client Significant Parties are optional.
- Documents are optional for the client and its significant parties.
- An identification document (fileName and content) must be sent together with the documentType, isoCountryCode (of the document) and identificationNumber when adding the document.
- 'Other' documents can be added in the Documents list (fileName and content).
- After the client is saved, a CDD Check will be automatically triggered and executed asynchronously.

## Request
### Post
https://api.finclusive.com/customer/{customerFinClusiveId}/client/individual

## JSON Example
```
{
    "finClusiveId": "23232323",
    "individualId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
    "firstName": "John",
    "lastName": "Doe",
    "emailAddress": "email@address.com",
    "phoneNumber": "+15417543010",
    "phoneNumberType": 0,
    "taxIdNumber": "3434343",
    "address": {
        "address1": "123 Main Street",
        "address2": "Apartment A-12",
        "city": "San Francisco",
        "state": "CA",
        "postalCode": "94203",
        "isoCountryCode": "US",
        "addressId": "61fffd90-d462-4d09-8b3c-15c8625d98a5"
    },
    "dateOfBirth": "2020-03-20T00:00:00Z",
    "document": {
        "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
        "documentUrl": "https://adocumentdomain.com/documenturl",
        "identificationNumber": "3435666",
        "documentType": 2,
        "fileName": "SampleFileName.txt",
        "content": "data:text/plain;base64,dGVzdDEyMw==",
        "isoCountryCode": "US"
    },
    "documents": [{
        "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
        "documentUrl": "https://adocumentdomain.com/documenturl",
        "identificationNumber": "3435666",
        "documentType": 2,
        "fileName": "SampleFileName.txt",
        "content": "data:text/plain;base64,dGVzdDEyMw==",
        "isoCountryCode": "US"
    }],
    "memoFields": [{
        "name": "MyCustomMemoField",
        "value": "string"
    }],
    "bvn": "08076665555",
    "isCreatedThroughStellarViaSEP12": "0",
    "customAttributes": [{
        "name": "CustomFieldName",
        "value": "ThisIsACustomFieldValue"
    }],
    "individualBeneficiaries": [{
        "firstName": "John",
        "lastName": "Doe",
        "emailAddress": "email@address.com",
        "phoneNumberType": 0,
        "dateOfBirth": "2020-03-20T00:00:00Z",
        "document": {
            "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
            "documentUrl": "https://adocumentdomain.com/documenturl",
            "identificationNumber": "3435666",
            "documentType": 2,
            "fileName": "SampleFileName.txt",
            "content": "data:text/plain;base64,dGVzdDEyMw==",
            "isoCountryCode": "US"
        },
        "id": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
        "type": "string",
        "address": {
            "address1": "123 Main Street",
            "address2": "Apartment A-12",
            "city": "San Francisco",
            "state": "CA",
            "postalCode": "94203",
            "isoCountryCode": "US",
            "addressId": "61fffd90-d462-4d09-8b3c-15c8625d98a5"
        },
        "taxIdNumber": "3434343",
        "phoneNumber": "+15417543010",
        "bvn": "08076665555",
        "customAttributes": [{
            "name": "CustomFieldName",
            "value": "ThisIsACustomFieldValue"
        }],
        "documents": [{
            "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
            "documentUrl": "https://adocumentdomain.com/documenturl",
            "identificationNumber": "3435666",
            "documentType": 2,
            "fileName": "SampleFileName.txt",
            "content": "data:text/plain;base64,dGVzdDEyMw==",
            "isoCountryCode": "US"
        }]
    }],
    "entityBeneficiaries": [{
        "legalName": "FinClusive",
        "incorporationDocument": {
            "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
            "documentUrl": "https://adocumentdomain.com/documenturl",
            "identificationNumber": "3435666",
            "documentType": 2,
            "fileName": "SampleFileName.txt",
            "content": "data:text/plain;base64,dGVzdDEyMw==",
            "isoCountryCode": "US"
        },
        "jurisdictionDocument": {
            "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
            "documentUrl": "https://adocumentdomain.com/documenturl",
            "identificationNumber": "3435666",
            "documentType": 2,
            "fileName": "SampleFileName.txt",
            "content": "data:text/plain;base64,dGVzdDEyMw==",
            "isoCountryCode": "US"
        },
        "id": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
        "type": "string",
        "address": {
            "address1": "123 Main Street",
            "address2": "Apartment A-12",
            "city": "San Francisco",
            "state": "CA",
            "postalCode": "94203",
            "isoCountryCode": "US",
            "addressId": "61fffd90-d462-4d09-8b3c-15c8625d98a5"
        },
        "taxIdNumber": "3434343",
        "phoneNumber": "+15417543010",
        "bvn": "08076665555",
        "customAttributes": [{
            "name": "CustomFieldName",
            "value": "ThisIsACustomFieldValue"
        }],
        "documents": [{
            "documentId": "459cf6dc-7cde-4a95-a4f8-ab56a45b62f9",
            "documentUrl": "https://adocumentdomain.com/documenturl",
            "identificationNumber": "3435666",
            "documentType": 2,
            "fileName": "SampleFileName.txt",
            "content": "data:text/plain;base64,dGVzdDEyMw==",
            "isoCountryCode": "US"
        }]
    }],
    "isDonor": true
}
```
