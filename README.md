# CAESAR CIPHER:

The Caesar cipher, named after Julius Caesar, is a simple substitution cipher used in cryptography. It is one of the earliest and most basic encryption techniques. The Caesar cipher works by shifting the letters of the alphabet by a fixed number of places.

# ENCRYPTION:

Choose a shift value, known as the key. Let's say the key is 3 and replace each letter in the plaintext with a letter found by moving n positions forward in the alphabet.

For Example:
              To Encrypt the word "HELLO" with a shift of 3.
"H" becomes "K" "E" becomes "H" "L" becomes "O" "L" becomes "O" "O" becomes "R".

So, "HELLO" becomes "KHOOR"

# DECRYPTION:

To decrypt shift the letters back by the same number of positions.
Example: Decrypt "KHOOR" with a shift of 3. "K" becomes "H" "H" becomes "E" "O" becomes "L" "O" becomes "L" "R" becomes "O".

So, "KHOOR" becomes "HELLO".

# EXAMPLE:

Plaintext: "HELLO" Shift: 3 (k=3) Encrypting "HELLO":

'H' -> 'K' 'E' -> 'H' 'L' -> 'O' 'L' -> 'O' 'O' -> 'R' So, "HELLO" encrypts to "KHOOR".

Decrypting "KHOOR" with the same shift (3):

'K' -> 'H' 'H' -> 'E' 'O' -> 'L' 'O' -> 'L' 'R' -> 'O'
