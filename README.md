# Unexpected NaN due to Loose Comparison with Null and Undefined

This code demonstrates a common JavaScript error related to loose comparison (==) when dealing with null and undefined values.

The function `foo` intends to return 0 if the input `x` is null, and `x + 1` otherwise. However, using loose comparison, `undefined == null` evaluates to true, leading to an incorrect result when `undefined` is passed as an argument. This results in `undefined + 1`, which evaluates to `NaN`.

The solution demonstrates the proper use of strict equality (===) to distinguish between null and undefined, ensuring the correct behavior.