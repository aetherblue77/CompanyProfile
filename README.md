# CompanyProfile
Belajar GIT Dasar, Materi Sync

```javascript
function fund() public payable {
        // want to be able to set a minimum fund amount in USD
        // 1. How do we send ETH to this contract??

        require(msg.value.getConversionRate() >= MINIMUM_USD, "Didn't Send Enough!!"); // 1e18 == 1 * 10^18 == 1000000000000000000
        // 18 Decimals --> 1 Ether == 10^18 Wei

        funders.push(msg.sender);
        addressToAmoundFunded[msg.sender] += msg.value; 

    }
```
