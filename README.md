Genesis Block Generator
=======================

Original post https://bitcointalk.org/index.php?topic=181981.0 

Compile:
--------
```bash
  gcc generator.c -o generator -lcrypto
```
Usage:
------
  generator &lt;pubkey&gt; &lt;timestamp&gt; &lt;nBits&gt;
  
Example:
--------
```bash
./generator 04678afdb0fe5548271967f1a67130b7105cd6a828e03909a67962e0ea1f61deb649f6bc3f4cef3 8c4f35504e51ec112de5c384df7ba0b8d578a4c702b6bf11d5f "The Times 03/Jan/2009 Chancellor on brink of second bailout for banks" 486604799
```
Output:
-------
```bash
Coinbase: 04ffff001d0104455468652054696d65732030332f4a616e2f32303039204368616e63656c6c6f7 2206f6e206272696e6b206f66207365636f6e6420
6261696c6f757420666f722062616e6b73

PubkeyScript: 4104678afdb0fe5548271967f1a67130b7105cd6a828e03909a67962e0ea1f61deb649f6bc3f4ce f38c4f35504e51ec112de5c384df7ba0b8d57
8a4c702b6bf11d5fac

Merkle Hash: 3ba3edfd7a7b12b27ac72c3e67768f617fc81bc3888a51323a9fb8aa4b1e5e4a
Byteswapped: 4a5e1e4baab89f3a32518a88c31bc87f618f76673e2cc77ab2127b7afdeda33b
```
#To change:
unixtime = 1231006505 # set time 09/01/2009 and nonce = 2083236893 # for Bitcoin genesis block
