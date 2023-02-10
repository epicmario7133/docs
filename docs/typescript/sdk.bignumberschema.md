---
slug: /sdk.bignumberschema
title: BigNumberSchema variable
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## BigNumberSchema variable

**Signature:**

```typescript
BigNumberSchema: z.ZodEffects<
  z.ZodUnion<
    [
      z.ZodString,
      z.ZodNumber,
      z.ZodBigInt,
      z.ZodType<BigNumber, z.ZodTypeDef, BigNumber>,
    ]
  >,
  BigNumber,
  string | number | bigint | BigNumber
>;
```