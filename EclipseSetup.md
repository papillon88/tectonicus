To set up Eclipse to download the project and upload a new build:

1. Install eclipse

2. Installl the [subclipse svn plugin for eclipse](http://subclipse.tigris.org/). You should be able to do that via 'help' -> 'Install new software' in Eclipse

3. Go to the 'svn repositories' perspective and right click and do 'new... repository location'

4. Enter the address of the project repository (see http://code.google.com/p/tectonicus/source/checkout) It should be https://tectonicus.googlecode.com/svn

5. Expand the new repository, then expand the 'trunk' dir so you see the 'tectonicus' dir.

6. Right click 'tectonicus' and do 'checkout...'

This should pull down the whole project as an already configured eclipse project.

Switch back to the 'java perspective' to actually do your work. And you should be able to right click the project and do 'team' -> 'update' to get the latest from the repository, or 'team->commit' to submit your changes.

You'll need your google code password (https://code.google.com/hosting/settings).

For 'svnversion' you need the svn client tools: http://subversion.apache.org/packages.html

Once you've got all of that you should be able to run the ant script to compile and upload a new version (make sure to change the version number in the ant file first).