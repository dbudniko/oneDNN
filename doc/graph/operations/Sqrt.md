# Sqrt {#dev_guide_op_sqrt}

## General

Sqrt operation performs element-wise square root operation with given tensor.

## Operation attributes

Sqrt operation does not support any attribute.

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

Sqrt operation supports the following data type combinations.

Src | Dst
-- | --
f32 | f32
f16 | f16
bf16 | bf16