Create an NFT Collection
Simple Overview of Use/Purpose
This project involves creating a simple NFT (Non-Fungible Token) collection using JavaScript. The program includes functions to mint new NFTs, list all created NFTs, and get the total supply of NFTs. This exercise helps in understanding how NFTs can be created and managed programmatically.

Description
In this project, you will develop a set of JavaScript functions to create and manage an NFT collection. You will create a variable to store the NFTs, a function to mint new NFTs with specified metadata, a function to list all NFTs, and a function to get the total number of minted NFTs. This project provides a fundamental understanding of managing NFT collections and metadata.

Getting Started
Installing
No installation is required for this project as it is a JavaScript-based project. You can use any JavaScript runtime environment like Node.js or a web browser console to run the code.

Executing Program
Create a new JavaScript file and name it nftCollection.js.

Copy and paste the following code into the file:

javascript
Copy code
// Create a variable to hold your NFTs
const NFTS = [];

// This function will take in some values as parameters, create an NFT object using the parameters passed to it for its metadata, and store it in the variable above.
function mintNFT(phoneNumber, displayName, statusMessage, lastSeen, isOnline, unreadMessages) {
    const NFT = {
        phoneNumber: phoneNumber,
        displayName: displayName,
        statusMessage: statusMessage,
        lastSeen: lastSeen,
        isOnline: isOnline,
        unreadMessages: unreadMessages,
    }
    console.log("Minted: " + displayName);
    NFTS.push(NFT);
}

// Create a 'loop' that will go through an 'array' of NFTs and print their metadata with console.log()
function listNFTS() {
    for (let i = 0; i < NFTS.length; i++) {
        console.table(NFTS[i]);
    }
}

// Print the total number of NFTs we have minted to the console
function getTotalSupply() {
    console.log("Total NFT's: " + NFTS.length);
}

// Call your functions below
mintNFT("1234567890", "Rajat Bodh", "Busy", "2024-05-30T14:48:00.000Z", true, 5);
mintNFT("0987654321", "Pramod", "Available", "2024-05-30T15:30:00.000Z", false, 0);
mintNFT("5556667777", "Shashi bhushan kumar", "At the gym", "2024-05-30T16:00:00.000Z", true, 12);
mintNFT("4445556666", "Yuvraj Singh", "In a meeting", "2024-05-30T14:15:00.000Z", false, 8);
mintNFT("3334445555", "Raj Bodh", "On vacation", "2024-05-30T17:20:00.000Z", true, 3);
mintNFT("2223334444", "Rahul kumar", "Offline", "2024-05-30T18:45:00.000Z", false, 10);

listNFTS();
getTotalSupply();
Run the program using a JavaScript runtime environment, such as Node.js, or by copying the code into a web browser console.

bash
Copy code
node nftCollection.js
Help
For common problems or issues:

Ensure your JavaScript runtime environment is properly set up.
Double-check the syntax for any typos or errors.
Make sure the functions are called correctly with the appropriate parameters.
For further assistance, you can refer to JavaScript documentation or seek help from online programming communities.

Authors
Contributors:

Rajat Bodh 
License
This project is licensed under the MIT License - see the LICENSE.md file for details.
