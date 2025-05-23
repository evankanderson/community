---
title: "Knative Steering Committee Election - 2024 Voters Guide"
linkTitle: "2024 Voters Guide"
weight: 30
type: "docs"
---

# 2024 Voters Guide - Knative Steering Committee Election

## Purpose

The role of this election is to fill out the two (2) seats due for election
this year on the [Knative Steering Committee]. Each elected member will serve a
two (2) year term.  

## Background

This election will shape the future of Knative as a community and project. The
Knative Steering Committee (SC) is responsible for the general health of the
Knative community, as well as establishing and coordinating other working groups.

## Eligibility

Please refer to the [SC Election Charter] for:

- [Eligibility for candidacy]
- [Eligibility for voting]

The list of eligible voters is stored [in the community repository](./voters.yaml), but it is easier
to check if you are eligible by logging into [Elekto]. See Voting Process below for more details.

## Schedule

| Date         | Event                    |
| ------------ | ------------------------ |
| November 20  | Announcement of Election, call for nominations, exceptions |
| December 9   | All candidate nominations due by 00:00 UTC (5:00pm Pacific) |
| December 12  | Election Begins via Elekto UI |
| December 17  | Voter exception requests due by 23:59 UTC (4:59pm Pacific) |
| December 20  | Election Closes by 23:59 UTC (4:59pm Pacific) |
| January 7    | Announcement of Results |

Schedule update: 
- Candidate nomination deadline extended by a week from Dec 2 to Dec 9.

## Election Officers

In an effort to run a fair and transparent election, the following people
have been asked by the Steering Committee to run this election:

- [Dawn Foster](https://github.com/geekygirldawn)
- [Christoph Stäbler](https://github.com/creydr)

You can reach us by emailing elections@knative.team

## Candidacy Process

**Nomination**

If you want to stand for election for a Steering Committee Seat, open a PR against the
[knative/community repository](https://github.com/knative/community) to include
your candidate profile in the `/elections/2024-SC` folder, with the following
filename format:

```
candidate-githubid.md
```

This profile should include:

* Your name
* Your company affiliation (employer or otherwise)
* Your contributions to Knative
* Why you are running

You can find [a sample template in the folder](./nomination-template.md).

Once you have created the PR, you may email knative-dev@googlegroups.com and/or knative-users@googlegroups.com
*once* to let people know about your candidacy and encourage endorsements as
comments on the PR. Please use a text similar to the text below for your email in order to
encourage endorsements in Github and not on the mailing list:

```
Fellow Knative community members,

My name is {your name} and I am running for Steering Committee.  You can read
my profile here: {link to PR}.  If you support my candidacy, please endorse me
by commenting on that PR.  Please do not reply to endorse me on this list.
```

After a candidate has met all election requirements, the Election Officers will
merge the profile PR.

If you want to nominate someone else, you may do so, but PLEASE talk to them
first.

**Campaigning**

Please refer to the [SC Election Charter] and understand
that we care deeply about [limiting corporate campaigning]. The election
officers and members of the steering committee [pledge to recuse] themselves
from any form of electioneering.

You should be running as a "brand free" individual, based on your contribution
to the project as a member of this community, outside of whatever corporate
roles you may hold.

## Voting Process

Elections will be held using [Elekto], an online voting tool created
as a CNCF internal project. As a reminder it relies on GitHub Oauth to log you
in to vote, instead of relying on email. More details on voting are in the [Elekto documentation].

Thus, when you go to [Elekto] you will be prompted to log in your GitHub account.
Please do so, and then click on "Explore Election" to look at the list of 
elections.  From there you can click on the "2023 Knative SC Election."

The election page will, among other things, tell you if you are eligible to vote,
via a button at the top of the screen. Due to limitations in our contributor
data, many contributors may have been unfairly missed; if you are one of these,
please [file a voting exception] by the deadline listed above so that we can
enfranchise you.

As candidates file their candidate statements in the community repo, they will
become visible in the [Elekto] UI.  You may click through to any candidate
to see their profile.

Once the vote begins, you will be able to rank the candidates in the order of
your preference, and submit your ballot.  When you submit, you will be offered
a chance to set a password, which is required if you want the ability to return
and re-cast your ballot before the election close deadline found above.

Employer diversity is encouraged, and thus maximal representation will be
enforced as spelled out in the [SC Election Charter].

Elekto is being run on an OpenShift instance operated by Red Hat's Open Source 
Practice Office.  Individual ballot data is encrypted, and not retrievable by 
anyone except the voter, or in aggregate form.

### Decision
Ballots are compiled by Elekto and all candidates are ranked using the [Condorcet]
method, Schultze variant.

The newly elected body will be announced on the knative-dev mailing list.

Following the mailing list post, the raw voting results and winners will be published on the
[Knative Blog].

For more information, definitions, and/or detailed election process, please refer to
the [SC Election Charter].

[Knative Steering Committee]: https://github.com/knative/community/blob/main/STEERING-COMMITTEE.md
[SC Election Charter]: https://github.com/knative/community/blob/main/mechanics/SC.md

[limiting corporate campaigning]: https://github.com/kubernetes/steering/blob/master/elections.md#limiting-corporate-campaigning
[pledge to recuse]: https://github.com/kubernetes/steering/blob/master/elections.md#steering-committee-and-election-officer-recusal

[Elekto]: https://elections.knative.dev
[Elekto documentation]: https://elekto.dev/docs/

[Knative Blog]: https://knative.dev/blog/
[voters.md]: ./voters.yaml

[Eligibility for candidacy]: https://github.com/knative/community/blob/main/mechanics/SC.md#candidate-eligibility
[Eligibility for voting]: https://github.com/knative/community/blob/main/mechanics/SC.md#voter-eligibility

[file a voting exception]: https://elections.knative.dev/app/elections/2023-SC/exception
[Condorcet]: https://en.wikipedia.org/wiki/Condorcet_method
