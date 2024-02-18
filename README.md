# NeighborParkingSmartContract
neighborhood parking lot smart contract to reallocate rights and profits.

## 合约规则

假设你家小区有一些私人拥有的停车位，当车位暂时不用时，可以用于临时出租创收。

NFT market：每个车位都是一个NTF，唯一标记车位位置，车位所有人可以将自己的私人车位mint NFT，当车位闲置时可以对车位定价并将其挂到NFT市场，出租给需要的人。
租客：当需要租用车位时，可以购买NFT，并抵押一定数量的币，结束租用时，归还NFT给车位所有人，付停车费并收回抵押的币。支持预约


链下可以配合车位地锁，地图导航等技术，这里不做探讨，认为租用和归还车位都由租客触发，通过前端页面调用合约。
