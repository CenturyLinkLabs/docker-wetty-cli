Dockerized Wetty for CLIs
================
**This Image does not run on its own!**

This wetty version is designed to be used as the FROM image on another child image. The purpose of the image is to allow the second image to contain any head-less apps or CLIs installations and then benfit from the wetty browser. 

_Note_ : Only Chrome is supported.

To access wetty on Chrome, be sure to run the container mapping your host port to 3000. You can also add any environemental variables. For example:

`docker run --rm --name yourcli -p 8000:3000 -e "FOO=BAR" your/image`

If you are using VirtualBox, be sure to port forward to 8000 (if mapped as above) in order to view on your local machine. For example 8000 to 8000. 

To view, browse to:

`http://localhost:8000`

User: term

PW: term

