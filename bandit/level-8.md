---
description: Millionaire
---

# Level 8

{% embed url="https://overthewire.org/wargames/bandit/bandit8.html" %}

The password is next to the word 'millionth' in `data.txt` file. Here is a quick look at data.txt to gain context of the challenge:

<figure><img src="../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>data.txt excerpt</p></figcaption></figure>

Instead of scrolling through the file endlessly, we can use `grep`!&#x20;

{% hint style="info" %}
Use `man grep` to learn more about the usage examples and options the command offers.
{% endhint %}

The command would be as follows:

```bash
grep <keyword> <filename>
# Result
grep millionth data.txt
```

And the output is as follows:

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>grep result</p></figcaption></figure>
