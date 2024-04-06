-- Tiny Tapeout Signed/unsigned nxn-bit multiplier (VHDL files)

-- 4-bit signed/unsigned multiplicand
-- 4-bit signed/unsigned multiplier
-- 8-bit signed/unsigned product
-- Signed_mode selects data type for both operands and result

-- The unsigned combinational multiplier uses a nxn array of full-adders plus product bits and
-- final stage of ripple-carry full-adders for the upper half of the product.

-- The signed (2's complement) version employs the Baugh-Wooley multiplier
-- algorithm, which avoids sign-extension by flipping MSBs of both operands
-- (cancel out for cell that combine MSBs of both operands), and adding ones
-- at the least and most significant bit positions of the ripple-carry adder.
