# Getting into CTFs: Day 2

Today, I focused on learning some cool cryptography things.

## ASCII

ASCII is a system for encoding characters. There are 256 ASCII characters in total (but the first 128 are most commonly used), each labelled with a ASCII Value from 0 to 255. To convert from ASCII in Python, we can use the function `chr()`. This function takes an integer i and returns a string representing the Unicode (Unicode is a superset of ASCII–where ASCII has a more limited characters set, mostly used for English, Unicode is more universal. Hence, _Uni(versal Character en)code(ing system)_!) character that has the code point i. 

On the other hand, `ord()` takes a character and gives you the ASCII value for it.

## Hexadecimal

Sometimes, text is encoded in hexadecimal (base 16). In order to decode this to something we can read, we use the `bytes.fromhex()` function from python, which takes a hex string and converts it to bytes. Bytes are groups of 8 binary digits (bits) and each byte can represent integers from 0 to 127 (so, it can represent the first 128 ASCII characters!). 

For example, if we want to decode this: 6E657264, we would run
```
bytes.fromhex("6E657264")
```
which returns `b'nerd'`! The prefix "b" indicates that it's a byte literal as opposed to a string literal.
