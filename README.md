github-jscraper
===============

How does the Wikiscraper class work?

he Wikiscraper class works by calling the scrapeTopic method, which will eventually print the first paragraph of text in the Wikipedia article to the screen. Furthermore, scrapeTopic requires another method, getURL, in order to do this. The getURL takes in an arbitrary URL and returns the raw source code as a string. Essentially, it creates a Java URL object from the URL string, and calls the openConnection method on that URL object. The openConnection method returns a URLconnection object, which can be used to create a BufferedReader object.
BufferedReader objects are designed to read from streams of text, stopping at a certain size limit, or reading streams one line at a time. In addition, the while loop here retrieves the text from the BufferedReader object one line at a time and adds it to outputText, which is then returned. After the getURL method has returned the HTML string to scrapeTopic, jsoup is used. The jsoup select function returns a jsoup object, which can be further manipulated, or turned into text, and printed.

Project Specific

You should probably always share the .project file and never .settings/ files. The .classpath may depend on your environment but I would not suggest to share it either, because it can cause conflicts (for example if one user uses openjdk and the other uses sun-jdk. The .settings contains preferences and settings for eclipse and changes a lot, thus it should not be shared. If you properly import the project after you cloned it from git then you will also not have any problems.

