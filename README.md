# ipfs.pics

**(Notice January 2020) ipfs.pics is currently unmaintained. Nowadays, you can use the [ipfs companion](https://github.com/ipfs-shipyard/ipfs-companion) to share pictures with the world. It's just as easy to use, it is more decentralized, and it even works with any types of files!**

[ipfs.pics](https://ipfs.pics/) is a open-source and distributed image hosting website.
It aims to be an alternative to non-libre image hosting websites such as imgur, flickr and others.

It is based on [IPFS - the InterPlanetary File System](https://github.com/ipfs/ipfs). 
The whole application runs on the concept of peer to peer connections, which means that instead of 
hosting the information in a single location, our servers, the data is stored by everyone who wants to. 
When a picture is put on IPFS, it is given a hash, a 46 characters long digital fingerprint. 
No other file will have it and if the same file is added twice then their hashes will be exactly the same, 
which means the picture can still be found on the network simply by knowing the hash, even if our website is down. 
You can find the hash at the end of a picture URL, just like below. 

https://ipfs.pics/QmX7mna7G3BLx2UCdAHviaDastbnvLiVmM2pQ5azBa1H7D

https://ipfs.io/ipfs/QmX7mna7G3BLx2UCdAHviaDastbnvLiVmM2pQ5azBa1H7D

We saw potential in that application for an image hosting website, where you can know for sure your pictures 
will be available forever.

[Hacker News post about this](https://news.ycombinator.com/item?id=10436792). 

# FAQ

You can open an issue if you have a question not listed here.

## Can I install ipfs.pics on my own server?

Yes you can! You can do whatever you want with the code, as long as you give a link to your code to your users. See the licence for more details. You only need to do two easy steps to start hacking on this project:

1. Install [docker compose](https://docs.docker.com/compose/install/)

2. Run `docker-compose up` and everything ipfs.pics needs will be started

You're done! ipfs.pics is running on http://localhost:5000

## What stops people from adding a bunch of junk on ipfs until the network is full?

IPFS does not work like that. Each computer is responsible for what it chooses to make available to the rest of the network, and you can't force a computer to store something it doesn't want to store. We make sure that everything you upload to the official ipfs.pics instance is distributed on multiple computers. We have also heard of a few people who redirect to their own instance to make sure the content they care about stays alive. 

If it's still unclear, you can learn more about IPFS [here](https://github.com/ipfs/ipfs). 

# Licence

This program is free software: you can redistribute it and/or modify
    it under the terms of the [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.html) as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

The program also contains the following libraries:

* jQuery under the [MIT licence](https://github.com/jquery/jquery/blob/master/LICENSE.txt).

* jQuery UI under the [MIT licence](https://github.com/jquery/jquery-ui/blob/master/LICENSE.txt).

* Bootstrap under the [MIT licence](https://github.com/twbs/bootstrap/blob/master/LICENSE).

* FontAwesome under the [MIT licence + SIL](https://fortawesome.github.io/Font-Awesome/license/).
