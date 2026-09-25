# hamster

Originally inspired by https://github.com/kunchenguid/firstmate/

Firstmate is amazing, but honestly it does way more than what I need it for.  So this is a smaller & opinionated single player version for speed & token efficiency.

Start your coding agent sessions in the hamster folder with all your Github repos under the projects directory, and start working across multiple projects efficiently.

## Setup

```sh
cd
git clone git@github.com:khooeee/hamster.git
```

Add Hamster's helpers to PATH for your shell:

```sh
# Bash
echo 'export PATH=~/hamster/bin:$PATH' >> ~/.bashrc
echo 'alias ch="cd ~/hamster"' >> ~/.bashrc
echo 'alias chp="cd ~/hamster/projects"' >> ~/.bashrc


# Zsh
echo 'export PATH=~/hamster/bin:$PATH' >> ~/.zshrc
echo 'alias ch="cd ~/hamster"' >> ~/.zshrc
echo 'alias chp="cd ~/hamster/projects"' >> ~/.zshrc
```

Add `TERMINOLOGY.md` if you have terms that refer to some aspect of your project (i.e. basically a shortcut for a project subdirectory).

See bin folder for relevant helper scripts that will be very useful for day-to-day use.

## Default Conventions

- Any requested code change will open a PR immediately, and any related changes will commit and push to the PR immediately.
- When a PR is merged or closed, it will delete all worktrees & branches immediately. If your main worktree is on the same branch, it will also switch back to the default branch and fast forward it to latest.

Licensed under the [MIT License](LICENSE).
