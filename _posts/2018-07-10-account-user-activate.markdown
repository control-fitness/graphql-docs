---
title: Account User Activate
layout: post
date: '2018-07-10 22:34:40 -0600'
mutation: AccountUserActivate
type: Mutation
categories: mutations
---

**Inputs**:

Name | Type | Description
------- | ------- | ---------------
confirmedToken | String | Automatically generated text string to activate a user account. This chain is sent with the electronic pad to confirm the user's account.

**Outputs**:

Name | Type | Description
------- | ------- | ---------------
activated | Boolean | To identify if the user's account was activated.

**Example**:

```
mutation AccountUserActivate {
  accountUserActivate(input: {
    confirmedToken: "abc123"
  }) {
    activated
  }
}
```
