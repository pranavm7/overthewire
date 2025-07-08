---
description: Not a bot 🤖
---

# Level 5

{% embed url="https://overthewire.org/wargames/bandit/bandit5.html" %}

The hint is that the password is in the only human-readable file in the `inhere` directory.

This is what the `inhere` directory looks like:

<figure><img src="../.gitbook/assets/image (1).png" alt="Directory listing of the inhere directory"><figcaption><p>Directory listing of <code>inhere</code></p></figcaption></figure>

Now we could go through each file one by one, however it is quite an issue to get it to print. In order to get the 'human readable' text, we can use the `strings` command.&#x20;

<figure><img src="../.gitbook/assets/image (2).png" alt="&#x60;strings&#x60; command output"><figcaption><p><code>strings</code> command output</p></figcaption></figure>

In order to grow our skills, this seems like a great chance to use a bash one-liner.

```bash
for i in {0..9}; do echo "File ./-file0$i: $(strings './-file0'$i)"; done
# Breaking the oneliner down
for i in {0..9};do # for loop where i iterates over 0,1,2..9 
echo "File ./-file0$i: $(strings './-file0'$i)";
# echo formats output, strings prints readable items in file
done # end the for loop
```

And the output is as follows:

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

And now we learned a bit of bash scripting!
