# Overview

Tips Protocol allows everyone to create a currency, emit signed bills, and   
exchange them with peers in a decentralized manner.

For example a pizza store may emit 'pizza' currency, where each coin is worth
a pizza slice. Customers get a coin each time they buy a pizza.
Once a customer has collected 8 coins, they may pay them back to the pizza
store to get a whole pizza. They may also trade them to other users, eg. to
get 'sushi' coins instead.

# Glossary

- address: bitcoin address (we use bitcoin cryptography but we don't use blockchain)
- currency: a currency code, such as 'USD' + address of the emitent
- emitent: a user that emits currency using their private key
- tip: an amount of currency emitted by the emitent to some address
- holder: a user that currently has a tip(s) emitted to their address
- doc: a cryptographically signed JSON object
- emission: a doc declaring a new tip
- trasfer: a doc declaring an intent to transfer tip ownership to another holder
- split: a doc declaring an intent to split or merge tips of the same type and holder
- exchange: a doc describing an intent to exchange one set of tips for another. May involve many holders, emitents, and currencies.