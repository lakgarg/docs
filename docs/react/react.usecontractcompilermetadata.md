---
slug: /react.usecontractcompilermetadata
title: useContractCompilerMetadata() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useContractCompilerMetadata() function

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

Use this to get the publish metadata for a deployed contract.

## Example

```javascript
const {
  data: compilerMetadata,
  isLoading,
  error,
} = useContractCompilerMetadata("{{contract_address}}");
```

**Signature:**

```typescript
export declare function useContractCompilerMetadata(
  contractAddress: RequiredParam<ContractAddress>,
): import("react-query").UseQueryResult<PublishedMetadata | undefined, unknown>;
```

## Parameters

| Parameter       | Type                                                                                           | Description                          |
| --------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------ |
| contractAddress | [RequiredParam](./react.requiredparam.md)&lt;[ContractAddress](./react.contractaddress.md)&gt; | the address of the deployed contract |

**Returns:**

import("react-query").UseQueryResult&lt;PublishedMetadata \| undefined, unknown&gt;

a response object that includes the published metadata (name, abi, bytecode) of the contract