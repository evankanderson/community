---
title: "Knative working group"
linkTitle: "Join working groups"
weight: 25
type: "docs"
aliases:
  - /contributing/working-groups/
---

Most community activity is organized into _working groups_.

Working groups follow the [contributing](../CONTRIBUTING.md) guidelines although
each of these groups may operate a little differently depending on their needs
and workflow.

When the need arises, a new working group can be created. See the
[working group processes](../mechanics/WORKING-GROUP-PROCESSES.md) for working
group proposal and creation procedures.

The working groups generate design docs which are kept in a
[shared drive](https://drive.google.com/drive/folders/0AM-QGZJ-HUA8Uk9PVA) and
are available for anyone to read and comment on. The shared drive currently
grants read access to
[knative-users@](https://groups.google.com/forum/#!forum/knative-users) and edit
and comment access to the
[knative-dev@](https://groups.google.com/forum/#!forum/knative-dev) Google
group.

Some working groups (mostly those with a plug-in or extension model) end up
responsible for a set of GitHub repos, one for each extension. This allows for
easier dependency management; in these cases, one or more repo prefix names will
be recorded as canonical "extension names" to allow WGs to be responsible for
their own namespace without needing to get Steering Committee approval for each repo name.

Additionally, all working groups should hold regular meetings, which should be
added to the
[shared knative calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com)
WG leads should have access to be able to create and update events on this
calendar, and should invite knative-dev@googlegroups.com to working group
meetings.

### Calendar import

If you're using Google Calendar, the above should work. If you're using some
other system (Apple Calendar or Outlook, for example),
[here is an iCal export of the community calendar](https://calendar.google.com/calendar/ical/knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com/public/basic.ics).

- [Follow these directions to import into Outlook Web](https://support.office.com/en-us/article/import-or-subscribe-to-a-calendar-in-outlook-on-the-web-503ffaf6-7b86-44fe-8dd6-8099d95f38df)
- [Follow these directions for desktop Outlook](https://support.office.com/en-us/article/See-your-Google-Calendar-in-Outlook-C1DAB514-0AD4-4811-824A-7D02C5E77126)
- [Follow the import directions to import into Apple Calendar](https://support.apple.com/guide/calendar/import-or-export-calendars-icl1023/mac)

# Working Groups

The current working groups are:

- [Working Groups](#working-groups)
  - [Serving](#serving)
  - [Client](#client)
  - [User Experience](#user-experience)
  - [Eventing](#eventing)
  - [Functions](#functions)
  - [Operations](#operations)
  - [Productivity](#productivity)
  - [Security](#security)
- [Emeritus Working Groups](#emeritus-working-groups)
  - [Eventing Kafka](#eventing-kafka)
  - [Build](#build)
  - [Documentation](#documentation)
  - [Event Delivery (previously called Eventing Channels Working Group)](#event-delivery-previously-called-eventing-channels-working-group)
  - [Eventing Sources](#eventing-sources)
  - [Observability](#observability)

## Serving

Covers API [resources](https://github.com/knative/serving/tree/main/pkg/apis/serving),
[validation](https://github.com/knative/pkg/tree/main/webhook),
[semantics](https://github.com/knative/pkg/tree/main/controller), autoscaling and networking behavior.

| Artifact                   | Link                                                                                                                                                                                                                                                                     |
| -------------------------- |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Charter                    | TODO (historical, was created before formal WG process)                                                                                                                                                                                                                  |
| Roadmap                    | [API](https://github.com/orgs/knative/projects/35), [Scaling](https://github.com/orgs/knative/projects/36/views/1)                                                                                                                                                       |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                                                                                                                                      |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1rpag5-zffHGxAT7V4Nv28C_xx5Ow6L4mZuHbe3ebOQ8/edit)                                                                                                                                                 |
| Community Meeting Calendar | Thurs 8:00am PST [Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com)                                                                                                                            |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1rpag5-zffHGxAT7V4Nv28C_xx5Ow6L4mZuHbe3ebOQ8/edit)                                                                                                                                                                            |
| Document Folder            | [API](https://drive.google.com/drive/folders/1eCSmaqJ4LYcuS3TlOqjW0xETnzLmo6Q9), [Scaling](https://drive.google.com/drive/folders/1IDDkJ3FD47xFSHY3iA9U2Q8th3Cwdo0K), [Networking](https://docs.google.com/document/d/1rpag5-zffHGxAT7V4Nv28C_xx5Ow6L4mZuHbe3ebOQ8/edit) |
| Repos                      | [`knative/serving`](https://github.com/knative/serving), [`knative/networking`](https://github.com/knative/networking), [`knative/pkg`](https://github.com/knative/pkg), [`knative-extensions/net-*`](https://github.com/knative-extensions?q=net)                       |
| Slack Channel              | [#knative-serving](https://cloud-native.slack.com/archives/C04LMU0AX60) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                                                           |
| Github Team WG Leads       | [@knative/serving-wg-leads](https://github.com/orgs/knative/teams/serving-wg-leads/members)                                                                                                                                                                              |

| &nbsp;                                                   | Leads            | Company | Profile                                 |
| -------------------------------------------------------- | ---------------- | ------- | --------------------------------------- |
| <img width="30px" src="https://github.com/dprotaso.png"> | Dave Protasowski | Independent | [dprotaso](https://github.com/dprotaso) |

| &nbsp;                                                         | Emeritus Leads   | Subgroup   | Profile                                             | Duration  |
| -------------------------------------------------------------- | ---------------- | ---------- | --------------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/dgerd.png">          | Dan Gerdesmeier  | API        | [dgerd](https://github.com/dgerd)                   | 2019-2020 |
| <img width="30px" src="https://github.com/mattmoor.png">       | Matt Moore       | API        | [mattmoor](https://github.com/mattmoor)             | 2018-2021 |
| <img width="30px" src="https://github.com/julz.png">           | Julian Friedman  | Scaling    | [julz](https://github.com/julz)                     | 2021-2022 |
| <img width="30px" src="https://github.com/markusthoemmes.png"> | Markus Thömmes   | Scaling    | [markusthoemmes](https://github.com/markusthoemmes) | 2019-2021 |
| <img width="30px" src="https://github.com/vagababov.png">      | Victor Agababov  | Scaling    | [vagababov](https://github.com/vagababov)           | 2019-2021 |
| <img width="30px" src="https://github.com/josephburnett.png">  | Joseph Burnett   | Scaling    | [josephburnett](https://github.com/josephburnett)   | 2018-2019 |
| <img width="30px" src="https://github.com/tcnghia.png">        | Nghia Tran       | Networking | [tcnghia](https://github.com/tcnghia)               | 2018-2021 |
| <img width="30px" src="https://github.com/ZhiminXiang.png">    | Zhimin Xiang     | Networking | [ZhiminXiang](https://github.com/ZhiminXiang)       | 2020-2022 |
| <img width="30px" src="https://github.com/nak3.png">           | Kenjiro Nakayama | Networking | [nak3](https://github.com/nak3)                     | 2020-2022 |
| <img width="30px" src="https://github.com/psschwei.png"> | Paul Schweigert | Serving | [psschwei](https://github.com/psschwei) | 2022-2023 |


## Client

[Client](https://github.com/knative/client), CLI, client libraries, and client
conventions

| Artifact                   | Link                                                                                                                                                                                                                                              |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter                    | [Charter](./client/CHARTER.md)                                                                                                                                                                                                                    |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/37)                                                                                                                                                                                           |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                                                                                                               |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1cD7NkJJhSBpo2Q6RBHrbrSe6R5zjTZgO_YDGAluQ_oI/edit)                                                                                                                          |
| Community Meeting Calendar | Every other Tuesday 10:30a Pacific<br>[Calendar Invitation](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1cD7NkJJhSBpo2Q6RBHrbrSe6R5zjTZgO_YDGAluQ_oI/edit)                                                                                                                                                     |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1QffYD_XM0vqaXDvFlZVsJHAT6-AahJCO)                                                                                                                                                                |
| Repos                      | [`knative/client`](https://github.com/knative/client), `kn-plugin-*`                                                                                                                                                                              |
| Slack Channel              | [#knative-client](https://cloud-native.slack.com/archives/C04LY4SKBQR) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                                                                                                                                                |
| Github Team WG leads       | [@knative/client-wg-leads](https://github.com/orgs/knative/teams/client-leads/members)                                                                                                                                                            |

| &nbsp;                                                      | Leads          | Company | Profile                                       |
| ----------------------------------------------------------- | -------------- | ------- | --------------------------------------------- |
| <img width="30px" src="https://github.com/dsimansk.png">    | David Simansky | Red Hat | [dsimansk](https://github.com/dsimansk)       |


| &nbsp;                                                     | Emeritus Leads  | Profile                                     | Duration  |
| ---------------------------------------------------------- | --------------- | ------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/rhuss.png">      | Roland Huß      | [rhuss](https://github.com/rhuss)           | 2018-2025
| <img width="30px" src="https://github.com/sixolet.png">    | Naomi Seyfer    | [sixolet](https://github.com/sixolet)       | 2018-2021 |
| <img width="30px" src="https://github.com/cppforlife.png"> | Dmitriy Kalinin | [cppforlife](https://github.com/cppforlife) | 2018-2020 |

## User Experience

User Experience concerns across Knative components, as well as designer contribution experience.
| Artifact                   | Link                                                                                                                                                             |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter / Mission          | [Charter](https://docs.google.com/document/d/1b_CliwhqjwcHHLh_UU-DwsRMDxE50cGc6vuJh0OW57E/edit?usp=sharing)                                                      |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/20)                                                                                                           |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                              |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1NSlGHen5Dh6c2A0LGavGWibddWrlSLV_PbEbMpNjSTU/edit?usp=sharing)                             |
| Community Meeting Calendar | Every other Thursday from 9:00-10:00am EST <br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1VCObP1IQFPDGzGG5KIgytQwX7RrU0tyeB7FGjkY0pPk/edit)                                                                    |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1XzZGqV7yHo38d_l7rH1uSIrbQp3JlbBP?usp=sharing)                                                                   |
| Slack Channel              | [#knative-ux](https://cloud-native.slack.com/messages/knative-ux) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                         |
| Github Repository          | [/ux](https://github.com/knative/ux)                                                                                                                             |
| Github Team WG leads       | [@knative/ux-wg-leads](https://github.com/orgs/knative/teams/ux-wg-leads/members)                                                                                |

| &nbsp;                                                               | Leads            | Company               | Profile                                                  |
| -------------------------------------------------------------------- | ---------------- | --------------------- | -------------------------------------------------------- |
| <img width="30px" src="https://github.com/cali0707.png">             | Calum Murray     | University of Toronto | [cali0707](https://github.com/cali0707)                  |
| <img width="30px" src="https://github.com/zainabhusain227.png">      | Zainab Husain    | OCAD University       | [zainabhusain227](https://github.com/zainabhusain227)    |
| <img width="30px" src="https://github.com/mmejia02.png">             | Mariana Mejia    | OCAD University       | [mmejia02](https://github.com/mmejia02)                  |
| <img width="30px" src="https://github.com/Leo6Leo.png">              | Leo Li           | University of Toronto               | [Leo Li](https://github.com/Leo6Leo)                     |

| &nbsp;                                                        | Emeritus Leads   | Profile                                           | Duration  |
| ------------------------------------------------------------- | ---------------- | ------------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/csantanapr.png">    | Carlos Santana   | [csantanapr](https://github.com/csantanapr)       | 2020-2022 |
| <img width="30px" src="https://github.com/omerbensaadon.png"> | Omer Bensaadon   | [omerbensaadon](https://github.com/omerbensaadon) | 2020-2021 |

## Eventing

Event sources, bindings, FaaS framework, and orchestration

| Artifact                   | Link                                                                                                                                                         |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Charter / Mission          | [Enable asynchronous application development through event delivery from anywhere.](https://github.com/knative/eventing/blob/main/docs/mission.md)           |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/38)                                                                                                       |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                          |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1Xha-FeunojN49OJN7W0WBnPMcRtp1ycYpbkiir6XsE0/edit)                                     |
| Community Meeting Calendar | Thursday 8:00a-8:30a PST<br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1Xha-FeunojN49OJN7W0WBnPMcRtp1ycYpbkiir6XsE0/edit)                                                                |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/16A4v6Qv9MNSumpy6geGm0u1izDqAfiNo)                                                                           |
| Repos                      | [`knative/eventing`](https://github.com/knative/eventing), `eventing-*`                                                                                      |
| Slack Channel              | [#knative-eventing](https://cloud-native.slack.com/archives/C04LMU33V1S) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                                    |
| Github Team WG leads       | [@knative/eventing-wg-leads](https://github.com/orgs/knative/teams/eventing-wg-leads/members)                                                                |

| &nbsp;                                                        | Leads                | Company | Profile                                     |
| ------------------------------------------------------------- | -------------------- | ------- | ------------------------------------------- |
| <img width="30px" src="https://github.com/pierdipi.png">      | Pierangelo Di Pilato | Red Hat | [pierdipi](https://github.com/pierdipi)     |
| <img width="30px" src="https://github.com/creydr.png">        | Christoph Stäbler    | Red Hat | [creydr](https://github.com/creydr)         |


| &nbsp;                                                  | Emeritus Leads            | Profile                                | Duration  |
| ------------------------------------------------------- | ------------------------- | -------------------------------------- | --------- |
| <img width="30px" src="https://github.com/lionelvillard.png"> | Lionel Villard (Technical) |  [lionelvillard](https://github.com/lionelvillard) | 2020-2022
| <img width="30px" src="https://github.com/devguyio.png">| Ahmed Abdalla (Execution) | [devguyio](https://github.com/devguyio)| 2021-2022 |
| <img width="30px" src="https://github.com/grantr.png">  | Grant Rodgers (Technical) | [grantr](https://github.com/grantr)    | 2020-2021 |
| <img width="30px" src="https://github.com/vaikas.png">  | Ville Aikas (Technical)   | [vaikas](https://github.com/vaikas)    | 2018-2021 |

## Functions

Knative Functions [CLI](https://github.com/knative/func), API, and [language packs](https://github.com/knative-extensions/func-tastic)

| Artifact                   | Link                                                                                                                     |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------|
| Charter / Mission          | [Charter](https://github.com/lance/community/blob/add-func-wg/working-groups/functions/CHARTER.md)                                                                              |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/49)                                                            |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                      |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1zydqnsw2ty5siL_FT2U7klMTK7OuKWRZNmkUJMx3cWE/edit?usp=sharing)
| Community Meeting Calendar | Tuesdays 10:00a-10:30a EDT <br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com)|
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1zydqnsw2ty5siL_FT2U7klMTK7OuKWRZNmkUJMx3cWE/edit?usp=sharing)                            |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1Ebe9blQDgDjFOylqAtUe85UNecEfOzes?usp=sharing)                           |
| Slack Channel              | [#knative-functions](https://cloud-native.slack.com/archives/C04LKEZUXEE) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                    |
| Github Team WG leads       | [@knative/func-wg-leads](https://github.com/orgs/knative/teams/func-wg-leads/members)                                                                       |

| &nbsp;                                                           | Leads           | Company | Profile                                           |
| ---------------------------------------------------------------- | --------------- | ------- | ------------------------------------------------- |
| <img width="30px" src="https://github.com/lkingland.png"> | Luke Kingland    | Red Hat     | [lkingland](https://github.com/lkingland) |
| <img width="30px" src="https://github.com/salaboy.png"> | Mauricio Salatino    | VMWare     | [salaboy](https://github.com/salaboy) |

| &nbsp;                                                     | Emeritus Leads | Profile                                     | Duration  |
| ---------------------------------------------------------- | -------------- | ------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/lance.png">   | Lance Ball    | [lance](https://github.com/lance)     | 2022-2023 |


## Operations

Managing, assessing system health and maintaining Knative clusters

| Artifact                   | Link                                                                                                                                                       |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter                    | [Charter](./operations/CHARTER.md)                                                                                                                         |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                        |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1m9oFlelI292Fzwi_sRUTrf69I-CcCwEVXkGcMAjDYqM/edit)                                   |
| Community Meeting Calendar | Tuesdays at 10:00am PST <br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1m9oFlelI292Fzwi_sRUTrf69I-CcCwEVXkGcMAjDYqM/edit)                                                              |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1GgBCtyWWGx8v8PHGbzJ_tu7DROyBl6x7)                                                                         |
| Repo prefixes              |                                                                                                                                                            |
| Slack Channel              | [#knative](https://cloud-native.slack.com/archives/C04LGHDR9K7) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                              |
| Github Team WG leads       | [@knative/operations-wg-leads](https://github.com/orgs/knative/teams/operations-wg-leads/members)                                                          |

| &nbsp;                                                     | Leads       | Company | Profile                                     |
| ---------------------------------------------------------- | ----------- | ------- | ------------------------------------------- |
| <img width="30px" src="https://github.com/houshengbo.png"> | Vincent Hou | Bloomberg | [houshengbo](https://github.com/houshengbo) |

| &nbsp;                                                     | Emeritus Leads | Profile                                     | Duration  |
| ---------------------------------------------------------- | -------------- | ------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/k4leung4.png">   | Kenny Leung    | [k4leung4](https://github.com/k4leung4)     | 2019-2020 |
| <img width="30px" src="https://github.com/bbrowning.png">  | Ben Browning   | [bbrowning](https://github.com/bbrowning)   | 2019-2020 |
| <img width="30px" src="https://github.com/greghaynes.png"> | Greg Haynes    | [greghaynes](https://github.com/greghaynes) | 2019-2019 |

## Productivity

Project health, test framework, continuous integration & deployment, release,
performance/scale/load testing infrastructure

| Artifact                   | Link                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter                    | [Charter](./productivity/CHARTER.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/40/views/4)                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/16go22yTCiaNBtdjghhrqSxnsWkMbxRs4i_gSIezGzUk/edit)                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Community Meeting Calendar | bi-weekly, Wednesday, 8am EDT (12am UTC, 2pm CEST)<br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com)                                                                                                                                                                                                                                                                                                                                                                                     |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1aPRwYGD4XscRIqlBzbNsSB886PJ0G-vZYUAAUjoydko)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1_1oWL7skjVt2211T0aagpwzDEfWmEIQK)                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Repo prefixes              | `actions-*`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Repos                      | [`knative/hack`](https://github.com/knative/hack), [`knative/test-infra`](https://github.com/knative/test-infra), [`knative-extensions/.github`](https://github.com/knative-extensions/.github), [`knative-extensions/reconciler-test`](https://github.com/knative-extensions/reconciler-test), [`knative-extensions/knobots`](https://github.com/knative-extensions/knobots) |
| Slack Channel              | [#knative-productivity](https://cloud-native.slack.com/archives/C04LY4M2G49) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Github Team WG leads       | [@knative/productivity-wg-leads](https://github.com/orgs/knative/teams/productivity-wg-leads/members)                                                                                                                                                                                                                                                                                                                                                                                                                                     |

| &nbsp;                                                   | Leads            | Company   | Profile                                 |
| -------------------------------------------------------- | ---------------- | --------- | --------------------------------------- |
| <img width="30px" src="https://github.com/upodroid.png">  | Mahamed Ali     | Cisco     | [upodroid](https://github.com/upodroid) |
| <img width="30px" src="https://github.com/cardil.png">    | Chris Suszynski | Red Hat   | [cardil](https://github.com/cardil) |

| &nbsp;                                                    | Emeritus Leads | Profile                                   | Duration  |
| --------------------------------------------------------- | -------------- | ----------------------------------------- | --------- |
| <img width="30px" src="https://github.com/krsna-m.png">  | Krsna Mahapatra  | [krsna-m](https://github.com/krsna-m)   | 2022-2024  |
| <img width="30px" src="https://github.com/chizhg.png">    | Chi Zhang      | [chizhg](https://github.com/chizhg)       | 2020-2022    |
| <img width="30px" src="https://github.com/n3wscott.png">  | Scott Nichols  | [n3wscott](https://github.com/n3wscott)   | 2020-2021 |
| <img width="30px" src="https://github.com/chaodaiG.png">  | Chao Dai       | [chaodaiG](https://github.com/chaodaiG)   | 2019-2020 |
| <img width="30px" src="https://github.com/jessiezcc.png"> | Jessie Zhu     | [jessiezcc](https://github.com/jessiezcc) | 2018-2019 |
| <img width="30px" src="https://github.com/adrcunha.png">  | Adriano Cunha  | [adrcunha](https://github.com/adrcunha)   | 2018-2020 |

## Security

Security concerns across Knative components

| Artifact                   | Link                                                                                                                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Charter / Mission          | [Charter](https://docs.google.com/document/d/194bECSbxPIONzhgGj1g9tccUsP8I-M7WIvbBqcT-tXY/edit)                                                        |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                    |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1b-aCADlUBo2FZEDp5z5XoXlfUT6CvED339fcAdKY66o/edit)                               |
| Community Meeting Calendar | Every other Monday at 8:30am PST <br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1b-aCADlUBo2FZEDp5z5XoXlfUT6CvED339fcAdKY66o/edit)                                                          |
| Document Folder            | [Folder](https://drive.google.com/drive/u/0/folders/1yOy_yU5vvUTFuxeYvhlY7uzIL4c4SSzX)                                                                 |
| Repo prefixes              |                                                                                                                                                        |
| Slack Channel              | [#knative-security](https://cloud-native.slack.com/archives/C04LGJ0D5FF) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                                                                                              |
| Github Team WG leads       | [@knative/security-wg-leads](https://github.com/orgs/knative/teams/security-wg-leads/members)                                                          |

| &nbsp;                                                        | Leads           | Company | Profile                                           |
| ------------------------------------------------------------- | --------------- | ------- | ------------------------------------------------- |
| <img width="30px" src="https://github.com/evankanderson.png"> | Evan Anderson   | VMware  | [evankanderson](https://github.com/evankanderson) |
| <img width="30px" src="https://github.com/davidhadas.png">    | David Hadas     | IBM     | [davidhadas](https://github.com/davidhadas)       |

| &nbsp;                                                     | Emeritus Leads | Profile                                     | Duration  |
| ---------------------------------------------------------- | -------------- | ------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/julz.png">          | Julian Friedman |[julz](https://github.com/julz)                   | 2021-2022 |

---

# Emeritus Working Groups

## Documentation

Documentation concerns across Knative -
especially the [Docs](https://github.com/knative/docs/) repo.

| Artifact                   | Link                                                                                                                                                             |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter / Mission          | [Charter](https://docs.google.com/document/d/1-opvSEzJMRbB6fybvjuCyhFBZvHwXnkbgyOIzjlmrpo/edit)                                                                  |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative/projects/20)                                                                                                           |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                                                              |
| Community Meeting VC       | See the top of the [Meeting notes](https://docs.google.com/document/d/1NSlGHen5Dh6c2A0LGavGWibddWrlSLV_PbEbMpNjSTU/edit?usp=sharing)                             |
| Community Meeting Calendar | Every other Tuesday from 9:30-10:30am PST <br>[Calendar](https://calendar.google.com/calendar/embed?src=knative.team_9q83bg07qs5b9rrslp5jor4l6s%40group.calendar.google.com) |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1NSlGHen5Dh6c2A0LGavGWibddWrlSLV_PbEbMpNjSTU/edit?usp=sharing)                                                        |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1XzZGqV7yHo38d_l7rH1uSIrbQp3JlbBP?usp=sharing)                                                                   |
| Slack Channel              | [#knative-documentation](https://cloud-native.slack.com/archives/C04LY5G9ED7) (need to join [CNCF Slack](https://slack.cncf.io/) for the first time)                            |
| Github Repository          | [/docs](https://github.com/knative/docs)                                                                                  |
| Github Team WG leads       | [@knative/ux-wg-leads](https://github.com/orgs/knative/teams/ux-wg-leads/members)                                                                                |

| &nbsp;                                                        | Leads            | Company  | Profile                                           | Duration  |
| ------------------------------------------------------------- | ---------------- | -------- | ------------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/snneji.png">        | Samia Nneji      | VMware   | [snneji](https://github.com/snneji)               | 2021-2023 |
| <img width="30px" src="https://github.com/abrennan89.png">    | Ashleigh Brennan | Red Hat  | [abrennan89](https://github.com/abrennan89)       | 2020-2023 |
| <img width="30px" src="https://github.com/samodell.png">      | Sam O'Dell       | Google   | [samodell](https://github.com/samodell)           | 2018-2020 |

## Eventing Kafka

The Eventing Kafka was a dedicated working group for Kafka-based Knative Eventing components. In 2023 it has been merged back into the parent Eventing working group.

| Artifact                   | Link                                                                                                                     |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------|
| Charter / Mission          | [Charter](/working-groups/kafka/CHARTER.md)                                                                              |
| Roadmap                    | [Roadmap](https://github.com/orgs/knative-extensions/projects/8)                                                            |
| Forum                      | [knative-dev@](https://groups.google.com/forum/#!forum/knative-dev)                                                      |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1ykBVPtiosGoDjzBklMt9HxbinGrMod6itOvfe6DeVmA/edit)                            |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/1ra5czyKOaMsWuwWXzkhce6_g6rFBdCxg?usp=sharing)                           |

| &nbsp;                                                           | Leads           | Profile                                                 | Duration  |
| ---------------------------------------------------------------- | --------------- | ------------------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/travis-minke-sap.png"> | Travis Minke    | [travis-minke-sap](https://github.com/travis-minke-sap) | 2022      |
| <img width="30px" src="https://github.com/devguyio.png">         | Ahmed Abdalla   | [devguyio](https://github.com/devguyio)                 | 2021-2022 |
| <img width="30px" src="https://github.com/lionelvillard.png">    | Lionel Villard  | [lionelvillard](https://github.com/lionelvillard)       | 2021-2022 |

## Build

| &nbsp;                                                   | Leads      | Profile                                 | Duration  |
| -------------------------------------------------------- | ---------- | --------------------------------------- | --------- |
| <img width="30px" src="https://github.com/ImJasonH.png"> | Jason Hall | [ImJasonH](https://github.com/ImJasonH) | 2018-2019 |

## Event Delivery (previously called Eventing Channels Working Group)

| &nbsp;                                                          | Leads               | Profile                                               | Duration  |
| --------------------------------------------------------------- | ------------------- | ----------------------------------------------------- | --------- |
| <img width="30px" src="https://github.com/harwayne.png">        | Adam Harwayne       | [Harwayne](https://github.com/harwayne)               | 2019-2021 |
| <img width="30px" src="https://github.com/matzew.png">          | Matthias Wessendorf | [matzew](https://github.com/matzew)                   | 2019-2021 |
| <img width="30px" src="https://github.com/slinkydeveloper.png"> | Francesco Guardiani | [slinkydeveloper](https://github.com/slinkydeveloper) | 2020-2021 |

## Eventing Sources

The Eventing Sources working group was responsible for various event producers, and has been started to split up the initial work to ramp up those soures. In 2022 it has been merged back into the parent Eventing working group.

| Artifact                   | Link                                                                                                                                                       |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Charter                    | [Charter](./sources/CHARTER.md)                                                                                                                            |
| Meeting Notes              | [Notes](https://docs.google.com/document/d/1Xha-FeunojN49OJN7W0WBnPMcRtp1ycYpbkiir6XsE0/edit#) [(Notes before March 2021)](https://docs.google.com/document/d/19txVRqA6_eY6ClGqoLRa0gPB50Ok7PT6_B6zDP1KtKQ/edit)                                                          |
| Document Folder            | [Folder](https://drive.google.com/drive/folders/13idi0QRqj1vsp5X0vDGfUOULhIyeeLaG)                                                                         |

| &nbsp;                                                    | Emeritus Leads       | Profile                                   | Duration  |
| --------------------------------------------------------- | -------------------- | ----------------------------------------- | --------- |
| <img width="30px" src="https://github.com/lionelvillard.png"> | Lionel Villard | [lionelvillard](https://github.com/lionelvillard) | 2019-2022 |
| <img width="30px" src="https://github.com/nachocano.png"> | Ignacio (Nacho) Cano | [nachocano](https://github.com/nachocano) | 2019-2020 |
| <img width="30px" src="https://github.com/vaikas.png">    | Ville Aikas          | [vaikas](https://github.com/vaikas)       | 2019-2021 |
| <img width="30px" src="https://github.com/n3wscott.png">  | Scott Nichols        | [n3wscott](https://github.com/n3wscott)   | 2019-2021 |

## Observability

| &nbsp;                                                    | Leads            | Profile                                   | Duration  |
| --------------------------------------------------------- | ---------------- | ----------------------------------------- | --------- |
| <img width="30px" src="https://github.com/mdemirhan.png"> | Mustafa Demirhan | [mdemirhan](https://github.com/mdemirhan) | 2018-2019 |

Except as otherwise noted, the content of this page is licensed under the
[Creative Commons Attribution 4.0 License](https://creativecommons.org/licenses/by/4.0/),
and code samples are licensed under the
[Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).
