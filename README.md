# ![LOGO](logo.png) SearchManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the SearchManagementClient API (version 2015-08-19).

Generated from: https://api.apis.guru/v2/specs/azure.com/search/2015-08-19/swagger.json<br/>
Generated at: 2019-05-07T17:38:49+03:00

## API Description

Client that can be used to manage Azure Search services and API keys.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the available REST API operations of the Microsoft.Search provider.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.

### Checks whether or not the given Search service name is available for use. Search service names must be globally unique since they are part of the service URI (https://<name>.search.windows.net).

*Tags:* `Services`

#### Input Parameters
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Gets a list of all Search services in the given subscription.

*Tags:* `Services`

#### Input Parameters
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Gets a list of all Search services in the given resource group.

*Tags:* `Services`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Deletes a Search service in the given resource group, along with its associated resources.

*Tags:* `Services`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Gets the Search service with the given name in the given resource group.

*Tags:* `Services`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Updates an existing Search service in the given resource group.

*Tags:* `Services`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service to update.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Creates or updates a Search service in the given resource group. If the Search service already exists, all properties will be updated with the given values.

*Tags:* `Services`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service to create or update. Search service names must only contain lowercase letters, digits or dashes, cannot use dash as the first two or last one characters, cannot contain consecutive dashes, and must be between 2 and 60 characters in length. Search service names must be globally unique since they are part of the service URI (https://<name>.search.windows.net). You cannot change the service name after the service is created.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Generates a new query key for the specified Search service. You can create up to 50 query keys per service.

*Tags:* `QueryKeys`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `name` - _required_ - The name of the new query API key.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Deletes the specified query key. Unlike admin keys, query keys are not regenerated. The process for regenerating a query key is to delete and then recreate it.

*Tags:* `QueryKeys`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `key` - _required_ - The query key to be deleted. Query keys are identified by value, not by name.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Gets the primary and secondary admin API keys for the specified Azure Search service.

*Tags:* `AdminKeys`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Returns the list of query API keys for the given Azure Search service.

*Tags:* `QueryKeys`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

### Regenerates either the primary or secondary admin API key. You can only regenerate one key at a time.

*Tags:* `AdminKeys`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group within the current subscription. You can obtain this value from the Azure Resource Manager API or the portal.
* `searchServiceName` - _required_ - The name of the Azure Search service associated with the specified resource group.
* `keyKind` - _required_ - Specifies which key to regenerate. Valid values include 'primary' and 'secondary'.
    Possible values: primary, secondary.
* `x-ms-client-request-id` - _optional_ - A client-generated GUID value that identifies this request. If specified, this will be included in response information as a way to track the request.
* `api-version` - _required_ - The API version to use for each request. The current version is 2015-08-19.
* `subscriptionId` - _required_ - The unique identifier for a Microsoft Azure subscription. You can obtain this value from the Azure Resource Manager API or the portal.

## License

**flow**ground :- Telekom iPaaS / azure-com-search-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
