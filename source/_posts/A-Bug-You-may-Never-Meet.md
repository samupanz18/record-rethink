---
title: A Bug You may Never Meet
date: 2016-07-14 18:43:33
tags: 
- Thought
comments: true
---
For convenience recently I turned my Dell 24' display into the portait mode so that I can split Sublime into two editors which align vertically.

Today when I finished a task I decided to close all the opened files. Easy, right? I just need to click the *File / Close All Files* menu item. Firstly I clicked the *File* menu but I can't find the *Close All Files* command. I'm sure it locates at the end of the *File* menu. I moved the cursor on the *File* menu for several times and finally found that it is hidden by the sub menu of the *Open Recent* command. This sub menu is too wide to follow its parent. So it displays under its parent. Because I opened a lot of files so the sub menu is very high and hides most items of the *File* menu. It's annoying! I have to bypass the the *Open Recent* command to prevent its sub menu from showing so that I can click the *Close All Files* command.

What I learned from this case is that **we should never hurry to say that our softwares are bug free**. Because there always is a special context in which they run. If we haven't considered that context in advance the bug happens finally.