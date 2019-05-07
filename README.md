# ![LOGO](logo.png) Admin Reports **flow**ground Connector

## Description

A generated **flow**ground connector for the Admin Reports API (version reports_v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/admin/reports_v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:07+03:00

## API Description

Fetches reports for the administrators of G Suite customers about the usage, collaboration, security, and risk for their users.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Retrieves a list of activities for a specific customer and application.

*Tags:* `activities`

#### Input Parameters
* `actorIpAddress` - _optional_ - IP Address of host where the event was performed. Supports both IPv4 and IPv6 addresses.
* `applicationName` - _required_ - Application name for which the events are to be retrieved.
* `customerId` - _optional_ - Represents the customer for which the data is to be fetched.
* `endTime` - _optional_ - Return events which occurred at or before this time.
* `eventName` - _optional_ - Name of the event being queried.
* `filters` - _optional_ - Event parameters in the form [parameter1 name][operator][parameter1 value],[parameter2 name][operator][parameter2 value],...
* `maxResults` - _optional_ - Number of activity records to be shown in each page.
* `orgUnitID` - _optional_ - the organizational unit's(OU) ID to filter activities from users belonging to a specific OU or one of its sub-OU(s)
* `pageToken` - _optional_ - Token to specify next page.
* `startTime` - _optional_ - Return events which occurred at or after this time.
* `userKey` - _required_ - Represents the profile id or the user email for which the data should be filtered. When 'all' is specified as the userKey, it returns usageReports for all users.

### Push changes to activities

*Tags:* `activities`

#### Input Parameters
* `actorIpAddress` - _optional_ - IP Address of host where the event was performed. Supports both IPv4 and IPv6 addresses.
* `applicationName` - _required_ - Application name for which the events are to be retrieved.
* `customerId` - _optional_ - Represents the customer for which the data is to be fetched.
* `endTime` - _optional_ - Return events which occurred at or before this time.
* `eventName` - _optional_ - Name of the event being queried.
* `filters` - _optional_ - Event parameters in the form [parameter1 name][operator][parameter1 value],[parameter2 name][operator][parameter2 value],...
* `maxResults` - _optional_ - Number of activity records to be shown in each page.
* `orgUnitID` - _optional_ - the organizational unit's(OU) ID to filter activities from users belonging to a specific OU or one of its sub-OU(s)
* `pageToken` - _optional_ - Token to specify next page.
* `startTime` - _optional_ - Return events which occurred at or after this time.
* `userKey` - _required_ - Represents the profile id or the user email for which the data should be filtered. When 'all' is specified as the userKey, it returns usageReports for all users.

### Stop watching resources through this channel

*Tags:* `channels`

#### Input Parameters
* `alt` - _optional_ - Data format for the response.
    Possible values: json.
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a report which is a collection of properties / statistics for a specific customer.

*Tags:* `customerUsageReports`

#### Input Parameters
* `customerId` - _optional_ - Represents the customer for which the data is to be fetched.
* `date` - _required_ - Represents the date in yyyy-mm-dd format for which the data is to be fetched.
* `pageToken` - _optional_ - Token to specify next page.
* `parameters` - _optional_ - Represents the application name, parameter name pairs to fetch in csv as app_name1:param_name1, app_name2:param_name2.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - An opaque string that represents a user for quota purposes. Must not exceed 40 characters.
* `userIp` - _optional_ - Deprecated. Please use quotaUser instead.

### Retrieves a report which is a collection of properties / statistics for a set of users.

*Tags:* `userUsageReport`

#### Input Parameters
* `customerId` - _optional_ - Represents the customer for which the data is to be fetched.
* `date` - _required_ - Represents the date in yyyy-mm-dd format for which the data is to be fetched.
* `filters` - _optional_ - Represents the set of filters including parameter operator value.
* `maxResults` - _optional_ - Maximum number of results to return. Maximum allowed is 1000
* `orgUnitID` - _optional_ - the organizational unit's ID to filter usage parameters from users belonging to a specific OU or one of its sub-OU(s).
* `pageToken` - _optional_ - Token to specify next page.
* `parameters` - _optional_ - Represents the application name, parameter name pairs to fetch in csv as app_name1:param_name1, app_name2:param_name2.
* `userKey` - _required_ - Represents the profile id or the user email for which the data should be filtered.

### Retrieves a report which is a collection of properties / statistics for a set of objects.

*Tags:* `entityUsageReports`

#### Input Parameters
* `customerId` - _optional_ - Represents the customer for which the data is to be fetched.
* `date` - _required_ - Represents the date in yyyy-mm-dd format for which the data is to be fetched.
* `entityKey` - _required_ - Represents the key of object for which the data should be filtered.
* `entityType` - _required_ - Type of object. Should be one of - gplus_communities.
* `filters` - _optional_ - Represents the set of filters including parameter operator value.
* `maxResults` - _optional_ - Maximum number of results to return. Maximum allowed is 1000
* `pageToken` - _optional_ - Token to specify next page.
* `parameters` - _optional_ - Represents the application name, parameter name pairs to fetch in csv as app_name1:param_name1, app_name2:param_name2.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-admin-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
