---
title: .Net 中MimeType 的获取
categories:
	- .NET
tags:
	- C#
---

### .NetFramework 中获取 MimeType

```csharp
// using System.Web;
MimeMapping.GetMimeMapping(filename);
```

### .NetCore 中获取MimeType

```csharp
//using Microsoft.AspNetCore.StaticFiles;
FileExtensionContentTypeProvider fileExtensionContentTypeProvider;
string contentType;
fileExtensionContentTypeProvider.TryGetContentType(filename,out contentType);
```
