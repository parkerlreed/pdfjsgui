pdfjsgui
========

A small python script to load pdf.js as it's own application

Found the example python here. http://ardoris.wordpress.com/2009/04/26/a-browser-in-14-lines-using-python-and-webkit/

It works decently for now but the program does not exit upon closing the GUI.

========

Requires python-webkit and nodejs for compiling pdf.js

sudo apt-get install python-webkit nodejs
  
========

Clone the pdf.js repo and then compile it

git clone git://github.com/mozilla/pdf.js

cd pdf.js

nodejs make generic

========

Then copy out the generic directory to whereever you want it. I chose my user's bin folder

cp -R build/generic/ ~/bin/

========

Then just replace the URL in the pdfjs script with whatever path your files reside at.

file:///home/parker/bin/generic/web/viewer.html
