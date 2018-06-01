# Secure EOS Block Producers Voting

URL: https://tokenika.github.io/secure-bp-voting/

## Single Page Voting

Much simpler way to vote, but if your computer was infected by some virus/keylogger in the past, this way cannot guarantee full security.

1. [Simple voting for block producers](https://tokenika.github.io/secure-bp-voting/1_vote.html)

## More secure voting, without a need to use your private key on device being online

This way is more complicated, but it gives you maximum security. The process is divided into 3 steps:

1. [Fetching information about the network](https://tokenika.github.io/secure-bp-voting/1_get_blockchain_data.html)
2. [Generating and signing transaction with your private key](https://tokenika.github.io/secure-bp-voting/2_generate_transaction.html) (you can do this offline, for example with a computer which was never connected to the internet)
3. [Pushing transaction to the network](https://tokenika.github.io/secure-bp-voting/3_push_transaction.html)

Both solutions are based on [eosjs library](https://github.com/eosio/eosjs).

Secure EOS Block Producers Voting is an open-source software created by [Tokenika.io](https://tokenika.io/) - an EOS block producer candidate.

Source code is available at https://github.com/tokenika/secure-bp-voting on [MIT Licence](LICENSE).

**We encourage EOS community to audit our code or improve!**