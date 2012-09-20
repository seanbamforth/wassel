Instructions. 
==============

What it is
----------
Wassel is a CoffeeScript and Less preprocessor for Visual Dataflex. 

what that means
----------
With increasingly complex web applications, CSS and Javascript are becoming increasingly hard to manage. Less and Coffeescript are designed to make it easier to create these web applications. 

You can learn more about LESS by going to : 
- http://lesscss.org/

You can learn more about Coffeescript by going to : 
- http://coffeescript.org/


What comes with it
----------
As well as coffeescript and less compilers, we've included jquery and bootstrap. If you haven't created an assets folder, then these will automatically be copied to it the first time you view an ASP file containing the `<%=oWassel.call("assets")%>`command. 

Links for the included modules are as follows: 

-  https://github.com/alisey/CoffeeScript-Compiler-for-Windows
-  https://github.com/duncansmart/less.js-windows
-  http://twitter.github.com/bootstrap/
-  http://jquery.com/

How to use it
----------
1) Create a copy of this project. You can download it using the "zip" option above, or if you've got and use git, you can just clone the repo. 

2) Include the wassel library in your web application using "tools -> maintain libraries" from the visual dataflex IDE

3) Create a new ASP file, and add the line 

`
<%=oWassel.call("assets")%>
`

to the `<head>` section of this file. 

4) Add the line `Use assets.pkg` to webapp.src as the first include inside your cWebApp object.

5) Create a new registry key in 
  `HKLM\Data Access Worldwide\Visual Dataflex\17.0\`

called
  `Asset Compiler`

with the value being the "compilers" folder of the "wassel" library 
  e.g. `C:\data\Visual DataFlex Projects\wassel\compilers`


6) Compile and open your ASP file. 

7) Add your .coffee and .less files to the assets\coffeescript & assets\less folders. Your .less files may need to be included as imports in the main.less file. 

8) That should be it, but it's new software, so it may not work...


Can you help
----------
Yes - If you use the library, consider throwing a donation my way (paypal sean@theguru.co.uk). If you're of a mind, you can make changes to the library too. Email me the details, or send me a pull request. I haven't quite worked out how to do pull requests, but I'll do my best. 

