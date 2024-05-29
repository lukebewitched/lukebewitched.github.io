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
rails generate controller StaticPages home help
```

Destroying a controller
```bash
rails destroy controller StaticPages home help
```

Generating a model
```bash
rails generate model User name:string email:string
```

Destroying a model
```bash
rails destroy model User
```

Initiating a database migration
```bash
rails db:migrate
```

Undoing a database migration
```bash
#Undoing a single migration
rails db:rollback
#Go back all the way to the beginning
rails db:migrate VERSION=0
```
