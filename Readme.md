<p>Commands related to web3.js</p>
 <ul>
    <li>
        <h3>1. To install web3</h3>
        <p>npm install --save web3</p>
    </li>
    <li>
        <h3>2. To import web3</h3>
        <p>let Web3 = require("web3");</p>
    </li>
    <li>
        <h3>3. To connect with Ganache</h3>
        <p>let web3 = new Web3(new Web3.providers.HttpProvider("HTTP://127.0.0.1:7545"));</p>
    </li>
    <li>
        <h3>4. To get the balance of an account.</h3>
        <p>web3.eth.getBalance("paste the address of the account inside it").then(console.log);</p>
    </li>
    <li>
        <h3>5. To convert wei into ether.</h3>
        <p>web3.eth.getBalance("address").then(function(result){console.log(web3.utils.fromWei(result,""ether"));})</p>
    </li>
    <li>
        <h3>6. To transfer ether from one account to another.</h3>
        <p>web3.eth.sendTransaction({from:"address1", to:"address2",value:web3.utils.toWei("5","ether")});</p>
    </li>
 </ul>

 <p>Interacting with Smart Contract</p>
 <ul>
    <li>
        <h3>1. To call a function.</h3>
        <p>contracts.methods.x().call().then(console.log);</p>
    </li>
    <li>
        <h3>To set a function</h3>
        <p>contract.methods.set(90).send({from:"address"});</p>
    </li>
 </ul>

 <p>Using browser to interact with smart contract</p>
 <ul>
    <li>
        <h3>Step 1:</h3>
        <p>Go to terminal and type "npm install web3.js-browser"</p>
    </li>
    <li>
        <h3>Step 2:</h3>
        <p>Create an index.html file and add "<script src="node_modules/web3.js-browser/build/web3.js"></script>" and then start the live server.</p>
    </li>
    <li>
        <h3>Step 3:</h3>
        <p>Go to console from "Developer Tools" and type "let web3 = new Web3(new Web3.providers.HttpProvider("HTTP://127.0.0.1:7545"));"</p>
    </li>
    <li>
        <h3>Step 4:</h3>
        <p>Type in console "web3.eth.getAccounts().then(console.log);"</p>
    </li>
 </ul>

 <p>Generating ABI and Bytecode using web3.js</p>
 <ul>
    <li>
        <h3>Step 1:</h3>
        <p>Install packages "npm install fs solc web3"</p>
    </li>
    <li>
        <h3>Step 2:</h3>
        <p>Create a folder and create two files inside it, named as "demo.sol" and "web_new.js". You will get the code from the repository.</p>
    </li>
    <li>
        <h3>Step 3:</h3>
        <p>Type "node web_new.js" and generate ABI and Bytecode.</p>
    </li>
 </ul>

 <p>Deployment of Smart Contract</p>
 <ul>
    <li>
        <h3>Step 1:</h3>
        <p>Write the deployment code on "web_new.js" file</p>
    </li>
    <li>
        <h3>Step 2:</h3>
        <p>Type "node web_new.js" and deploy your contract using Ganache.</p>
    </li>
 </ul>