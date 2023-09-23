
## **Useful commands**

Edit existing validator
```
gaiad tx staking edit-validator \
--new-moniker "Atlas.Node" \
--chain-id school-testnet-4 \
--from cosmos1nu40yhxxwrht2v2ujnch3asruhk87ttx796g3v
```

List all keys

```
gaiad keys list
```

Find out the address
~~~
gaiad keys show Atlas.Node -a
~~~

How to find out address and voloperaddress using explorer? Open the validator and click on the transaction at the bottom in the Transactions section.


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

## **Governance**

Query proposals
```
gaiad query gov proposals
```

View Proposal By ID
```
gaiad query gov proposal 1
```

Vote YES for proposal 1
```
gaiad tx gov vote 1 yes --from mykey
```

Query votes on a proposal 1

```
gaiad query gov votes 1
```
