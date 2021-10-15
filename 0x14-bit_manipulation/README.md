0x14. C - Bit manipulation

Ø Computers represent all data internally as sequences of bits.

Ø Each bit can assume the value 0 or the value 1.

Ø The bitwise operators are used to manipulate the bits of integral operands both signed and unsigned.

Unsigned integers are normally used with the bitwise operators.

Ø Bitwise manipulations are machine dependent.

& Binary AND Operator copies a bit to the result if it exists in both operands.

(A & B) will give 12 which is 0000 1100

| Binary OR Operator copies a bit if it exists in eather operand.

(A | B) will give 61 which is 0011 1101

^ Binary XOR Operator copies the bit if it is set in one operand but not both.

(A ^ B) will give 49 which is 0011 0001

~ Binary Ones Complement Operator is unary and has the efect of 'flipping' bit.

(~A ) will give -60 which is 1100 0011

<< Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand.

A << 2 will give 240 which is 1111 0000

Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand.

A >> 2 will give 15 which is 0000 1111