# JS_Assesment-_Metacraft

This code represents a simple NFT system that mints unique digital assets with metadata, stores them in an array, and provides functions to display and track the total supply of NFTs.

This code represents a simple NFT system that mints unique digital assets with metadata, stores them in an array, and provides functions to display and track the total supply of NFTs.

## Description

This code defines a simple system for minting, storing, and listing NFTs (Non-Fungible Tokens) in JavaScript. Each NFT contains basic metadata like a name, eye color, shirt type, and bling, which are stored in an array. The program also includes functions to mint new NFTs, display their metadata, and print the total number of NFTs created.

## Getting Started

### Executing program

To run this program, you can use Remix, an online Java Script Compiler. To get started, go to the Remix website at [https://remix.ethereum.org/](https://www.programiz.com/javascript/online-compiler/).

Write your code on this website and run your code.

```javascript
const NFTs = [];

function mintNFT(name, eyecolor, shirtType, bling) {
  const NFT = {
    name: name,
    eyecolor: eyecolor,
    shirtType: shirtType,
    bling: bling,
  };
  NFTs.push(NFT);
  console.log("Minted \t" + name);
}

function listNFTs() {
  for (let i = 0; i < NFTs.length; i++) {
    console.log("\nID: \t\t" + (i + 1));
    console.log("Name: \t\t" +NFTs[i].name);
    console.log("Eyecolor: \t" +NFTs[i].eyecolor);
    console.log("Shirt Type:\t" +NFTs[i].shirtType);
    console.log("Bling: \t\t" +NFTs[i].bling);
  }
}

function getTotalSupply() {
  console.log("\n", +NFTs.length);
}


mintNFT("Tushar", "black", "shirt full sleeve", " Gold bracelet");
mintNFT("Deepesh", "grey", "Hoodie", "Gold chain");
mintNFT("Harsh", "blue", "Jacket", "Ear ring");
mintNFT("Amit", "brown", "Hoodie", "Silver bracelet");
listNFTs();
getTotalSupply();

```



## Authors

Tushar Srivastav 



## License

This project is licensed under the MIT License - see the LICENSE.md file for details

