# Secure EOS Block Producers Voting

This is in best interest of whole EOS community, to select block producers rather sooner than later. Network will not be fully activated if at least 15% of tokens won't vote. Without fully activated network, people will not be able to transfer any funds. At the same time we expect than many bad actors will try to exploit inexperienced users, by providing many tools which could steal your funds.

That's why Tokenika decided to release a tool, to give people a possibility to vote being OFFLINE, with no risk of exposing your private keys.

URL: https://tokenika.github.io/secure-bp-voting/

## 1. Simple online voting (not recommended)

Very simpler way to vote, but if your computer was infected by some virus/keylogger in the past, this way cannot guarantee full security.

1. [Simple voting for block producers](https://tokenika.github.io/secure-bp-voting/1_vote.html)

We do not recommend this way, but we release it, because it can be useful in some cases, for example for voting on a testnet.

## 2. Secure OFFLINE voting (recommended), without a need to use your private key on device being online

This way is a little bit more complicated, but it gives you maximum security. The process is divided into 3 steps:

1. [Fetching information about the network](https://tokenika.github.io/secure-bp-voting/1_get_blockchain_data.html)
2. [Generating and signing transaction with your private key](https://tokenika.github.io/secure-bp-voting/2_generate_transaction.html) (you can do this OFFLINE, for example with a computer which was never connected to the internet)
3. [Pushing transaction to the network](https://tokenika.github.io/secure-bp-voting/3_push_transaction.html)

## 3. Voting Using the Command Line (for advanced users)
Of course, there is also a way, to vote with tools provided by Block One. The easiest way to do that require installation of docker. EOS New York recently published very good and detail instruction how this can be done. We can recommend [their article](https://steemit.com/eos/@eosnewyork/your-vote-matters-3-eos-block-producer-voting-using-the-command-line) to all people, which know how to use docker and have some basic command line skills.


# How to build eos.js on your own

First and second solutions are based on [eosjs library](https://github.com/eosio/eosjs).

Our plan was, to not include `eos.js` in our repository and just use a version 13.0.0:

    <script src="https://github.com/EOSIO/eosjs/releases/download/v13.0.0/eos.js"></script>

 
which was released in official repository [here](https://github.com/EOSIO/eosjs/releases/tag/v13.0.0). Thanks to that you would not have to trust our eos.js file.

However the problem appeared when Block One decided to release new version of eos.js (13.1.0), without uploading new build version of eos.js to [released bundle](https://github.com/EOSIO/eosjs/releases/tag/v13.1.0) :(

So, we [created an issue on official github](https://github.com/EOSIO/eosjs/issues/153) hopping that they will build and upload newest trusted version of eos.js, so every developer would be able hot-link to it.

But in the meantime, we have been forced to build latest eos.js on our own, so we could publish our solution.

**Important**: there is no requirement for your, to trust `eos.js` build by us. We encourage you, to build it on your own, according to [provided official instruction](https://github.com/EOSIO/eosjs#browser): 

    git clone https://github.com/EOSIO/eosjs.git
    cd eosjs
    npm install
    npm run build_browser
    # builds: ./dist/eos.js


# About

Secure EOS Block Producers Voting is an open-source software created by [Tokenika.io](https://tokenika.io/) - an EOS block producer candidate.

Source code is available at https://github.com/tokenika/secure-bp-voting on [MIT Licence](LICENSE).

**We encourage EOS community to audit our code or improve it!**