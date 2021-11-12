redeploying the contract

Starting deployment. Account id: dev-1636742726472-62450935830753, node: https://rpc.testnet.near.org, helper: https://helper.testnet.near.org, file: ./build/release/lottery.wasm
Transaction Id DmpcYn67r4y562YCyDwtT4HYiWcy4WS1yGX7MpuKn2Gz
To see the transaction in the transaction explorer, please open this url in your browser
https://explorer.testnet.near.org/transactions/DmpcYn67r4y562YCyDwtT4HYiWcy4WS1yGX7MpuKn2Gz
Done deploying to dev-1636742726472-62450935830753
--------------------------------------------
run the following commands

export CONTRACT=__new_contract_account_id__
near call $CONTRACT init '{"owner":"'$OWNER'"}' --accountId $CONTRACT


export OWNER=dev-1636742726472-62450935830753                                     
export OWNER=hryer2.testnet
export CONTRACT=dev-1636742726472-62450935830753
export PLAYER=hryer2.testnet
near call $CONTRACT init '{"owner":"'$OWNER'"}' --accountId $CONTRACT 
Scheduling a call: dev-1636742726472-62450935830753.init({"owner":"hryer2.testnet"})
Doing account.functionCall()
Transaction Id CqD3fXFbiWZSc5Avfx5DJvHkLAEcbpJy6QYn5KfYeK3F
To see the transaction in the transaction explorer, please open this url in your browser
https://explorer.testnet.near.org/transactions/CqD3fXFbiWZSc5Avfx5DJvHkLAEcbpJy6QYn5KfYeK3F
''
➜  NCD.L1.sample--lottery git:(main) ✗ ./scripts/2.play.sh 

About to call play() on the contract
near call $CONTRACT play --account_id $PLAYER --amount $1

$CONTRACT is dev-1636742726472-62450935830753
$PLAYER is hryer2.testnet
$1 is [ NEAR ] (the optionally attached amount)

Scheduling a call: dev-1636742726472-62450935830753.play()
Doing account.functionCall()
Receipt: H4DyktgfpG6L6b2gh3ht285GxfDGkTSbKuRAwFuqy6LH
	Log [dev-1636742726472-62450935830753]: roll: 2190347208
	Log [dev-1636742726472-62450935830753]: hryer2.testnet did not win.  The pot is currently 1 NEAR
Transaction Id C4fp734boKy34aaHNj3YpLmzABoChE4ruc6NjYeK1eXU
To see the transaction in the transaction explorer, please open this url in your browser
https://explorer.testnet.near.org/transactions/C4fp734boKy34aaHNj3YpLmzABoChE4ruc6NjYeK1eXU
''