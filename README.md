# GitHub Actions

> [!NOTE]
> The repository name was a suggestion by GitHub and I kept it, however in
> terms of what the repository actually contains it is mostly silly.

Exercises to get used to GitHub Actions with some notes in the `README.md`.

## Workflow Definition

> [!TIP]
> Very helpful reference used a lot to figure out the structure: https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax

There are different sets of runners available for use. Public repositories can
use the GitHub hosted ones for free, while private repositories have a quota
for runners. [Self-hosting a runner is also
possible](https://docs.github.com/en/actions/concepts/runners/self-hosted-runners).
See the [full
explanation](https://docs.github.com/en/actions/reference/workflows-and-actions/workflow-syntax#choosing-github-hosted-runners)
for details.

In the folder `$GITHUB_WORKSPACE` is the entire code as checked out by the
action. The path indicates that it uses the format
`/home/runner/work/$reponame/$reponame`.

As I found out through tips of friends the entire GitHub workflow definitions
are compatible with Forgejo and Gitea workflows! There are some differences overall but they are neatly documented.

https://forgejo.org/docs/latest/user/actions/github-actions/
https://docs.gitea.com/usage/actions/comparison

Both differ a lot from GitLab CI/CD a lot though.
