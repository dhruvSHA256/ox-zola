+++
title = "Image"
date = 2017-07-06T16:21:36-04:00
tags = []
+++

**To be fixed**: At the moment, you need to place the point here and do `C-c C-e H H`. If the point is under any of the nested sub-trees in here where you do that, only that subtree gets exported.

*Need to add smarts that determines which subtree contains the whole post.. like look for `EXPORT_FILE_NAME`?*


# Unclickable image

![img](./images/org-mode-unicorn-logo.png)

**To be fixed**: The sub-headings in a post get exported as *Heading 1* instead of *Heading 2*.

For example, this sub-section&rsquo;s heading is exported as:

{{< highlight markdown >}}
# Unclickable image
{{< /highlight >}}

instead of

{{< highlight markdown >}}
## Unclickable image
{{< /highlight >}}

So the sub-heading title and the post title both get the *Heading 1* tag and look the same size.


# Clickable link that opens the image

[Click here to see the unicorn](./images/org-mode-unicorn-logo.png)


# Clickable image that opens the image

Click below image to jump to the unicorn image.

[![img](./images/org-mode-unicorn-logo.png)](images/org-mode-unicorn-logo.png)

-   **NOTE 1:** `file:` has to be used in both Link and Description components of the Org link.
-   **NOTE 2:** As the path is relative, we need to use `./images/..` instead of `/images/..`.