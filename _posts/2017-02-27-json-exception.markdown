---
layout: post
title:  "Newtonsoft JSON exception: Can not add JProperty to JArray"
date:   2017-02-27 08:22:00 +0100
---

Today I get some unexpected behaviuor while using the Newtonsoft JSON library.
In my experience, the library is really cool and makes good error messages.
Today I get an ArgumentException with the message: "Can not add JProperty to JArray".
The confusing thing was, there was not JProperty added to a JArray.

![Exception message]({{ site.url }}/assets/2017-02-27-exception.png "Exception message")

After splitting the statement, the error was identified. The correct error message should be: "Can not add JProperty to JProperty".
So I added a JObject in between the to JProperties the error was fixed.

![Fixed code]({{ site.url }}/assets/2017-02-27-fix.png "Fixed code")
