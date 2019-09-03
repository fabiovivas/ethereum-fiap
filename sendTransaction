function depositar(value, address){
    var from = eth.accounts[0];
    var valueTo = web3.toWei(value);
    var transaction = {from: from, to: address, value: valueTo};

    var result = {
        beforeValue: web3.fromWei(eth.getBalance(address).toString(), "ether"),
        transactionHash: eth.sendTransaction(transaction),
        afterValue: web3.fromWei(eth.getBalance(address).toString(), "ether")
    };

    return result;
}
