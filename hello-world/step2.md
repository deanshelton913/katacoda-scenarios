## Get your dragonchain out of its shell

Now that the environment is set-up, lets install the Dragonchain commandline tool (DCTL)

`yarn global add dctl`{{execute}}

DCTL has many commands to help us interface with our dragonchain, and manipulate our smart contracts.

In future tutorials, we will even use DCTL to talk to other public blockchains like bitcoin and ethereum,
but for now we can just create our first smart contract.

`dctl contract init --language node --dir myContract`{{execute}}

> NOTE: Dont feel tied to nodejs. We could have chosen java, c#, golang or even bash! Checkout the docs for more information on supported languages.


