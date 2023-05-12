---
slug: /reference/sdk.splitinitializer
title: SplitInitializer variable
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# SplitInitializer variable

**Signature:**

```typescript
SplitInitializer: {
  name: "Split";
  contractType: "split";
  schema: {
    deploy: import("zod").ZodObject<
      {
        name: import("zod").ZodString;
        description: import("zod").ZodOptional<import("zod").ZodString>;
        image: import("zod").ZodOptional<
          import("zod").ZodUnion<
            [
              import("zod").ZodUnion<
                [
                  import("zod").ZodTypeAny,
                  import("zod").ZodObject<
                    {
                      data: import("zod").ZodUnion<
                        [import("zod").ZodTypeAny, import("zod").ZodString]
                      >;
                      name: import("zod").ZodString;
                    },
                    "strip",
                    import("zod").ZodTypeAny,
                    {
                      name: string;
                      data?: any;
                    },
                    {
                      name: string;
                      data?: any;
                    }
                  >,
                ]
              >,
              import("zod").ZodString,
            ]
          >
        >;
        external_link: import("zod").ZodOptional<import("zod").ZodString>;
        app_uri: import("zod").ZodOptional<import("zod").ZodString>;
        recipients: import("zod").ZodEffects<
          import("zod").ZodDefault<
            import("zod").ZodArray<
              import("zod").ZodObject<
                {
                  address: import("zod").ZodUnion<
                    [
                      import("zod").ZodType<
                        string,
                        import("zod").ZodTypeDef,
                        string
                      >,
                      import("zod").ZodType<
                        `0x${string}`,
                        import("zod").ZodTypeDef,
                        `${string}.eth` | `${string}.cb.id`
                      >,
                    ]
                  >;
                  sharesBps: import("zod").ZodNumber;
                },
                "strip",
                import("zod").ZodTypeAny,
                {
                  address: string;
                  sharesBps: number;
                },
                {
                  address: string;
                  sharesBps: number;
                }
              >,
              "many"
            >
          >,
          {
            address: string;
            sharesBps: number;
          }[],
          | {
              address: string;
              sharesBps: number;
            }[]
          | undefined
        >;
        trusted_forwarders: import("zod").ZodDefault<
          import("zod").ZodArray<
            import("zod").ZodUnion<
              [
                import("zod").ZodType<string, import("zod").ZodTypeDef, string>,
                import("zod").ZodType<
                  `0x${string}`,
                  import("zod").ZodTypeDef,
                  `${string}.eth` | `${string}.cb.id`
                >,
              ]
            >,
            "many"
          >
        >;
      },
      "strip",
      import("zod").ZodTypeAny,
      {
        name: string;
        trusted_forwarders: string[];
        recipients: {
          address: string;
          sharesBps: number;
        }[];
        description?: string | undefined;
        image?: any;
        external_link?: string | undefined;
        app_uri?: string | undefined;
      },
      {
        name: string;
        description?: string | undefined;
        image?: any;
        external_link?: string | undefined;
        app_uri?: string | undefined;
        recipients?:
          | {
              address: string;
              sharesBps: number;
            }[]
          | undefined;
        trusted_forwarders?: string[] | undefined;
      }
    >;
    output: import("zod").ZodObject<
      {
        name: import("zod").ZodString;
        description: import("zod").ZodOptional<import("zod").ZodString>;
        image: import("zod").ZodOptional<import("zod").ZodString>;
        external_link: import("zod").ZodOptional<import("zod").ZodString>;
        app_uri: import("zod").ZodOptional<import("zod").ZodString>;
        recipients: import("zod").ZodArray<
          import("zod").ZodObject<
            {
              address: import("zod").ZodUnion<
                [
                  import("zod").ZodType<
                    string,
                    import("zod").ZodTypeDef,
                    string
                  >,
                  import("zod").ZodType<
                    `0x${string}`,
                    import("zod").ZodTypeDef,
                    `${string}.eth` | `${string}.cb.id`
                  >,
                ]
              >;
              sharesBps: import("zod").ZodNumber;
            },
            "strip",
            import("zod").ZodTypeAny,
            {
              address: string;
              sharesBps: number;
            },
            {
              address: string;
              sharesBps: number;
            }
          >,
          "many"
        >;
      },
      "strip",
      import("zod").ZodUnknown,
      import("zod").objectOutputType<
        {
          name: import("zod").ZodString;
          description: import("zod").ZodOptional<import("zod").ZodString>;
          image: import("zod").ZodOptional<import("zod").ZodString>;
          external_link: import("zod").ZodOptional<import("zod").ZodString>;
          app_uri: import("zod").ZodOptional<import("zod").ZodString>;
          recipients: import("zod").ZodArray<
            import("zod").ZodObject<
              {
                address: import("zod").ZodUnion<
                  [
                    import("zod").ZodType<
                      string,
                      import("zod").ZodTypeDef,
                      string
                    >,
                    import("zod").ZodType<
                      `0x${string}`,
                      import("zod").ZodTypeDef,
                      `${string}.eth` | `${string}.cb.id`
                    >,
                  ]
                >;
                sharesBps: import("zod").ZodNumber;
              },
              "strip",
              import("zod").ZodTypeAny,
              {
                address: string;
                sharesBps: number;
              },
              {
                address: string;
                sharesBps: number;
              }
            >,
            "many"
          >;
        },
        import("zod").ZodUnknown,
        "strip"
      >,
      import("zod").objectInputType<
        {
          name: import("zod").ZodString;
          description: import("zod").ZodOptional<import("zod").ZodString>;
          image: import("zod").ZodOptional<import("zod").ZodString>;
          external_link: import("zod").ZodOptional<import("zod").ZodString>;
          app_uri: import("zod").ZodOptional<import("zod").ZodString>;
          recipients: import("zod").ZodArray<
            import("zod").ZodObject<
              {
                address: import("zod").ZodUnion<
                  [
                    import("zod").ZodType<
                      string,
                      import("zod").ZodTypeDef,
                      string
                    >,
                    import("zod").ZodType<
                      `0x${string}`,
                      import("zod").ZodTypeDef,
                      `${string}.eth` | `${string}.cb.id`
                    >,
                  ]
                >;
                sharesBps: import("zod").ZodNumber;
              },
              "strip",
              import("zod").ZodTypeAny,
              {
                address: string;
                sharesBps: number;
              },
              {
                address: string;
                sharesBps: number;
              }
            >,
            "many"
          >;
        },
        import("zod").ZodUnknown,
        "strip"
      >
    >;
    input: import("zod").ZodObject<
      {
        name: import("zod").ZodString;
        description: import("zod").ZodOptional<import("zod").ZodString>;
        image: import("zod").ZodOptional<
          import("zod").ZodUnion<
            [
              import("zod").ZodUnion<
                [
                  import("zod").ZodTypeAny,
                  import("zod").ZodObject<
                    {
                      data: import("zod").ZodUnion<
                        [import("zod").ZodTypeAny, import("zod").ZodString]
                      >;
                      name: import("zod").ZodString;
                    },
                    "strip",
                    import("zod").ZodTypeAny,
                    {
                      name: string;
                      data?: any;
                    },
                    {
                      name: string;
                      data?: any;
                    }
                  >,
                ]
              >,
              import("zod").ZodString,
            ]
          >
        >;
        external_link: import("zod").ZodOptional<import("zod").ZodString>;
        app_uri: import("zod").ZodOptional<import("zod").ZodString>;
        recipients: import("zod").ZodEffects<
          import("zod").ZodDefault<
            import("zod").ZodArray<
              import("zod").ZodObject<
                {
                  address: import("zod").ZodUnion<
                    [
                      import("zod").ZodType<
                        string,
                        import("zod").ZodTypeDef,
                        string
                      >,
                      import("zod").ZodType<
                        `0x${string}`,
                        import("zod").ZodTypeDef,
                        `${string}.eth` | `${string}.cb.id`
                      >,
                    ]
                  >;
                  sharesBps: import("zod").ZodNumber;
                },
                "strip",
                import("zod").ZodTypeAny,
                {
                  address: string;
                  sharesBps: number;
                },
                {
                  address: string;
                  sharesBps: number;
                }
              >,
              "many"
            >
          >,
          {
            address: string;
            sharesBps: number;
          }[],
          | {
              address: string;
              sharesBps: number;
            }[]
          | undefined
        >;
      },
      "strip",
      import("zod").ZodTypeAny,
      {
        name: string;
        recipients: {
          address: string;
          sharesBps: number;
        }[];
        description?: string | undefined;
        image?: any;
        external_link?: string | undefined;
        app_uri?: string | undefined;
      },
      {
        name: string;
        description?: string | undefined;
        image?: any;
        external_link?: string | undefined;
        app_uri?: string | undefined;
        recipients?:
          | {
              address: string;
              sharesBps: number;
            }[]
          | undefined;
      }
    >;
  }
  roles: readonly["admin"];
  initialize: (
    network: NetworkInput,
    address: string,
    storage: ThirdwebStorage<
      import("@thirdweb-dev/storage").IpfsUploadBatchOptions
    >,
    options?:
      | {
          supportedChains?:
            | {
                rpc: string[];
                chainId: number;
                nativeCurrency: {
                  symbol: string;
                  name: string;
                  decimals: number;
                };
                slug: string;
              }[]
            | undefined;
          thirdwebApiKey?: string | undefined;
          alchemyApiKey?: string | undefined;
          infuraApiKey?: string | undefined;
          readonlySettings?:
            | {
                rpcUrl: string;
                chainId?: number | undefined;
              }
            | undefined;
          gasSettings?:
            | {
                maxPriceInGwei?: number | undefined;
                speed?: "standard" | "fast" | "fastest" | undefined;
              }
            | undefined;
          gasless?:
            | {
                openzeppelin: {
                  relayerUrl: string;
                  relayerForwarderAddress?: string | undefined;
                  useEOAForwarder?: boolean | undefined;
                  domainName?: string | undefined;
                  domainVersion?: string | undefined;
                };
                experimentalChainlessSupport?: boolean | undefined;
              }
            | {
                biconomy: {
                  apiId: string;
                  apiKey: string;
                  deadlineSeconds?: number | undefined;
                };
              }
            | undefined;
          gatewayUrls?: string[] | undefined;
        }
      | undefined,
  ) => Promise<import("./prebuilt-implementations/split").Split>;
  getAbi: (
    address: Address,
    provider: ethers.providers.Provider,
    storage: ThirdwebStorage,
  ) =>
    Promise<
      | import("zod").objectOutputType<
          {
            type: import("zod").ZodString;
            name: import("zod").ZodDefault<import("zod").ZodString>;
            inputs: import("zod").ZodDefault<
              import("zod").ZodArray<
                import("zod").ZodObject<
                  {
                    type: import("zod").ZodString;
                    name: import("zod").ZodDefault<import("zod").ZodString>;
                    stateMutability: import("zod").ZodOptional<
                      import("zod").ZodString
                    >;
                    components: import("zod").ZodOptional<
                      import("zod").ZodArray<
                        import("zod").ZodObject<
                          {
                            type: import("zod").ZodString;
                            name: import("zod").ZodDefault<
                              import("zod").ZodString
                            >;
                          },
                          "strip",
                          import("zod").ZodAny,
                          import("zod").objectOutputType<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            import("zod").ZodAny,
                            "strip"
                          >,
                          import("zod").objectInputType<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            import("zod").ZodAny,
                            "strip"
                          >
                        >,
                        "many"
                      >
                    >;
                  },
                  "strip",
                  import("zod").ZodAny,
                  import("zod").objectOutputType<
                    {
                      type: import("zod").ZodString;
                      name: import("zod").ZodDefault<import("zod").ZodString>;
                      stateMutability: import("zod").ZodOptional<
                        import("zod").ZodString
                      >;
                      components: import("zod").ZodOptional<
                        import("zod").ZodArray<
                          import("zod").ZodObject<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            "strip",
                            import("zod").ZodAny,
                            import("zod").objectOutputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >,
                            import("zod").objectInputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >
                          >,
                          "many"
                        >
                      >;
                    },
                    import("zod").ZodAny,
                    "strip"
                  >,
                  import("zod").objectInputType<
                    {
                      type: import("zod").ZodString;
                      name: import("zod").ZodDefault<import("zod").ZodString>;
                      stateMutability: import("zod").ZodOptional<
                        import("zod").ZodString
                      >;
                      components: import("zod").ZodOptional<
                        import("zod").ZodArray<
                          import("zod").ZodObject<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            "strip",
                            import("zod").ZodAny,
                            import("zod").objectOutputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >,
                            import("zod").objectInputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >
                          >,
                          "many"
                        >
                      >;
                    },
                    import("zod").ZodAny,
                    "strip"
                  >
                >,
                "many"
              >
            >;
            outputs: import("zod").ZodDefault<
              import("zod").ZodArray<
                import("zod").ZodObject<
                  {
                    type: import("zod").ZodString;
                    name: import("zod").ZodDefault<import("zod").ZodString>;
                    stateMutability: import("zod").ZodOptional<
                      import("zod").ZodString
                    >;
                    components: import("zod").ZodOptional<
                      import("zod").ZodArray<
                        import("zod").ZodObject<
                          {
                            type: import("zod").ZodString;
                            name: import("zod").ZodDefault<
                              import("zod").ZodString
                            >;
                          },
                          "strip",
                          import("zod").ZodAny,
                          import("zod").objectOutputType<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            import("zod").ZodAny,
                            "strip"
                          >,
                          import("zod").objectInputType<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            import("zod").ZodAny,
                            "strip"
                          >
                        >,
                        "many"
                      >
                    >;
                  },
                  "strip",
                  import("zod").ZodAny,
                  import("zod").objectOutputType<
                    {
                      type: import("zod").ZodString;
                      name: import("zod").ZodDefault<import("zod").ZodString>;
                      stateMutability: import("zod").ZodOptional<
                        import("zod").ZodString
                      >;
                      components: import("zod").ZodOptional<
                        import("zod").ZodArray<
                          import("zod").ZodObject<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            "strip",
                            import("zod").ZodAny,
                            import("zod").objectOutputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >,
                            import("zod").objectInputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >
                          >,
                          "many"
                        >
                      >;
                    },
                    import("zod").ZodAny,
                    "strip"
                  >,
                  import("zod").objectInputType<
                    {
                      type: import("zod").ZodString;
                      name: import("zod").ZodDefault<import("zod").ZodString>;
                      stateMutability: import("zod").ZodOptional<
                        import("zod").ZodString
                      >;
                      components: import("zod").ZodOptional<
                        import("zod").ZodArray<
                          import("zod").ZodObject<
                            {
                              type: import("zod").ZodString;
                              name: import("zod").ZodDefault<
                                import("zod").ZodString
                              >;
                            },
                            "strip",
                            import("zod").ZodAny,
                            import("zod").objectOutputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >,
                            import("zod").objectInputType<
                              {
                                type: import("zod").ZodString;
                                name: import("zod").ZodDefault<
                                  import("zod").ZodString
                                >;
                              },
                              import("zod").ZodAny,
                              "strip"
                            >
                          >,
                          "many"
                        >
                      >;
                    },
                    import("zod").ZodAny,
                    "strip"
                  >
                >,
                "many"
              >
            >;
          },
          import("zod").ZodAny,
          "strip"
        >[]
      | (
          | {
              inputs: never[];
              stateMutability: string;
              type: string;
              anonymous?: undefined;
              name?: undefined;
              outputs?: undefined;
            }
          | {
              anonymous: boolean;
              inputs: {
                indexed: boolean;
                internalType: string;
                name: string;
                type: string;
              }[];
              name: string;
              type: string;
              stateMutability?: undefined;
              outputs?: undefined;
            }
          | {
              inputs: {
                internalType: string;
                name: string;
                type: string;
              }[];
              name: string;
              outputs: {
                internalType: string;
                name: string;
                type: string;
              }[];
              stateMutability: string;
              type: string;
              anonymous?: undefined;
            }
          | {
              stateMutability: string;
              type: string;
              inputs?: undefined;
              anonymous?: undefined;
              name?: undefined;
              outputs?: undefined;
            }
        )[]
    >;
}
```