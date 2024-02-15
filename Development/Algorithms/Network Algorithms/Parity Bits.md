For every group of bits, a singular bit named the "parity bit" is added. If the number of '1' bits in the group is odd then the parity bit will be one, and zero otherwise (Even parity).

If the number of '1' bits in the group is even then the parity bit will be zero, and one other wise (odd parity).

# Why does this work?

If any bit, either data or parity, changes then the rule of having an Even or Odd number of '1's will not be satisfied. Therefore, 1-bit error can be detected using this method.

![[Pasted image 20240212163346.png]]