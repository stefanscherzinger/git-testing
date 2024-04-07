# Insights
Testing commits with different users:

- There's a local `config` file in each `.git` repository with 
  ```txt
    [user]
        name = Stefan-Testi
        email = stefan@testi-email.com
  ```
  that determines who's the author of local commits (normal and merge)
- The `name` and `email` fields can be arbitrary
- When pushing to the remote repo, git only asks for the key-phrase of the `id_rsa.pub` key in `~/.ssh/`
- This key must be one of the available keys in the personal (my) Github configuration.
- The commiter is the one specified in the local `config` file.
- I did not test what happens if there are several keys to choose from in `~/.ssh`.
- When doing merges online via PRs, Github lets me choose which email will be associated with this merge commit.
- The available email options are the ones associated with my account.

