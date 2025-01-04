# encryption-decryption-tool
**Features**
Vigenère Cipher Integration: Introduces a classical encryption mechanism for specific rounds.
Custom S-Box Transformation: Ensures strong substitution operations.
Permutation Tables: Provides diffusion by rearranging bits.
Additive Cipher Key: A placeholder to simulate additional security without impacting the algorithm's core functionality.
Loop Support: Enables multiple encryption and decryption operations within a single session.

**User Input**
Plaintext: multiple of 8-character ASCII string for encryption.
Ciphertext: 64-bit binary string for decryption.
128-bit Key: Binary key used for encryption and decryption.
Vigenère Key: String key used in specific rounds of the algorithm.
Additive Cipher Key: Integer key asked during input (not currently implemented in logic).

_**Workflow**_

**Encryption:**
Convert plaintext to a 64-bit binary string.
Apply initial permutation.
Split into left and right halves.
Perform 8 rounds of transformations:
Expand the right half.
XOR with round keys.
Substitute using the S-Box.
Integrate Vigenère cipher in later rounds.
Permute the result.
Swap left and right halves.
Apply the final permutation to generate the ciphertext.

**Decryption:**
Reverse the encryption steps using the same keys.
Validate and decode the binary string into plaintext.

**License**
This algorithm is for educational purposes. Use responsibly.
