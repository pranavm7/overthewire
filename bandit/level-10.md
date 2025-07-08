# Level 10

{% embed url="https://overthewire.org/wargames/bandit/bandit10.html" %}

We are given a file with a bunch of data, but the hint is that the password is human readable preceeded by multiple '=' symbols.

Here's a sample of the data contained in the target `data.txt`

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

This can be simply solved by using a combination of the command `strings` to print readable output and `grep` to filter for `'==='` pattern. We can increase or reduce the equal signs as we'd like.

And we get the resultant command as follows:

```bash
strings data.txt|grep "==="
```

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
