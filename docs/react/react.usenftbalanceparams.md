---
slug: /react.usenftbalanceparams
title: useNFTBalanceParams type
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useNFTBalanceParams type

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

The params to pass to `useNftBalance`.

**Signature:**

```typescript
export declare type useNFTBalanceParams<TContract> = TContract extends Erc1155
  ? [
      contract: RequiredParam<TContract>,
      ownerWalletAddress: RequiredParam<WalletAddress>,
      tokenId: RequiredParam<BigNumberish>,
    ]
  : [
      contract: RequiredParam<TContract>,
      ownerWalletAddress: RequiredParam<WalletAddress>,
    ];
```

**References:** [RequiredParam](./react.requiredparam.md), [WalletAddress](./react.walletaddress.md)