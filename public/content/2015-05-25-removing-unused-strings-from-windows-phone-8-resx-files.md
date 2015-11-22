---
title: Removing unused strings from Windows Phone 8 RESX files
author: Igor Kulman
layout: post
date: 2015-05-25
url: /removing-unused-strings-from-windows-phone-8-resx-files/
twitterCardType:
  - summary
cardImageWidth:
  - 280
cardImageHeight:
  - 150
dsq_thread_id:
  - 3791556033
categories:
  - Windows Phone
tags:
  - 'c#'
  - Windows Phone
  - xaml
---
Using RESX files is the standard approach to Windows Phone 8 app localization, it is even contained in the standard project templates. When you work on a project for a longer time, you may get to a situation that your RESX files contain strings that you no longer use. This is a problem especially when you want to add a new localization, because it is slower and kind of wasteful localizing unused strings.

To solve this problem I have created a simple command line utility, that is [available at Github][1]. This utility assumes that you use the standard localization approach from the templates (AppResources.{lang}.resx and LocalizedStrings.{value} in XAML).

The usage is really simple. Just run the utility with the path to your project as a parameter. It will detect all resources files and remove all the unused strings from them.

 [1]: https://github.com/igorkulman/RemoveUnusedResources