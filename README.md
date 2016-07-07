# Lua-TLS
A custom version of TLS for Computercraft. See [the specification](/specification.txt) for more details.

## Implementation status
Please note that some functions may not have been publicly released despite being implemented.
* RSAES-OAEP-ENCRYPT - Untested
  * MGF1 - Untested
    * SHA-1 - Untested
    * CONCATENATE - Verified
  * XOR - Untested
  * MODPOW - Untested
    * MULTIPLY - Untested
    * MODULUS - Untested
      * FLOORDIV - Verified
        * ADD - Verified
        * SUBTRACT - Assumed
        * COPYTABLE - Assumed
        * COMPARE
      * COMPARE - Verified
  * RESIZE - Verified
  * SHA-1
  * CONCATENATE
* RSAES-OAEP-DECRYPT - Untested
  * SPLIT - Untested
  * MGF1
  * SHA-1
  * CONCATENATE
  * XOR
  * RESIZE
  * MODPOW
  * COMPARE
* RSASSA-PSS-SIGN - Untested
  * EMSA-PSS-ENCODE - Untested
    * MGF1
    * SHA-1
    * CONCATENATE
    * XOR
  * RSASP1 - Untested
    * COMPARE
    * MODPOW
  * RESIZE
* RSASSA-PSS-VERIFY - Untested
  * EMSA-PSS-VERIFY - Untested
    * TEST-LEFTMOST-BITS - Untested
    * CLEAR-LEFTMOST-BITS - Untested
    * MGF1
    * SHA-1
    * CONCATENATE
    * XOR
    * SPLIT
  * RSAVP1 - Untested
    * MODPOW
  * RESIZE
* AES-CBC-ENCRYPT - Provided
* AES-CBC-DECRYPT - Provided
* SERIALIZE - Provided
* UNSERIALIZE - Provided
* TYPE - Provided

Other functions that may be provided by the API.
* GENERATE-KEYS - Untested
  * MODULAR-INV - Untested
  * SUBTRACT
  * MULTIPLY
* OPEN-CLIENT - Untested
  * RSAES-OAEP-ENCRYPT
  * RSAES-OAEP-DECRYPT
  * RSASSA-PSS-VERIFY
  * AES-CBC-ENCRYPT
  * AES-CBC-DECRYPT
  * SERIALIZE
  * UNSERIALIZE
* OPEN-SERVER - Unimplemented
  * RSAES-OAEP-ENCRYPT
  * RSAES-OAEP-DECRYPT
  * AES-CBC-ENCRYPT
  * AES-CBC-DECRYPT
  * SERIALIZE
  * UNSERIALIZE
