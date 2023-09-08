SA3

Display a Blockchain
=====================


In this activity, you will learn to display the blockchain.




<video src= "https://s3.amazonaws.com/media-p.slid.es/videos/1525749/EVpcfxt-/sa3.mp4" width = "480" height = "320"></video>




Follow the given steps to complete this activity:
1. Create and append a new block to the blockchain.


* Open the file app.py.


* Pass the length of the chain as the index of the block.


    `'index': len(chain.chain),`


* Open the file index.html from the templates folder.


* Pass transaction information (sender, receiver and amount) to the toggelInfoSection() function.


    `'{{block.transaction['sender']}}',
    '{{block.transaction['receiver']}}',
    '{{block.transaction['amount']}}'`


* Receive the transaction information sent from the web form by adding parameters sender, receiver, amount to the toggleInfoSection() function.
 
    `function toggleInfoSection(index, timestamp, currentHash, previousHash, sender, receiver, amount)`


* Add the data to the respective fields.


    `document.getElementById('senderData').innerHTML = sender
    document.getElementById('receiverData').innerHTML = receiver
    document.getElementById('amountData').innerHTML = amount`


* Save and run the code to check the output.