---
description: Checklist
---

# Level 6

{% embed url="https://overthewire.org/wargames/bandit/bandit6.html" %}

Now we have certain properties of the file we are trying to find:

* human-readable
* 1033 bytes in size
* not executable

Seems like `find` command would be hugely helpful here. We know that the file will be readable, and that it has 1033 bytes inside. I did not focus on the not executable here since it did not seem like a critical requirement initially. However, the following command addresses all the requirements.

```bash
find . -type f -size 1033c -readable ! -executable
```

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

And we find the password to the next level.
