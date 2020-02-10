*Installation of JRE*

Download correct JRE version from this site\
`https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html`

Move to directory of installation choice\
`$ cd /usr/java`

Move the downloaded file to the new directory, may require sudo. Remember to choose correct filename for jre\
`$ sudo mv /home/$USER/Downloads/jre-* /usr/java/`

Unpach the file\
`$ sudo tar zxvf jre-*`

Add $JAVA_HOME to your path variables, remember to correct jre version\
Add the line `export JAVA_HOME=/usr/java/jre*` to your bashrc file