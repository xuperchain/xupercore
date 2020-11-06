# xuperos

面向公链应用场景设计的区块链执行引擎。

## 组件说明

reader: 只读组件。采用读写分离设计，降低代码复杂度。

ledger: 统一收敛账本变更操作（交易、同步块、创世块修改等）。

contract: 系统合约，考虑到系统合约和链强相关，放到引擎中实现，注册到合约组件。

## 应用案例

超级链开放网络。

    Init()
    Start()
    Stop()
    ProcessTx()
    ProcessBlock()
    QueryTx()
    QueryForbiddenTx()
    QueryBlock()
    QueryBlockByHeight()
    ChainState()
    QueryMethodACL()
    QueryAccountACL()
    ListAccount()
    ListUtxo()
    Balance()
    FrozenBalance()
    BalanceDetail()
    PreExec()
    ListContract()
    ContractState()