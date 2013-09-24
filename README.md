Dev-Standards
=============

Coding standards and developmental best practices at OSU Libraries &amp; Press.

Language Notes:

 * "Use" is a positive instruction, equivalent to "must use".
 * "Prefer" indicates a better option and its alternative to watch out for.
 * "Avoid" means don't do it unless you have good reason.
 * "Don't" means there's never a good reason.

General Practices
------------------

### Style Guidelines

1. Use two spaces to an indent.
2. Use unix-style line endings.
3. Use a newline at the end of the file.
4. Don't leave trailing whitespace.

#### Documentation

1. Do document every method using comments.
   * Prefer automatic documentation systems which use tag syntax.
   * Specific recommendations can be found in the language-specific files.
2. Avoid inline comments.

### Source Control
1. Use Git for source control.

#### Feature Branches
1. Do work in feature branches, named with a prefix 'feature/[branch-name]'.
2. Publish feature branches to the GitHub repository when:
   * Collaboratively developing the feature.
   * Seeking code review in advance of a pull request.
   * Sharing the feature externally.
   * If your code isn't going to be useful or meaningful to others,
     clean it up first.
3. Keep branches clean before publishing. Public commit history is immutable.
4. Send pull requests to merge features to Master.
5. Delete branches when they are fully merged and no longer needed.

#### Pull Requests & Merging
1. Keep pull requests clean.
   * Retain 'milestone' commits, representing substantial peices of work.
   * Squash minor and personal workflow commits into milestones.
2. Pull requests are subject to review. Someone other than you must merge them.
3. Let CI finish before merging a pull request.

### Security

 1. Use environment variables to store confidential information.
    * If this is not possible be sure that an example config is provided, the true config is not in source control, and the proper config is set up in production
      via an automatic deploy step.

Language Specific
------------------

 * [Python](python.md)

 * [Ruby](ruby.md)


License
-------

[![cc-by](http://i.creativecommons.org/l/by/3.0/88x31.png)](http://creativecommons.org/licenses/by/3.0)
