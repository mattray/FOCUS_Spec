# Usage Quantity

The Usage Quantity represents the volume of a given [*resource*](#glossary:resource) or [*service*](#glossary:service) used or purchased based on the [Usage Unit](#usageunit). Usage Quantity is often derived at a finer granularity or over a different time interval when compared to the [Pricing Quantity](#pricingquantity) (complementary to [Pricing Unit](#pricingunit)), and focuses on *resource* and *service* consumption, not pricing and cost.

UsageQuantity MUST be present in the billing data. This column MUST be of type Decimal and MUST conform to [Numeric Format](#numericformat). The value MAY be negative in cases where [ChargeSubcategory](#chargesubcategory) is "Refund". This column MUST NOT contain null values when [SkuPriceId](#skupriceid) is not null.

## Column ID

UsageQuantity

## Display name

Usage Quantity

## Description

Volume of a given *resource* or *service* used or purchased based on the [Usage Unit](#usageunit).

## Content constraints

| Constraint      | Value         |
|:----------------|:--------------|
| Column type     | Metric        |
| Column required | True          |
| Allows nulls    | True          |
| Data type       | Decimal       |
| Value format    | [Numeric Format](#numericformat) |
| Number range    | Any valid decimal value |

## Introduced (version)

1.0
