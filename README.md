# Block Release: Agile Processes

## Overview

Repo with support files for the block release on using the agile process for group software development.

## Development

### Git

This repository uses a Git [filter](https://git-scm.com/book/en/v2/Customizing-Git-Git-Attributes) to remove the output from notebooks so as to not clutter up your Git history. This is done using the `nbconvert` tool which can be installed with `pip install nbconvert`. This should help a little with merge conflicts but generally it is better to use native Python files for collaborative coding.

You can enable the filter by running the following command in your repository:

```shell
git config filter.strip-notebook-output.clean 'jupyter nbconvert --ClearOutputPreprocessor.enabled=True --to=notebook --stdin --stdout --log-level=ERROR'
```

## Documentation

User stories are contained [in the documentation folder](./doc/stories.md). Much more information about user stories can be found online, e.g. in [Atlassian](https://www.atlassian.com/agile/project-management/user-stories) have a good write up of Agile topics, including user stories.
