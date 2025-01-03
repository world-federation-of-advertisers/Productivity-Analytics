<h1 align="center">
  <br>
  <a href="https://github.com/world-federation-of-advertisers"><img src="https://raw.githubusercontent.com/world-federation-of-advertisers/Home/refs/heads/main/img/Halo-Logo.png" alt="Halo CMM" width="200"></a>
  <br>
</h1>

<h3 align="center">Productivity Analytics</h3>

<p align="center">
  <a href="#description">Description</a> •
  <a href="#docs">Docs</a> •
  <a href="#owner">Owner</a> •
  <a href="#get-help">Get Help</a>
</p>
<hr>

## Description

A suite of tools for productivity analytics.

## Owner

[@mikkokotila](https://github.com/mikkokotila)

## Docs

### Get started

1) Download the package to your local machine
2) Start an environment inside `productivity-analytics` directory

To the root of the `productivity-analytics`, add a file `.env.dev` with the following contents: 

```
repo_owner=world-federation-of-advertisers
repo_name=cross-media-measurement
token=your_github_token
```

**NOTE:** The `repo_name` variable decides which repo data is fetched for. All the reports will be based on that data. You can also change the repo_name when executing the data building functions.

### Collect data

To understand how the data is collected, check out [Basic Walkthrough](./examples/Basic-Walkthrough.ipynb). The data collection is currently per repo, so a separate dataset must be created for each repo following the examples given in the notebook.

### Analyze data

[Velocity Report](./examples/Velocity-Report.ipynb) answers the following questions for `cross-media-measurement` repo:

- How many days on average it takes to go from opening a PR to merging or closing it?
- How many PRs are each contributor opening?
- How many PR reviews or comments are each contributor making?
- How many PR change requests are each contributor making?
- How many back and forths with the PR author does it require to merge a PR?

[Productivity Report](./examples/Productivity-Report.ipynb) answers the following questions for `cross-media-measurement` repo:

- How many PRs are there for each Conventional Commit tags?
- How many sustaining PRs vs. transformative PRs are there?
- How many merged vs. not merged PRs are there by contributor?
- How many PRs that never get merged are there by contributor?

## Get Help

If you need any help or have suggestions for improvements, you can do that [here](issues/new).
