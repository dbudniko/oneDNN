# Log {#dev_guide_op_log}

## General

Log operation performs element-wise natural logarithm operation with given 
tensor, it applies following formula on every element of \src tensor (the 
variable names follow the standard @ref dev_guide_conventions):

\f[ dst = \log(src) \f]

## Operation attributes

Log operation does not support any attribute.

## Execution arguments

The inputs and outputs must be provided according to below index order when
constructing an operation.

### Inputs

Index | Argument Name | Required or Optional
-- | -- | --
0 | `src` | Required

### Outputs

Index | Argument Name | Required or Optional
-- | -- | --
0 | `dst` | Required

## Supported data types

Log operation supports the following data type combinations.

Src | Dst
-- | --
f32 | f32
f16 | f16
bf16 | bf16