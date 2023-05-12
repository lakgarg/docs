---
slug: /reference/sdk.contractdeployer.deploymarketplace
title: ContractDeployer.deployMarketplace property
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# ContractDeployer.deployMarketplace property

Deploys a new Marketplace contract

## Example

```javascript
const contractAddress = await sdk.deployer.deployMarketplace({
  name: "My Marketplace",
  primary_sale_recipient: "your-address",
});
```

**Signature:**

```typescript
deployMarketplace: {
        (metadata: MarketplaceContractDeployMetadata): Promise<string>;
        prepare: (metadata: MarketplaceContractDeployMetadata) => Promise<DeployTransaction>;
    };
```

## Remarks

Deploys a Marketplace contract and returns the address of the deployed contract