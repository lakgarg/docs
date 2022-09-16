---
slug: /sdk.tokenimpl._constructor_
title: TokenImpl.(constructor)
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## TokenImpl.(constructor)

Constructs a new instance of the `TokenImpl` class

**Signature:**

```typescript
constructor(network: NetworkOrSignerOrProvider, address: string, storage: IStorage, options: {
        readonlySettings?: {
            chainId?: number | undefined;
            rpcUrl: string;
        } | undefined;
        gasSettings?: {
            maxPriceInGwei?: number | undefined;
            speed?: "standard" | "fast" | "fastest" | undefined;
        } | undefined;
        gasless?: {
            experimentalChainlessSupport?: boolean | undefined;
            openzeppelin: {
                relayerForwarderAddress?: string | undefined;
                relayerUrl: string;
            };
        } | {
            biconomy: {
                deadlineSeconds?: number | undefined;
                apiId: string;
                apiKey: string;
            };
        } | undefined;
    } | undefined, abi: typeof ABI, contractWrapper?: ContractWrapper<TokenERC20>);
```

## Parameters

| Parameter       | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | Description       |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- |
| network         | [NetworkOrSignerOrProvider](./sdk.networkorsignerorprovider.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |                   |
| address         | string                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |                   |
| storage         | IStorage                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |                   |
| options         | { readonlySettings?: { chainId?: number &#124; undefined; rpcUrl: string; } &#124; undefined; gasSettings?: { maxPriceInGwei?: number &#124; undefined; speed?: "standard" &#124; "fast" &#124; "fastest" &#124; undefined; } &#124; undefined; gasless?: { experimentalChainlessSupport?: boolean &#124; undefined; openzeppelin: { relayerForwarderAddress?: string &#124; undefined; relayerUrl: string; }; } &#124; { biconomy: { deadlineSeconds?: number &#124; undefined; apiId: string; apiKey: string; }; } &#124; undefined; } &#124; undefined |                   |
| abi             | typeof ABI                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                   |
| contractWrapper | ContractWrapper&lt;TokenERC20&gt;                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | <i>(Optional)</i> |