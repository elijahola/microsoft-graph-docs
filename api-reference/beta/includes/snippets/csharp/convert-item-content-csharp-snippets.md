---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Content.GetAsync((requestConfiguration) =>
{
	requestConfiguration.QueryParameters.Format = "{format}";
});


```