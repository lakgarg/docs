---
slug: /reference/sdk.standarderc20.transfer
title: StandardErc20.transfer property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# StandardErc20.transfer property

Transfer Tokens

## Example

```javascript
// Address of the wallet you want to send the tokens to
const toAddress = "0x...";
// The amount of tokens you want to send
const amount = 0.1;
await contract.transfer(toAddress, amount);
```

**Signature:**

````typescript
transfer: {
        (to: string, amount: string | number): Promise<Omit<{
            receipt: import("@ethersproject/abstract-provider").TransactionReceipt; /**
             * Get Token Balance for the currently connected wallet
             *
             * @remarks Get a wallets token balance.
             *
             * @example
             * ```javascript
             * const balance = await contract.balance();
             * ```
             *
             * @returns The balance of a specific wallet.
             */
            data: () => Promise<unknown>;
        }, "data">>;
        prepare: (to: string, amount: string | number) => Promise<Transaction<Omit<{
            receipt: import("@ethersproject/abstract-provider").TransactionReceipt; /**
             * Get Token Balance for the currently connected wallet
             *
             * @remarks Get a wallets token balance.
             *
             * @example
             * ```javascript
             * const balance = await contract.balance();
             * ```
             *
             * @returns The balance of a specific wallet.
             */
            data: () => Promise<unknown>;
        }, "data">>>;
    };
````

## Remarks

Transfer tokens from the connected wallet to another wallet.