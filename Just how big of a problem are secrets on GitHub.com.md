# Just how big of a problem are secrets on GitHub.com?

## Summary

Public GitHub repositories are a gold mine for credential thieves. In fact, over the course of 2023, more than 10 million plain-text credentials were written to public repositories on github.com.  In this talk, we’ll explore how credentials are leaked on GitHub, what GitHub is doing to address the problem, and how the open source community can work together to meaningfully reduce the risk of credentials in public repos.

## Abstract

Public GitHub repositories are a gold mine for credential thieves. In fact, over the course of 2023, more than 10 million plain-text credentials were written to public repos on [github.com](http://github.com/).

In this session, we’ll share how GitHub is addressing this problem.

We'll do a deep data analysis on the most common secrets we see, as well as how and where they're leaked.  We'll explore how attackers are using these tokens and provide a live demo showing how just how quickly leaked credentials can be used to exploit cloud infrastructure.  Finally, we'll wrap up the discussion with practical tips we can all use to make meaningful security changes in the open source ecosystem.

## Outline

- Introduction
- Discuss the scope of the problem
    - How many credentials are actually published on GitHub every day
    - Where are secrets being leaked?
        - Gists
        - Commit messages
        - Actions workflows
        - Source code
    - How are attackers using these credentials?
        - Live demo leaking an AWS token on a public repo
- Strategies for dealing with credentials in your environment
    - Secret management
        - Vault, GitHub secrets, AWS secrets manager, etc.
    - Alternatives to hardcoded credentials
    - User training
- What GitHub is doing about credentials
    - Secret scanning in public repos
    - Preventing tokens from being stored in repos
    - What the future of secret identification looks like at GitHub
- Q/A
