---
layout: post
title:  "Visual Studio 2017 plugins for ASP.NET Core"
date:   2017-03-12 11:08:53 +0100
---

As I started to do some ASP.NET Core development with the new Visual Studio 2017, I wanted to set up my development environment as best as possible. In addition to the IDE I want to use some plugins.

I noticed that there was no IntelliSense for the HTML tag helpers like asp-action.

To have IntelliSense support for the asp-... HTML tags, you need to install the NuGet package Microsoft.AspNetCore.Razor.Tools In my case it was not sufficient to install the NuGet package. There is a known bug in the current version of Visual Studio with ASP.NET Core and the tag helpers. Installing the razor [language services package](https://marketplace.visualstudio.com/items?itemName=ms-madsk.RazorLanguageServices) helped for me.

Another plugin I'm using is the [Bootstrap snippet pack](https://marketplace.visualstudio.com/items?itemName=EricLebetsamer.BootstrapSnippetPack). This plugin provides bootstrap snippets, e.g. bootstrap class names.

I will extend the post if I found some more usefull plugins for ASP.NET Core.