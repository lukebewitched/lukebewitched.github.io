---
author: <author_id>
layout: post
title: Ruby On Rails Prerequisites
description: Contains the necessary basics to get you up to speed
date: '2024-05-28 19:32:01 +0300'
categories: [Beginner, Basics]
tags: [basics]
pin: true
---

Generating a controller
```bash
$ rails generate controller StaticPages home help
```
{: .nolineno }

Destroying a controller
```bash
$ rails destroy controller StaticPages home help
```
{: .nolineno }

Generating a model
```bash
$ rails generate model User name:string email:string
```
{: .nolineno }

Destroying a model
```bash
$ rails destroy model User
```
{: .nolineno }

Initiating a database migration
```bash
$ rails db:migrate
```
{: .nolineno }

Undoing a database migration
```bash
#Undoing a single migration
$ rails db:rollback
#Go back all the way to the beginning
$ rails db:migrate VERSION=0
```
{: .nolineno }

> Test-driven development (TDD) is a valuable tool to have in your kit. Here are a set of guidelines on when we should test first (or test at all):
{: .prompt-info}

- [x] When a test is especially short or simple compared to the application code it tests, lean toward writing the test first.

- [x] When the desired behavior isn’t yet crystal clear, lean toward writing the application code first, then write a test to codify the result.

- [x] Because security is a top priority, err on the side of writing tests of the security model first.

- [x] Whenever a bug is found, write a test to reproduce it and protect against regressions, then write the application code to fix it.

- [x] Lean against writing tests for code (such as detailed HTML structure) likely to change in the future.

- [x] Write tests before refactoring code, focusing on testing error-prone code that’s especially likely to break.

{% include giscus.html %}
