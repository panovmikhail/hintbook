# How to configure per user git configuration

Create **.gitconfig** file in your user directory

```bash
[includeIf "gitdir:/Users/<user_name>/Documents/work1/"]
    path = ~/.gitconfig-work1

[includeIf "gitdir:/Users/<user_name>/Documents/my-code/gitlab.com/"]
    path = ~/.gitconfig-<user_name>-gitlab
```

Create per-project gitconfig files in your user directory:
* .gitconfig-user_name-gitlab
* .gitconfig-work1

> [!NOTE]
> This is Git's per-user configuration file.

```bash
[user]
    name = Mikhail Panov
    email = panovmikail@gmail.com
```

By the same way create config for each user/git-system