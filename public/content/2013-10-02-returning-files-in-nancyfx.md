---
title: Returning files in NancyFX
author: Igor Kulman
layout: post
date: 2013-10-02
url: /returning-files-in-nancyfx/
dsq_thread_id:
  - 1817065926
categories:
  - Windows Azure
tags:
  - azure
  - 'c#'
  - NancyFX
---
In my current project, I have chosen [NancyFx][1] to implement a REST API. NancyFx is a .NET framework known for its &#8220;[super-duper-happy-path][2]&#8220;. 

In one use case I generate a ZIP file in the temp folder and I want the API to return this ZIP file. NancyFx contains a Responses.AsFile helper but it works only with paths relative to the application. 

If you have an absolute path of a file, you cannot use it. You need to create a StreamResponse and return the file as an attachment

 [1]: http://nancyfx.org/
 [2]: https://github.com/NancyFx/Nancy/wiki/Introduction#the-super-duper-happy-path