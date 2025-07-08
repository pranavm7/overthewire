---
description: Perm check 👀
---

# Level 7

{% embed url="https://overthewire.org/wargames/bandit/bandit7.html" %}

This is the excerpt from the [challenge](https://overthewire.org/wargames/bandit/bandit7.html)

```properties
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size
```

Seems like the `find` command from the last challenge can help us here as well!

Here is the command I crafted:

```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
# Command breakdown:
# -type f -> type of object is a file
# -user bandit7 -> object is owned by bandit7
# -group bandit6 -> object is owned by bandit6
# -size 33c -> object is 33 bytes in size
# 2>/dev/null -> 
```

This gives us a path that we can check with `ls -l` to verify the requirements are met and `cat` to print the password!

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>The output of the command crafted.</p></figcaption></figure>
