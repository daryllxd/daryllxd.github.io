# My Blog

```
Setup:

$ git worktree add public master # This will make it such that when we compile via `hugo`, the `public` directory links to the `master` branch.

```

``` shell
$ hugo new posts/TITLE.md
$ h or $ hugo server -D                           # Serve at localhost:13131
$ hugo -E                                         # Publish (remove draft: true from the articles

$ pandoc cv_pdf_format.md -o static/cv.pdf # Compiles the CV
```
