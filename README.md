# Emojify

This notebook is a programming exercise of the Deep Learning Specialization by Deeplearning.ai. In this notebook, we are going to use word vector representations to build an Emojifier.

This emojifier app will make our text messages more expressive. So rather than writing:

&quot;Congratulations on the promotion! Let&#39;s get coffee and talk. Love you!&quot;

The emojifier can automatically turn this into:

&quot;Congratulations on the promotion! 👍 Let&#39;s get coffee and talk. ☕️ Love you! ❤️&quot;

#### Using word vectors to improve emoji lookups

- In many emoji interfaces, you need to remember that ❤️ is the &quot;heart&quot; symbol rather than the &quot;love&quot; symbol.
  - In other words, you&#39;ll have to remember to type &quot;heart&quot; to find the desired emoji, and typing &quot;love&quot; won&#39;t bring up that symbol.
- We can make a more flexible emoji interface by using word vectors!
- When using word vectors, you&#39;ll see that even if your training set explicitly relates only a few words to a particular emoji, your algorithm will be able to generalize and associate additional words in the test set to the same emoji.
  - This works even if those additional words don&#39;t even appear in the training set.
  - This allows you to build an accurate classifier mapping from sentences to emojis, even using a small training set.
