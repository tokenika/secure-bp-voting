# Secure EOS Block Producers Voting

This is in best interest of whole EOS community, to select block producers rather sooner than later. Network will not be fully activated if at least 15% of tokens won't vote. Without fully activated network, people will not be able to transfer any funds. At the same time we expect than many bad actors will try to exploit inexperienced users, by providing many tools which could steal your funds.

That's why Tokenika decided to release a tool, to give people a possibility to vote being OFFLINE, with no risk of exposing your private keys.

URL: https://tokenika.github.io/secure-bp-voting/

## Simple online voting (not recommended)

Very simpler way to vote, but if your computer was infected by some virus/keylogger in the past, this way cannot guarantee full security.

1. [Simple voting for block producers](https://tokenika.github.io/secure-bp-voting/1_vote.html)

We do not recommend this way, but we release it, because it can be useful in some cases, for example for voting on a testnet.

## Secure OFFLINE voting (recommended), without a need to use your private key on device being online

This way is a little bit more complicated, but it gives you maximum security. The process is divided into 3 steps:

1. [Fetching information about the network](https://tokenika.github.io/secure-bp-voting/1_get_blockchain_data.html)
2. [Generating and signing transaction with your private key](https://tokenika.github.io/secure-bp-voting/2_generate_transaction.html) (you can do this OFFLINE, for example with a computer which was never connected to the internet)
3. [Pushing transaction to the network](https://tokenika.github.io/secure-bp-voting/3_push_transaction.html)

## Voting Using the Command Line (recommended for advanced users)

Of course, there is also a way, to vote with tools provided by Block One. The easiest way to do that require installation of docker. EOS New York recently published very good and detail instruction how this can be done. We can recommend [their article](https://steemit.com/eos/@eosnewyork/your-vote-matters-3-eos-block-producer-voting-using-the-command-line) to all people, which know how to use docker and have some basic command line skils.

------------

First and second solutions are based on [eosjs library](https://github.com/eosio/eosjs).

Secure EOS Block Producers Voting is an open-source software created by [Tokenika.io](https://tokenika.io/) - an EOS block producer candidate.

Source code is available at https://github.com/tokenika/secure-bp-voting on [MIT Licence](LICENSE).

**We encourage EOS community to audit our code or improve it!**