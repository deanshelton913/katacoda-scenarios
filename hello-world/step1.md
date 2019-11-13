First things first.

## Get up to date!

Lets make sure we have atleast version 10 on NodeJS.

`node --version`{{execute}}

8!? Thats pretty old. Lets update to the latest LTS version of nodeJS (v12) to be sure we are supported.

Try using this command to update:

`curl -sL https://deb.nodesource.com/setup_12.x | bash && apt-get install nodejs`{{execute}}


After that's done, lets confirm the version is now high enough to support installing DCTL.

`node --version`{{execute}}

12 :D Nice...


That does it for the environment.

Next we will install the commandline tool which will help us build our smart contracts on the blockchain.
