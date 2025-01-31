---
layout: essay
type: essay
title: "To Question Smartly"
# All dates must be YYYY-MM-DD format!
date: 2025-01-30
published: true
labels:
  - Learning
  - Communication
  - Deep thinking
---
<img width="600px" class="rounded float-start pe-4" src="../img/headerimage.jpg">

To employers in the software development industry, communicating effectively is a valued skill they look for in every potential candidate. A one-man army that can out-code everyone in the room is useless if they can't effectively communicate information between colleagues and managers. 
thus, it's important to know what effective communication looks like. Things like requesting specific tools/technology, organizing a strategy, gathering information from sources to solve a problem, etc. These are all basic forms of effective communication. In particular, being able to ask
SMART questions will improve your chances at information gathering and will more often than not lead you to a fix for your specific problem. I continue this writing by showing you two example questions, one being the smart way (as written about [here](http://www.catb.org/esr/faqs/smart-questions.html) by Eric Raymond in 'How to ask questions the smart way'), and one being the not-so-smart way. These questions were gathered from StackOverflow and links will be provided to you so you may explore the full questions and their responses.

## Before Asking a Question
It is advised that before asking a question, you should search for your answer via these methods:<br>
  "
  - Try to find an answer by searching the archives of the forum or mailing list you plan to post to.

  - Try to find an answer by searching the Web.

  - Try to find an answer by reading the manual.

  - Try to find an answer by reading a FAQ.

  - Try to find an answer by inspection or experimentation.

  - Try to find an answer by asking a skilled friend.

  - If you're a programmer, try to find an answer by reading the source code."
  (Raymond, 2014). 

## Asking a Smart Question
<img width="300px" class="rounded float-start pe-4" src="../img/smartquestion.jpg">
Eric Raymond's essay includes a lengthy guideline to assist those who read it an optimal way to ask a question. If you follow them, you are more likely to find an answer. Let's take a look at [this StackOverflow question](https://stackoverflow.com/questions/79401857/jenkins-offline-and-plugins-installation-failed-issue-in-azure-windows-10-vm) to see if it was asked smartly.


# Jenkins offline and plugins installation failed issue in Azure Windows 10 VM  

"I tried installing Jenkins on my Windows 10 Azure VM, but during the initial configuration, it shows that Jenkins is offline just before the plugins installation page. enter image description here

After referring to some blogs, I changed the jenkins.xml file by updating https://updates.jenkins.io/update-center.json to http://updates.jenkins.io/update-center.json.

After restarting the Jenkins service, I tried configuring Jenkins again, but this time I couldn’t install the suggested plugins. All plugin installations failed. I also tried adding the certificate to the Java cacerts file. The server has internet access.

enter image description here enter image description here

Could someone help me rectify this issue?

Jenkins version : Jenkins 2.479.3 LTS Java : open jdk version 17.0.14"




The asker's header is meaningful and specific. In Raymond's essay, he mentions "object-deviation", a method of generating a header in a way that shows what is having the issue (object) and what is the issue (deviation). Although a question is not asked directly, we as a reader can clearly understand 
the initial issue that the asker is facing is a failed plugin installation in an Azure Windows 10 virtual machine. As we look at the body of the question itself, the asker shows that they have tried referencing other sources for information before asking for help, thus we know that they are not, in Raymond's words, a "lazy sponge".
Furthermore, the asker writes clearly, taking care to write with grammatically correct spelling and syntax. This helps define the body of the question and conveys to us as the reader the exact issue with less of a chance of miscommunication due to a spelling error. The asker continues the body by describing their problem
chronologically and in a precise manner. They even include an image to show greater detail of the issue. This question follows many of Raymond's points and we can confidently say that this is a smart question!

## Asking a Dumb Question
<img width="300px" class="rounded float-start pe-4" src="../img/dumbquestion2.jpg"><br>

Perhaps dumb isn't the right word. I should say, there are no real dumb questions; every question is an opportunity for learning and growth. However, there are both good and bad ways to ask a question. [Here is an example](https://stackoverflow.com/questions/40048404/debugserver-died-with-an-exit-status-of-0x00000000) of a poorly posed question.

# debugserver died with an exit status of 0x00000000

"I was running an app on Xcode with the iPhone 6 stimulator using the latest iOS 10. And after some time the app crashed with the following message:
debugserver died with an exit status of 0x00000000

I ran the code at 7:56 PM and it crashed 9 minutes later. So does anyone have any idea why this is happening? Is this an indication that the app might crash when it goes to the background or anything else?"

This question is a good example of how NOT to ask a question as it breaks several principles that Raymond had outlined. Starting with the header, it does not follow the "object-deviation" method. At a glance, there is no way of understanding what the problem is, and more than that, we have no idea what is experiencing the problem. It is a meaningless header with no clarity. Another problem with this question is that the asker does not describe any goal, only the steps they took. If you want a reader to understand definitively what it is you are trying to accomplish, you need to outline a goal that you have and why your issue is preventing you from reaching it. Then the reader can begin to understand why you took the steps you did to try and solve the problem. The final issue with the question is that at the end, the asker starts to include their guesses as to why their issue is happening. This is bad because it is pointless; as in why bother consulting others if you're guessing what the problem is? You should perhaps then diagnose the problem first (using your guess), and if it doesn't work, include that in the body of the question.

## Afterthoughts
I hope that the two question examples posed were insightful to anyone reading this. Chances are that we all have asked a 'dumb' question before, and we'll probably do it again. I hope that in the future you (and I) remember these examples of good and bad questions. A good question can lead to good answers while a bad question always leads to indifference. 


