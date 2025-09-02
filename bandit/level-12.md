---
description: Rot13
---

# Level 12

{% embed url="https://overthewire.org/wargames/bandit/bandit12.html" %}

The challenge has all the lowercase and uppercase alphabets rotated by 13. This is a common encryption ciphers primarily used in CTFs called [Caesar cipher](https://en.wikipedia.org/wiki/Caesar_cipher). Lets take a look.

### Steps

1. We use the `cat` command to read the contents of the file `data.txt`\


<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

2. The we can copy the text and use an online rot13 decoder, I used [dcode.fr](https://www.dcode.fr/caesar-cipher)&#x20;

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

3. Pressing the decrypt button we get the password!

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Congrats! Onto the next adventure.
