
## **Useful commands**

List all keys

```
gaiad keys list
```

Find out the address
~~~
gaiad keys show Atlas.Node -a
~~~

How to find out address and voloperaddress using explorer?

Open the validator and click on the transaction at the bottom in the Transactions section.

## **Balance**

gaiad query bank balances [address]

```
gaiad query bank balances cosmos19xu32g7ev7wwj6ktzuekwr5tdggh4zm50p4889
```
## **Delegate tokens to validator**
gaiad tx staking delegate <TO_VALOPER_ADDRESS> 1000000uatom --from wallet --chain-id school-testnet-4 --gas-adjustment 1.4 --gas auto --fees 2500uatom -y
```
gaiad tx staking delegate cosmosvaloper19xu32g7ev7wwj6ktzuekwr5tdggh4zm524pjtk 1000000uatom --from yuri-reserv --chain-id school-testnet-4 --gas-adjustment 1.4 --gas auto --fees 0utom -y
```
