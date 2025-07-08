---
description: Read a file!
---

# Level 1

{% embed url="https://overthewire.org/wargames/bandit/bandit1.html" %}
Level 0 -> Level 1 Hints @ OTW
{% endembed %}



We need to read a file that contains the password! Lets start by listing all the files in the current directory (folder).

```bash
# -a => All files
# -l => Long List (formats output)
ls -al
```

Here we see the _readme_ file mentioned on the OTW page.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption><p>Listing of home directory</p></figcaption></figure>

We will use the `cat` command to print the password:

```bash
cat ./readme
```

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Output of solution</p></figcaption></figure>

Then we simply type exit to exit the shell and reconnect as bandit1 and use the provided password

```bash
exit
ssh -p 2220 bandit1@bandit.labs.overthewire.org    
```

