---
description: Compression all the way down.
---

# Level 13

{% embed url="https://overthewire.org/wargames/bandit/bandit13.html" %}

The challenge instructions are as follows:

The password for the next level is stored in the file **data.txt**, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

### Setup

First off, I wanted to ensure that I can work on this challenge without disturbing the original environment, so I chose to create a directory in the "tmp" root directory which is the temporary workspace, named it gr4y and copied the challenge over.

```
mkdir /tmp/gr4y
cp data.txt /tmp/gr4y
cd /tmp/gr4y/
```

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### Recon

On opening the data.txt file we see the hexdump as follows:

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

The text in this file can be interpreted as follows:

| Offset    | Hex data                                | Ascii Representation |
| --------- | --------------------------------------- | -------------------- |
| 00000000: | 1f8b 0808 84c9 8768 0203 6461 7461 322e | .......h..data2.     |

Which it repeats for the entire file. For the purpose of this challenge we will use the `xxd` tool which is very helpful for working with file data. If I run `xxd data.txt` it will output the data.txt file as a hex dump!



