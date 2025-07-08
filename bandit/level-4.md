---
description: Hidden Files
---

# Level 4

{% embed url="https://overthewire.org/wargames/bandit/bandit4.html" %}

On level 3, we see the simple folder  named _inhere._

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

When we check the listing for the directory _inhere_, it does not reveal any information. Does this mean that the folder is empty? Not necessarily; lets use additional flags on the command to show all the files present. We will use the `-la` flag which enables long-listing all files.

<figure><img src="../.gitbook/assets/image (5) (1).png" alt=""><figcaption><p>Utilizing the flags for the command</p></figcaption></figure>

and therefore we can simply use the cat command to find the flag.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
