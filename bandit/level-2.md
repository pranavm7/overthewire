---
description: >-
  The password for the next level is stored in a file called - located in the
  home directory
---

# Level 2

{% embed url="https://overthewire.org/wargames/bandit/bandit2.html" %}

Running the same ls command as before got us different results.

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>listing all files at home dir</p></figcaption></figure>

Here we will output the contents of the file

```bash
cat ./-
```

Then the password revealed that can be used to bandit2!

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

