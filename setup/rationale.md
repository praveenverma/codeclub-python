Rationale for setup decisions
===============================

PyCharm
-------

I know nothing much about Python IDEs. PyCharm was recommended and seems to be quite good.

The school PCs I'm using are Atom netbooks with small screens. Eclipse is therefore probably out of the question.

PyCharm have free educational licenses but it seems some ID is required. I haven't got to the
bottom of this yet.

I am not completely happy with the choice of PyCharm. Any better ideas?

github for storing source code
--------------------------------

git and github are obviously very complicated and to be avoided when teaching kids.
But they were the best idea I could come up with:

* With the Scratch exercises the kids are used to uploading their projects so that they can
  work on them from home and/or show their parents. This achieves the same, although
  we will need to go through some hassle teaching them to upload etc.
* github is unlikely to have been blocked by different schools (I hope). It uses https so school
  proxies probably won't interfere too much?? (These statements may be entirely wrong.)
* At a simple level it works well with PyCharm (for checking code out).

I believe all upload/download steps should be by rote as opposed to trying to understand
git/github because that could be a whole terms' curriculum in itself.

Submodules
----------

You'll notice that the source code for the problems (and their solutions) is stored in submodules
within the main git project.

I have a love/hate relationship with submodules but I think it works OK in this case. It means
that the code projects themselves can be stored independently on github, and further, that different
revisions of the same project can be used for problem/solution code.

Kids can therefore check out the problem code as an individual repository during an exercise,
whilst for a teacher/guide to check out the whole thing it's a matter of checking out the parent
project and then just running `git submodule update --init`.

Markdown for documents
----------------------

Just because it's easy to edit and for git to merge, so multiple people can be working on these
projects without the risk of binary files having merge conflicts. It also has the advantage that it
can automatically show nicely formatted Python code.

On the other hand it's proving to be an almighty pain for constructing the Scratch-Python cheatsheet,
and it's hopeless for pretty formatting along the lines of the Scratch CodeClub exercises.
