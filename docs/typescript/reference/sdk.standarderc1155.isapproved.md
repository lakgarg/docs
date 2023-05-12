---
slug: /reference/sdk.standarderc1155.isapproved
title: StandardErc1155.isApproved() method
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# StandardErc1155.isApproved() method

Get whether this wallet has approved transfers from the given operator

**Signature:**

```typescript
isApproved(address: AddressOrEns, operator: AddressOrEns): Promise<boolean>;
```

## Parameters

| Parameter | Type                                  | Description          |
| --------- | ------------------------------------- | -------------------- |
| address   | [AddressOrEns](./sdk.addressorens.md) | the wallet address   |
| operator  | [AddressOrEns](./sdk.addressorens.md) | the operator address |

**Returns:**

Promise&lt;boolean&gt;