# MvcDynamicForms

Create dynamic forms in ASP.NET MVC.

#Requirements

this library requires .NET 4.5.2 and above.

# Installation

You can either <a href="https://github.com/lettucebo/MvcDynamicForms.git">download</a> the source and build your own dll or, if you have the NuGet package manager installed, you can grab them automatically.

```
PM> Install-Package MvcDynamicForms
```

Once you have the libraries properly referenced in your project, you can include calls to them in your code. 
For a sample implementation, check the [Demo](https://github.com/lettucebo/MvcDynamicForms/tree/master/MvcDynamicForms.Demo) folder.

Add the following namespaces to use the library:
``` csharp
using MvcDynamicForms.Core;
using MvcDynamicForms.Core.Fields;
```

# Getting Started

First off, below Demos do the exact same thing from the end user's perspective. The difference is in how the Form object is persisted across requests.

Most often, you'll need to keep the original Form and Field objects around for as long as your user is working on completing the form. This is because, when InputField objects are constructed, they are keyed with a new Guid. See [How to #1](#how-to-1) & [How to #2](#how-to-2) for examples.

You can key your InputFields manually by setting the InputField.Key property. If you do this and can guarantee that the Fields and their Keys will not change after a complete reconstruction of all objects, then you don't have to persist the objects across requests. See [How to #3](#how-to-3).

# How to #1

# How to #2

# How to #3
