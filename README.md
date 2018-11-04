# Shaasgaz

Shaasgaz is a comprehensive tool that manages the secure access to your resources in AWS.

# Where does the name come from? 

Shaashgaz (shå-ash'-gaz) is a biblical character, from the Book of Esther [Chapter 2, verse 14](https://biblehub.com/esther/2-14.htm) 

*"In the evening she went, and on the morrow she returned into the second house of the women, to the custody of Shaashgaz, the king’s chamberlain, who kept the concubines: she came in unto the king no more, except the king delighted in her, and she were called by name."*

I chose this name because the character in the book of Esther was the the one that was responsible for one of the most important jewels of King Ahasuerus' - his queen. She was entrusted to Shaashguz so that he would guard her (and of course all of the kings other concubines).

# Background

One of the weakest links in any cloud architecture are the entry points into the system, which are usually your [bastion hosts](https://aws.amazon.com/blogs/security/tag/bastion-host/). 

This tool was built to allow access to number of bastion hosts from anywhere in the world.

# How does it work?

A support engineer will access an static web page which is backed by an API gateway.

With the request the user's public IP will be populated into their request - which will be a drop down of the current instances thay they have access too. 

By default the user will have access for the next 30 minutes - this can be changed
