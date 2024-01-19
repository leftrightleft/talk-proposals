# How to accidentally host a crypto-mining operation in less than 3 minutes

## Summary

Public GitHub repositories are a gold mine for credential thieves. In fact, it takes only 3 minutes for AWS tokens written to public repositories to be stolen by crypto-mining bots. Once they have those tokens, your infrastructure becomes their mining operation. In this talk, we’ll explore how credentials are leaked on GitHub and how you can prevent these leaks.

## Abstract

Public GitHub repositories are a gold mine for credential thieves. In fact, it takes only 3 minutes for AWS tokens written to public repositories to be stolen by crypto-mining bots. Once they have those tokens, your infrastructure quickly becomes their mining operation.

However, AWS tokens are only one of many types of credentials leaked every day. At GitHub, we see this problem as a fundamental risk to the open source software supply-chain. 

In this session, we’ll share how GitHub is stopping credentials from being published to public repositories. We’ll talk about the most common types of secrets we see on our platform, how they’re leaked, and how you can identify and prevent them from being stored in plain-text in your environment. 

Join us to learn how we can all work together to put a stop to secret leaks and protect the open source ecosystem from security breaches.

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
    - What the future of secret identification looks like
- Q/A

## Outcomes/Learnings

By the end of this presentation, attendees will know:

- How bad the issue with leaked credentials is in the open source world, and how that applies to private code repositories
- How to identify plain-text secrets in their code repositories
- How to prevent secrets from being written to their open-source repositories
