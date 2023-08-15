# gh-label-template-ethereum
GitHub Repo pre-configured for Ethereum projects based off of Spearbit


### Requirements 

Install:

```bash
brew install gh
```

]GitHub command-line tool](https://github.com/cli/cli)


## Usage

### gh label clone

```
gh label clone <source-repository> [flags]
```

Clones labels from a source repository to a destination repository on GitHub. By default, the destination repository is the current repository.

All labels from the source repository will be copied to the destination repository. Labels in the destination repository that are not in the source repository will not be deleted or modified.

Labels from the source repository that already exist in the destination repository will be skipped. You can overwrite existing labels in the destination repository using the --force flag.

### Options

`-f`, `--force`

Overwrite labels in the destination repository

### Options inherited from parent commands

`-R`, `--repo <[HOST/]OWNER/REPO>`

Select another repository using the \[HOST/\]OWNER/REPO format

### Examples

```
# clone and overwrite labels from cli/cli repository into the current repository
$ gh label clone cli/cli --force

# clone labels from cli/cli repository into a octocat/cli repository
$ gh label clone cli/cli --repo octocat/cli
```

### See also

-   [gh label](https://cli.github.com/manual/gh_label)
