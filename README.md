# ![LOGO](logo.png) SwaggerHub Registry **flow**ground Connector

## Description

A generated **flow**ground connector for the SwaggerHub Registry API (version 1.0.47).

Generated from: https://api.apis.guru/v2/specs/swaggerhub.com/1.0.47/swagger.json<br/>
Generated at: 2019-05-07T17:44:19+03:00

## API Description

# Introduction
This is the registry API for SwaggerHub. It allows you to access, manage, and update your APIs and Domains in SwaggerHub bypassing the Web application.

# Authentication
Use your personal API Key: you can find it by visiting the [API Key page](https://app.swaggerhub.com/settings/apiKey).


## Authorization

Supported authorization schemes:
- API Key
## Actions

### Retrieves a list of currently defined APIs in APIs.json format.

*Tags:* `APIs`

#### Input Parameters
* `query` - _optional_ - Free text query to match
* `state` - _optional_ - Matches against published state of the spec:
* UNPUBLISHED - spec is a draft, a work in progress
* PUBLISHED - spec is a stable version ready for consuming from client applications
* ANY - either PUBLISHED or UNPUBLISHED

    Possible values: ALL, PUBLISHED, UNPUBLISHED.
* `tag` - _optional_ - Matches against tags associated with an API
* `page` - _optional_ - Page to return
* `limit` - _optional_ - Number of results per page
* `sort` - _optional_ - Sort criteria or result set:
* NAME
* UPATED
* CREATED
* OWNER

    Possible values: NAME, UPDATED, CREATED, OWNER.
* `order` - _optional_ - Sort order
    Possible values: ASC, DESC.

### Retrieves an APIs.json listing of all APIs defined for this owner

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `page` - _optional_ - Page to return
* `limit` - _optional_ - Number of results per page
* `sort` - _optional_ - Sort criteria or result set:
* NAME
* UPATED
* CREATED
* OWNER

    Possible values: NAME, UPDATED, CREATED, OWNER.
* `order` - _optional_ - Sort order
    Possible values: ASC, DESC.

### Deletes the specified API

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)

### Retrieves an APIs.json listing for all API versions for this owner and API

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)

### Saves the provided Swagger definition

> Saves the provided Swagger definition; the owner must match the token owner. The version will be extracted from the Swagger definition itself.

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `isPrivate` - _optional_ - Defines whether the API has to be private
* `version` - _optional_ - API version
* `oas` - _optional_ - The OpenApi Specification (OAS)
  version.
* 2.0 - For OAS2 (aka 'Swagger 2.0')
* 3.0.X - For OAS3

    Possible values: 2.0, 3.0.0, 3.0.1.
* `force` - _optional_ - Force update

### Deletes API's collaboration

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)

### Gets API's collaboration

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `expandTeams` - _optional_

### Updates API's collaboration

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)

### Deletes a particular version of the specified API

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves the Swagger definition for the specified API and version

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Returns comments for the specified API version

> Returns all the comments and replies added by collaborators in the specified API version.

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves the Swagger definition for the specified API and version in JSON format

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves the Swagger definition for the specified API and version in YAML format

*Tags:* `APIs`

#### Input Parameters
* `owner` - _required_ - API owner (user or organization, case-sensitive)
* `api` - _required_ - API name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves a list of currently defined domains in APIs.json format

*Tags:* `Domains`

#### Input Parameters
* `query` - _optional_ - Free text query to match
* `state` - _optional_ - Matches against published state of the spec:
* UNPUBLISHED - spec is a draft, a work in progress
* PUBLISHED - spec is a stable version ready for consuming from client applications
* ANY - either PUBLISHED or UNPUBLISHED

    Possible values: ALL, PUBLISHED, UNPUBLISHED.
* `tag` - _optional_ - Matches against tags associated with a domain
* `page` - _optional_ - Page to return
* `limit` - _optional_ - Number of results per page
* `sort` - _optional_ - Sort criteria or result set:
* NAME
* UPATED
* CREATED
* OWNER

    Possible values: NAME, UPDATED, CREATED, OWNER.
* `order` - _optional_ - Sort order
    Possible values: ASC, DESC.

### Retrieves an APIs.json listing of all domains defined for this owner

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `page` - _optional_ - Page to return
* `limit` - _optional_ - Number of results per page
* `sort` - _optional_ - Sort criteria or result set:
* NAME
* UPATED
* CREATED
* OWNER

    Possible values: NAME, UPDATED, CREATED, OWNER.
* `order` - _optional_ - Sort order
    Possible values: ASC, DESC.

### Deletes the specified domain

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `force` - _optional_ - Force update

### Retrieves an APIs.json listing for all domain versions for this owner and domain

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)

### Saves the provided Swagger definition of a domain

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `isPrivate` - _optional_ - Specifies whether the domain has to be private
* `version` - _required_ - Domain version
* `force` - _optional_ - Force update

### Deletes a particular version of the specified domain

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)
* `force` - _optional_ - Force update

### Retrieves the Swagger definition for the specified domain and version

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Returns comments for the specified domain version

> Returns all the comments and replies added by collaborators in the specified domain version.

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves the definition for the specified domain and version in JSON format

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves the definition for the specified domain and version in YAML format

*Tags:* `Domains`

#### Input Parameters
* `owner` - _required_ - Domain owner (user or organization, case-sensitive)
* `domain` - _required_ - Domain name (case-sensitive)
* `version` - _required_ - Version identifier (case-sensitive)

### Retrieves a list of currently defined APIs and Domains in APIs.json format

*Tags:* `APIs` `Domains`

#### Input Parameters
* `specType` - _optional_ - Type of Swagger specs to search:
* API - APIs only
* DOMAIN - Domains only
* ANY - Both APIs and Domains

    Possible values: API, DOMAIN, ANY.
* `visibility` - _optional_ - The visibility of a spec in SwaggerHub:
* PUBLIC - can be viewed by anyone
* PRIVATE - can only be viewed by you or your Org and those that you are collaborating with or have shared it with
* ANY - either PUBLIC or PRIVATE

    Possible values: PUBLIC, PRIVATE, ANY.
* `state` - _optional_ - Matches against published state of the spec:
* UNPUBLISHED - spec is a draft, a work in progress
* PUBLISHED - spec is a stable version ready for consuming from client applications
* ANY - either PUBLISHED or UNPUBLISHED

    Possible values: ALL, PUBLISHED, UNPUBLISHED.
* `owner` - _optional_ - API or Domain owner identifier. Can be username or organization name
* `query` - _optional_ - Free text query to match
* `page` - _optional_ - Page to return
* `limit` - _optional_ - Number of results per page
* `sort` - _optional_ - Sort criteria or result set:
* NAME
* UPATED
* CREATED
* OWNER

    Possible values: NAME, UPDATED, CREATED, OWNER.
* `order` - _optional_ - Sort order
    Possible values: ASC, DESC.

## License

**flow**ground :- Telekom iPaaS / swaggerhub-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
