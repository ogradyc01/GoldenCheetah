First. Thank you for taking the time to help enhance and improve Golden Cheetah.

Second, here are some guidelines to help make it easier to get the patch submitted.

1: Please make sure your patch has no trailing whitespaces. GIT hates trailing whitespaces.

Run two versions of the source code.
Apply your patch to an unmodifed current master of the branch you are working on.
Check that there are no whitespaces after each commit: git show --color
Trailing whitespaces turn up as RED blobs.

2: If you are patching for a bug or in existing code

Please do not submit style formatting changes in the original patch.
Just submit the changes that fix the bug or tweak the code.
This is so those who review the code can see what is being done easily.
If you would like to do formatting changes for code readability, please submit a second patch with these changes.

3: Make sure that you attach the patch to the bug or feature

You did raise a bug or feature request didn't you if you initiated this?
Please make sure that in the message for the patch you put in a line:

Fixes: #xxx

4: Check out Sean's original developers guide. It is a good read:

[Golden Cheetah Website - Developer's Guide](http://www.goldencheetah.org/developers-guide.html)