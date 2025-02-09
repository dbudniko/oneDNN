# TypeCast {#dev_guide_op_typecast}

## General

TypeCast operation performs element-wise cast from input data type to the data
type given by output tensor. It requires that \src and \dst have the same shape
and layout. Rounding to nearest even will be used during cast.

## Operation attributes

TypeCast operation does not support any attribute.

## Execution arguments

The inputs and outputs must be provided according to below index order when
constructing an operation.

### Inputs

Index | Argument Name | Required or Optional
-- | -- | --
0|`src` | Required

### Outputs

Index | Argument Name | Required or Optional
-- | -- | --
0|`dst` |Required

## Supported data types

TypeCast operation supports the following data type combinations.

Src | Dst
-- | --
bf16, f16  |f32
f32 | bf16, f16

@note This operation is to support
[mixed precision](@ref dev_guide_graph_mixed_precision_model) computation.
