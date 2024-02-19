# NeighborParkingSmartContract
neighborhood parking lot smart contract.
小区停车位智能合约

## smart contract rules

Assuming your residential community has privately owned parking spaces that can be temporarily rented out for additional income. Each parking space is represented by a non-fungible token (NFT) that uniquely identifies its location.

The owners of the parking spaces can mint NFTs for their private parking spaces. When a parking space becomes available for rent, the owner can set the rental price and list it on the NFT marketplace.

When a tenant wants to rent a parking space, they can purchase the corresponding NFT. At the end of the rental period, the tenant pays the parking fee and returns the NFT to the owner.

假设你家小区有一些私人拥有的停车位，当车位暂时不用时，可以用于临时出租创收。每个车位都是一个NTF，唯一标记车位位置。
车位所有人可以将自己的私人车位mint NFT，当车位闲置可出租时，对车位定价并将其挂到NFT市场。
租客需要租用车位时，可以购买NFT，结束租用时，支付停车费并归还NFT给车位所有人。
链下可以配合车位地锁，地图导航等技术，这里不做探讨，认为租用和归还车位都由租客触发，通过前端页面调用合约。

## smart contract design
### NFT 合约
创建 NFT，车位所有人将车位创建一个新的 NFT
销毁 NFT，车位用有人销毁 NFT
转移指定 NFT

### NFT market 合约
车位所有人上架NFT
车位所有人下架NFT
租客购买NFT，开始计时
查询需要支付的费用
租客归还NFT到NFT market，结束计时，支付租金给合约账户
合约支付90%收益给车位所有人

## backend api
查询当前market上架的所有 NFT
查询当前登录人拥有的车位，当前登陆人租用的车位，当前登陆人交易历史


## front end
创建NFT
销毁NFT
上架NFT
下架NFT
购买NFT
归还NFT，并支付
