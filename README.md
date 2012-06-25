# My Hubot

This is a version of GitHub's hubot. He's pretty cool.
I make some configs and tailor it to Gtalk.
I have selected serveral hubot-scripts from the enormous amount of them. Feel free to clone
the version if you take interest in hubot. Or to do better, click the [root_hubot](https://github.com/github/hubot)

## how to run
The dependancies are put in the json file. However, it seems to use pretty mach npms, parts of
them need to compile native libraries. In ubuntu, run the commands at first:

```shell
sudo apt-get install libexpat1 libexpat1-dev
sudo apt-get install libicu-dev 

```
then to install npms
```
npm install
```

at last, prepare a file(.source) filling the context followed:

```
export HUBOT_GTALK_USERNAME="xxx@gmail.com"
export HUBOT_GTALK_PASSWORD="yyyyyy"
export HUBOT_GTALK_WHITELIST_USERS=""
```

Now, you can run the hubot.

```
source .source
hubot/bin/hubot -a gtalk
```

If you see something like `undefined`, the most possible reason is that you input the login and password uncorrectly。
Please check them.

