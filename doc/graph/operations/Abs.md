# Abs {#dev_guide_op_abs}

## General

Abs operation performs element-wise the absolute value with given tensor, it
applies following formula on every element of \src tensor (the variable names
follow the standard @ref dev_guide_conventions):

\f[ dst = \begin{cases} src & \text{if}\ src \ge 0 \\
    -src & \text{if}\ src < 0 \end{cases} \f]

## Operation attributes

Abs operation does not support any attribute.

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

Abs operation supports the following data type combinations.

Src | Dst
-- | --
f32 | f32
f16 | f16
bf16 | bf16
