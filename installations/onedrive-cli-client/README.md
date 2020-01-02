*Guide for installing OneDrive CLI client on linux*

Install curl and git\
`$ sudo apt install libcurl4-openssl-dev git`

Install Development files for sqlite3\
`$ sudo apt install libsqlite3-dev`

Using the classic security policy install dmd (Compiler for the D programming language) and dub (Build tool for projects written in D)\
`$ sudo snap install --classic dmd && sudo snap install --classic dub`

Clone the git repo with the software\
`$ git clone https://github.com/abraunegg/onedrive.git`

Compile and install\
`$ cd onedrive
./configure
make
sudo make install` 

Authorize onedrive with Microsoft\
`$ onedrive`
A windows will open, type in your creadentials\

Once this is done, you will be presented with a blank white page. Copy the URL and paste it into the Terminal at the prompt\

To start syncronizing the folder start the service\
`$ onedrive --synchronize`

To have it monitor for changes continuesly you can do\
`$ onedrive --monitor`
This command can be added to your startup programs