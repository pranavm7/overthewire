---
description: U r uniq
---

# Level 9

{% embed url="https://overthewire.org/wargames/bandit/bandit9.html" %}

The challenge here is to find the password that appears only once in `data.txt` &#x20;

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption><p>Sample data from data.txt</p></figcaption></figure>

Here we will use a bash pipe '|' to redirect the output of one command as input for the second command.

We will use two commands to get the result, namely `sort` and `uniq`&#x20;

Sort will sort the lines inside data.txt in an orderly fashion, which will then be passed onto uniq to delete duplicates. We will use the `-u` option in uniq to find unique lines instead of groupings of words.

Therefore the resultant command is as follows:

```bash
sort data.txt|uniq -u
```

This gives us the password as follows:

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption><p>Result</p></figcaption></figure>
