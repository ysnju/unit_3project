Why is 0.1+0.2 == 0.3 false for python?

Because of :binary represenation 
(-1)^sign * 2^-1-22 * 0.fraction

zero will look like

0 : 0 00000000000 0000000000000000000000000000000000000000000000000000

negative zero will look like

1 : 0 00000000000 0000000000000000000000000000000000000000000000000000

0.1 will look like

0 : 0 01111111{011} [1001100110011001100110011001100110011001100110011010]

0.2 will look like

0 : 0 01111111{100} [1001100110011001100110011001100110011001100110011010]

we can compare the bits of 0.1 and 0.2 , and find that they are almost identical, except for the parts in curly brackets.
This is because 0.1*2 is 0.2, and the bits there differenciate them. However, when we look at the bits in brackets, we can see that they are the exact same.
For 0.1 and 0.2, the binary bits in brackets are the exact same. This is due to the rounding done when the bits were cut off to represent the number in 52 bits shown on the screen.
This rounding error is why 0.1+0.2 has an slight difference from 0.3. 

```py
0.1 is 0.100000000000005551112312578 when 
print(f"{0.1:.06f}")

0.2 is 0.20000000000 when 
print(f"{0.1:.06f}")

0.3 is 0.29999999999999 when 
print(f"{0.1:.06f}")

print(f"{0.1+0.2:.06f}") is
0.300000000000

binary_representation = struct.pack('>d', number)
binary_representation = 

```

citation
James Murphy "0.1 + 0.2 is NOT 0.3 in Most Programming Languages" mCoding 2021
