This is your second step.

## Task

Now lets install the Dragonchain Commandline Tool.

`yarn global add dctl` {{execute}}


DCTL has many commands to help us interface with our dragonchain, and manipulate our smart contracts.

In future tutorials, we will even use DCTL to talk to other public blockchains like bitcoin and ethereum,
but for now we can just create our first smart contract.


Dragonchain supports any programming language for it's smart contract, but for this example lets choose
to create a new contract in using the language "nodejs". It's popular, and this contract is pretty well documented.

`dctl contract init --language node --dir myContract` {{execute}}
