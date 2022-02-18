Github issues for BPO users
===========================

Here are some frequently asked quesions about how to do things in
Github issues that you used to be able to do on `bpo`_.

Before you ask your own question, make sure you read :doc:`tracker2`
and :doc:`triaging2` (specifically including :doc:`gh-labels`) as those
pages include a lot of introductory material.

How to format my comments nicely?
---------------------------------

There is a wonderful `beginner guide to writing and formatting on Github
<https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github>`_.
Highly recommended.

One pro-tip we can sell you right here is that if you want to paste
some longer log as a comment, attach a file instead (see how below).
If you still insist on pasting it in your comment, do it like this::

    <details>
    <summary>This is the summary text, click me to expand</summary>

    Here goes the long, long text.
    It will be collapsed by default!
    </details>

How to attach files to an issue?
--------------------------------

Drag them into the comment field, wait until the file uploads, and Github
will automatically put a link to your file in your comment text.

How to link to file paths in the repository when writing comments?
------------------------------------------------------------------

Use Markdown links. If you link to the default Github path, the file
will link to the latest current version on the given branch.

You can get a permanent link to a given revision of a given file by
`pressing "y" <https://docs.github.com/en/repositories/working-with-files/using-files/getting-permanent-links-to-files>`_.

How to do advanced searches?
----------------------------

Use the `Github search syntax`_ or the interactive `advanced search`_ form
that generates search queries for you.

Where is the "nosy list"?
-------------------------

Subscribe another person to the issue by tagging them in the comment with
``@username``.

If you want to subscribe yourself to an issue, click the *🔔 Subscribe*
button in the sidebar.

Similarly, if you were tagged by somebody else but
decided this issue is not for you, you might click the *🔕 Unsubscribe*
button in the sidebar.

How to add issue dependencies?
------------------------------

Add a checkbox list like this in the issue description::

    - [x] #739
    - [ ] https://github.com/octo-org/octo-repo/issues/740
    - [ ] Add delight to the experience when all tasks are complete :tada:

then those will become sub-tasks on the given issue. Moreover, Github will
automatically mark a task as complete if the other referenced issue is
closed. More details in the `official Github documentation
<https://docs.github.com/en/issues/tracking-your-work-with-issues/about-task-lists>`_.

Where did the "Resolution" field go?
------------------------------------

Based on historical data we found it not being used very often.

Where did the "Low", "High", and "Critical" priorities go?
----------------------------------------------------------

Based on historical data we found those not being used very often.

How to find a random issue?
---------------------------

This is not supported by Github.

Where are regression and version labels? 
----------------------------------------

We're still discussing how to best add them.


.. _bpo: https://bugs.python.org/
.. _Github search syntax: https://docs.github.com/en/search-github/getting-started-with-searching-on-github/understanding-the-search-syntax
.. _advanced search: https://github.com/search/advanced