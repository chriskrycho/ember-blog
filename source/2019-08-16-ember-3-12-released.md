---
title: Ember 3.12 Released
author: Kenneth Larsen
tags: Releases, 2019, 3, 3.12
responsive: true
---

Today the Ember project is releasing version 3.12 of Ember.js, Ember Data, and Ember CLI. This release of Ember.js is an LTS (Long Term Support) candidate. LTS candidates contain no new features, and have an extended support schedule. To learn about the next wave of features coming in future releases, see the [Octane release plan](https://blog.emberjs.com/2019/08/15/octane-release-plan.html) post.

This release kicks off the 3.13 beta cycle for all sub-projects. We encourage our community (especially addon authors) to help test these beta builds and report any bugs before they are published as a final release in six weeks' time. The [ember-try](https://github.com/ember-cli/ember-try) addon is a great way to continuously test your projects against the latest Ember releases.

You can read more about our general release process here:

- [Release Dashboard](http://emberjs.com/builds/)
- [The Ember Release Cycle](http://emberjs.com/blog/2013/09/06/new-ember-release-process.html)
- [The Ember Project](http://emberjs.com/blog/2015/06/16/ember-project-at-2-0.html)
- [Ember LTS Releases](http://emberjs.com/blog/2016/02/25/announcing-embers-first-lts.html)

---

## Ember.js

Ember.js is the core framework for building ambitious web applications.

### Changes in Ember.js 3.12
The 3.12.0 release is an Ember.js Long-Term Support candidate. In six weeks, the 3.12.x series will become the latest LTS release and six weeks after that the 3.4 LTS branch will no longer receive bugfix patches. LTS versions allow teams to upgrade less frequently while still getting support from the Ember project and the wider ecosystem.

For more information about Ember's LTS policies, see the [announcement blog post](http://emberjs.com/blog/2016/02/25/announcing-embers-first-lts.html) and [builds page](http://emberjs.com/builds/).

Ember.js 3.12 is an incremental, backwards compatible release of Ember with bugfixes, performance improvements, and minor deprecations. There is zero (0) new features, zero (0) deprecations, and several bugfixes in this version.

#### New Features (0)

There are no new features in Ember.js 3.12.

#### Deprecations (0)

There are no deprecations added in Ember.js 3.12

Deprecations are added to Ember.js when an API will be removed at a later date. Each deprecation has an entry in the deprecation guide describing the migration path to a more stable API. Deprecated public APIs are not removed until a major release of the framework.

Consider using the [ember-cli-deprecation-workflow](https://github.com/mixonic/ember-cli-deprecation-workflow) addon if you would like to upgrade your application without immediately addressing deprecations.

For more details on changes in Ember.js 3.12, please review the [Ember.js 3.12 release page](https://github.com/emberjs/ember.js/releases/tag/v3.12.0).

---

## Ember Data

Ember Data is the official data persistence library for Ember.js applications.

### Changes in Ember Data 3.12

#### New Features (0)

No new features introduced in Ember Data 3.12.

#### Deprecations (2)

**Evented Api Usage (1 of 2)**

With Ember Data 3.12 the `Ember.Evented` functionality on `DS.Model`, `DS.ManyArray`, `DS.Errors`, `DS.RecordArray`, and `DS.PromiseManyArray` is deprecated. Please refer to the [deprecations guide](https://deprecations.emberjs.com/ember-data/v3.x#toc_evented-api-usage) for more info.

**Record Lifecycle Event Methods (2 of 2)**

Lifecycle event methods on `DS.model` such as `becameError`, `becameInvalid`, `didCreate`, `didDelete`, `didLoad`, `didUpdate`, `ready`, `rolledBack` are deprecated as of Ember Data 3.12. For a guide to replacing these event methods with computed properties please refer to the [deprecations guide](https://deprecations.emberjs.com/ember-data/v3.x#toc_record-lifecycle-event-methods)


For more details on changes in Ember Data 3.12, please review the
[Ember Data 3.12.0 release page](https://github.com/emberjs/data/releases/tag/v3.12.0).

---

## Ember CLI

Ember CLI is the command line interface for managing and packaging Ember.js applications.

### Upgrading Ember CLI

You may upgrade Ember CLI easily using the ember-cli-update project:

```bash
npm install -g ember-cli-update
ember-cli-update
```

This utility will help you to update your app or add-on to the latest Ember CLI version. You will probably encounter merge conflicts, in which the default behavior is to let you resolve conflicts on your own. For more information on the `ember-cli-update` project, see [the github README](https://github.com/ember-cli/ember-cli-update).

While it is recommended to keep Ember CLI versions in sync with Ember and Ember Data, this is not required. After updating ember-cli, you can keep your current version(s) of Ember or Ember Data by editing `package.json` to revert the changes to the lines containing `ember-source` and `ember-data`.

### Changes in Ember CLI 3.12

#### New Features (0)

There are no new features in Ember CLI 3.12.

#### Deprecations (0)

There are no new deprecations in Ember CLI 3.12.

---

For more details on the changes in Ember CLI 3.12 and detailed upgrade
instructions, please review the [Ember CLI  3.12.0 release page](https://github.com/ember-cli/ember-cli/releases/tag/v3.12.0).

## Thank You!

As a community-driven open-source project with an ambitious scope, each of these releases serve as a reminder that the Ember project would not have been possible without your continued support. We are extremely grateful to our contributors for their efforts.
