---
slug: /reference/sdk.contractdeployer.deploytoken
title: ContractDeployer.deployToken property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# ContractDeployer.deployToken property

Deploys a new Token contract

## Example

```javascript
const contractAddress = await sdk.deployer.deployToken({
  name: "My Token",
  primary_sale_recipient: "your-address",
});
```

**Signature:**

```typescript
deployToken: {
        (metadata: TokenContractDeployMetadata): Promise<string>;
        prepare: (metadata: TokenContractDeployMetadata) => Promise<DeployTransaction>;
    };
```

## Remarks

Deploys a Token contract and returns the address of the deployed contract