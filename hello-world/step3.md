## Test Your smart contract

The stage is set. Your contract is on disk, lets build with docker so that we can test the contract as it would be run by a real live Dragonchain.

`docker build myContract/src -t my-contract`{{execute}}

Now that the contract is built, we can run it using DCTL!

If all goes according to plan, this demo contract will count up from 1 to infinity, reading from what we call "heap." the Heap is a key value store of data. Under the hood, it's just redis and S3, but when this thing runs on a dragonchain it will also be on the blockchain, getting verifications from dragonnet.

Lets try invoking it locally.

`dctl contract test my-contract:latest --payload "Hello, World!" --test-directory ./myContract/test`{{execute}}

The output should show that the call-count is 1.

Subsequent runs should count up, try it again:

`dctl contract test my-contract:latest --payload "Get schwifty!" --test-directory ./myContract/test`{{execute}}
