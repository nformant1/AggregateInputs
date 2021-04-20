# :rocket: Dogecoin: Aggregate Inputs

This script will take a number of UTXOs (defined in txcount) and will send/aggregate it to another address (defined in aggAddress).
The script will do 3 loops (defined in maxloops) and will wait 20 seconds (time.sleep(20)) after each transaction in send.

You need a dogecoin core wallet running for this script. It is okay to just have dogecoin-qt up and running. In my case I run "dogecoin-qt -testnet". 
Make sure your dogecoin.conf file matches the variables (rpcuser, rpcpassword, rpcport).

The fees seem to be calculated wrong (too high for big transactions) and probably in a suboptimal way, but they made it to the chain :chains:

:warning: This script comes with **absolutely no warranty!** I used it only on the testnet so far, any help and reviews are appreciated!

# :waning_gibbous_moon: Working script example
![Screenshot](https://github.com/nformant1/AggregateInputs/blob/main/script_in_action.png)

You see the txid as print-output in the script and it will appear in your tx list in your core wallet.
