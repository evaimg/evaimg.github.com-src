
# Source files for evaimg.github.com website generation
----------------------

Web pages of www.evaimg.org are generated Pelican, a nice static site generator written in Python.
# How to use
## Requirements
* Python 2.7+
* Pelican 3.3 (python library)
* Markdown (python library)
## Generate pages
### Windows
User of Windows can use pmake.cmd to generate pages and debug. Commands can be run like this:
```
.\pmake COMMAND
```
The following commands are available: 
 * **.\pmake html** (re)generate the web site
 * **.\pmake clean** remove the generated files
 * **.\pmake regenerate** regenerate files upon modification
 * **.\pmake publish** generate using production settings
 * **.\pmake serve** serve site at http://localhost:8000
 * **.\pmake devserver** start/restart develop_server.sh
 * **.\pmake upload ssh** upload the web site via SSH
 * **.\pmake upload rsync** upload the web site via rsync+ssh
 * **.\pmake upload dropbox** upload the web site via Dropbox
 * **.\pmake upload ftp** upload the web site via FTP
 * **.\pmake upload github** upload the web site via gh-pages

For example, you can use the following command to generate pages and upload to evaimg.github.io (master branch):
```
.\pmake html
.\pmake upload github
```

### Linux and Mac
Make tool can be used in these platform, a make file similar to the pmake.cmd is provided by Pelican. Just the type the following command:
```
make COMMAND
```
Similar commands are provided, usage of the commands:

 * ** make html** (re)generate the web site '
 * ** make clean** remove the generated files '
 * ** make regenerate**                  regenerate files upon modification '
 * ** make publish**                     generate using production settings '
 * ** make serve**                       serve site at http://localhost:8000'
 * ** make devserver**                   start/restart develop_server.sh '
 * ** make stopserver**                  stop local server '
 * ** ssh_upload**                       upload the web site via SSH '
 * ** rsync_upload**                     upload the web site via rsync+ssh '
 * ** dropbox_upload**                   upload the web site via Dropbox '
 * ** ftp_upload**                       upload the web site via FTP '
 * ** s3_upload**                        upload the web site via S3 '
 * ** github**                           upload the web site ( to evaimg.github.com)'


###Note
In order to upload to github you should ***clone evaimg.github.io repository in the same directory*** with this one. For more detailed information, you can open the file named pmake.cmd and Makefile.



