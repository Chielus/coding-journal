+++
title = "AutoCompleteBox for Universal Apps"
date = "2012-09-19T05:56:44"
link = "https://github.com/igorkulman/AutoCompleteBox"
+++

There is no AutoCompleteBox control that can be used when building Windows Store apps in C# and XAML so I decided to create one, because I needed it for a project. Currently it supports only String collections and the selected value must be accessed using code behind, but this will hopefully change. 

The AutoCompleteBox uses WinRT XAML Toolkit to show the watermark andReactive Extensions so the users does not need to press enter, the results will show after they stop typing for a second.

### Installation


    PM> Install-Package AutoCompleteBoxWinRT

<!--more-->