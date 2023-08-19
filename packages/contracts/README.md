## Mumbai Network へのデプロイコマンド

```bash
cd packages/contracts && pnpm run deploy:mumbai
```

## Latice Testnetへのデプロイコマンド

```bash
cd packages/contracts && pnpm run deploy:testnet
```

## 秘密鍵に基づいているBurnerWalletアドレス情報

[0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266 - mumbai](https://mumbai.polygonscan.com/address/0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266)  

[0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266 - Latice Testnet](https://explorer.testnet-chain.linfra.xyz/address/0xf39Fd6e51aad88F6F4ce6aB8827279cffFb92266) 

## デプロイしたWorldContractのアドレス情報

[0x1d83781da0787A5d0Fe1ced3fe55f0CB62e99ED9 - Latice Testnet](https://explorer.testnet-chain.linfra.xyz/address/0x1d83781da0787A5d0Fe1ced3fe55f0CB62e99ED9)

## MODE を使って情報を取得する API リクエスト

- mumbai の場合

```bash
grpcurl -plaintext -d '{"chainTables": [], "worldTables": [], "namespace": {"chainId":"80001", "worldAddress": "0x0b90377Db497D52F580896AC4Af8b4Bc2b7CFEd2"}}' localhost:8545 mode.QueryLayer/StreamState
```

- local の場合

```bash

```

## World コントラクト

[0x2F9aD9440cBd077352aEBA8A6610E62a3F4d903B](https://mumbai.polygonscan.com/address/0x2F9aD9440cBd077352aEBA8A6610E62a3F4d903B)

## 向き先を任意のブロックチェーンに変更するためのコマンド

```bash
cd packages/client && pnpm vite
```

## Worldコントラクトに暗号資産を送金した時のトランザクション

[0xf9bfd5c1b32596215e677dd9a36456cfa2d228c17f792d31cfde41c1788e45eb - Latice testnet](https://explorer.testnet-chain.linfra.xyz/tx/0xf9bfd5c1b32596215e677dd9a36456cfa2d228c17f792d31cfde41c1788e45eb)

### 参考文献

1. [Using MODE](https://v2.mud.dev/mode)