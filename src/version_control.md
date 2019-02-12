This content is hosted at <https://github.com/ml-evs/part2-computing-git-tutorial> under the MIT license (i.e. do what you want with this material). The talk slides and notes are available as PDFs. Any queries/corrections can be raised as issues/pull requests on GitHub or Cambridge people can email me (me388) directly if they would prefer.
The aim of this tutorial is to teach basic concepts of version control that you might consider using for the coursework. A few hours of investment, and maybe some moments of confusion, will hopefully lead to a productivity boost. We shall work with the Git (`git`) version control system as, at the time of writing this, it dominates the market with Subversion (`svn`) and Mercurial (`hg`) lagging behind (as evidenced by [Google trends](https://g.co/trends/CECvA)).
`git` is an example of what is called a distributed version control system. This means that there is no "master copy" of a project, and instead the entire history of a project is mirrored on the computer of every developer (and potentially user). This becomes extremely useful when multiple people are actively developing a project for reasons we shall touch on later.
Each provider has its own advantages and disadvantages to consider but for our usage they are all broadly similar (and all allow unlimited private repos for free, often providing extra benefits for students [^students]). One of the useful features of distributed VCS is that you can easily transfer your entire code history to a different provider, since you are constantly mirroring your own version of the project locally [^microsoft].
#### Example 1.1: A Contrived Example of a Local Repository
In this example, we will make a local Git repository, add some files to it, commit them, make some changes, then commit the changes. Very exciting. First, make a new folder and tell Git that you want it to be a repository:
```
$ mkdir git_example_1
$ cd git_example_1
$ git init
```

Now, lets make a file with some text in it, by reciting Moby Dick from memory...