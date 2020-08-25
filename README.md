# Blockchain for Beginners
### A dive into blockchain technology for those who know nothing about it (like me, previously).

Paper and sample code included. Paper [here](Paper.pdf). An example of a basic python blockchain implementation, specifically an implementation of a cryptocurrency called ZackCoin, is included as part of the paper, located [here](ZackCoin.py). This basic implementation uses many concepts discussed in the paper in an effort to further the understanding of blockchain technology. 

To run this code, ensure you have the `python`, `flask` and `requests` packages installed on your machine (`pip install <packageName>` to install a package within a terminal window). Download the files into a local directory and open up the directory in a terminal window. To run the Flash application, run `python ZackCoin.py`. Then in another terminal within the same directory, you can run `curl localhost:5000/transaction -H "Content-Type: application/json"-d '{"from": "<SomeString>", "to":"<SomeOtherString>", "amount": <SomeNumber>}'` to add a transaction to the network. Additionally, you can run `curl localhost:5000/mine` to mine a block for the most recent transaction, or if there isn’t one, just a general block. Finally, you can run `curl localhost:5000/AllZackCoins` to print out the contents of the entire blockchain. Relevant output will be printed for the other two commands as well.

