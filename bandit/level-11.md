---
description: B64 decoded.
---

# Level 11

{% embed url="https://overthewire.org/wargames/bandit/bandit11.html" %}

The data is encoded in [Base64](https://en.wikipedia.org/wiki/Base64) which we'll need to decode in order to get the password. It is important to distinguish that there is a difference between encryption and encoding.

If data is encrypted, we have to crack the encryption or need a password. However, since it is encoded, we can simply decode the data.

The `data.txt` has the following data:

<figure><img src="../.gitbook/assets/image (14).png" alt=""><figcaption><p>Encoded data</p></figcaption></figure>

And in order to decode it, we simply pass it to base64 command with `-d` argument to decode it

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption><p>Decoded data</p></figcaption></figure>

