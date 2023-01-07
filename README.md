# Blockchain-Framework
A simple blockchain framework that allows mining, adding new transactions and viewing the chain

## Getting Started

Please install the following packages in comand prompt to begin:
* flask
  ```sh
  python pip install Flask==0.12.2
  ```
* requests
  ```sh
  python pip install requests==2.18.4 
  ```
I used three methods:
* Create a new transaction to a block
  ```sh
  /transactions/new
  ```
* Mine a new block
  ```sh
  /mine 
  ```
* Return the full Blockchain
  ```sh
  /chain
  ```
  You can use cURL or Postman to interact with the API over a network (I use Postman)
  
See below for example requests:

![Screenshot_20230107_140823](https://user-images.githubusercontent.com/112626017/211155041-66599607-a62c-449a-8a38-1c0c82807914.png)

* When sending data to the server send in JSON format something like this:
  ```sh
  {
 "sender": "d4ee26eee15148ee92c6cd394edd974e",
 "recipient": "address-2",
 "amount": 100
  }
  ``` ```
![Screenshot_20230107_140957](https://user-images.githubusercontent.com/112626017/211155044-b37a3760-7434-418d-9339-707ea2fc4313.png)
![Screenshot_20230107_141031](https://user-images.githubusercontent.com/112626017/211155046-9da2ad72-b522-4f62-9a81-8c47f679894f.png)

After this using two nodes (created manually using different ports or using different machines) you can use the below as a get method:
```sh
  /nodes/resolve
  ```
If one node has a chain that is longer, the shorter chain will get replaced by the Conensus Algorithm

### Contact!

- Connect on LinkedIn: Benjamin Holmes
- Project Link: https://github.com/holmesbenjamin/Blockchain-Framework
