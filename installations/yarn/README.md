*Guide for installing yarn on linux*

Install Curl\
`$ sudo apt-get install curl`

Add PPA to system\
`$ curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -`

Add PPA to sources list\
`$ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list`

Install yarn\
`$ sudo apt update && sudo apt install yarn` 