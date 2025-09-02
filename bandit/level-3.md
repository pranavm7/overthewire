---
description: File with spaces!
---

# Level 3

{% embed url="https://overthewire.org/wargames/bandit/bandit3.html" %}

Herein, we must print the contents of the file containing spaces.

Running the same `ls` command we find:

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption><p>Bandit2 home dir</p></figcaption></figure>

We will escape the spaces in order for the file to be treated as one file, and not multiples.

```bash
cat spaces\ in\ this\ filename
# This directly outputs the password requried.
```

We can then use the password to move onto level 4!
