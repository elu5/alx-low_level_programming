0x0C. C - More malloc, free

It makes your code more portable between C and C++, and as SO experience shows a great many programmers claim they are writing in C when they are really writing in C++ (or C plus local compiler extensions).

Failing to do so can hide an error: note all the SO examples of confusing when to write type * versus type **.

The idea that it keeps you from noticing you failed to #include an appropriate header file misses the forest for the trees. It's the same as saying "don't worry about the fact you failed to ask the compiler to complain about not seeing prototypes -- that pesky stdlib.h is the REAL important thing to remember!" It forces an extra cognitive cross-check. It puts the (alleged) desired type right next to the arithmetic you're doing for the raw size of that variable. I bet you could do an SO study that shows that malloc() bugs are caught much fasterwhen there's a cast. As with assertions, annotations that reveal intent decrease bugs.

Repeating yourself in a way that the machine can check is often a great idea. In fact, that's what an assertion is, and this use of cast is an assertion. Assertions are still the most general technique we have for getting code correct, since Turing came up with the idea so many years ago.