# CRAYS

### Build the software connecting people, places and everyday operations.

CRAYS brings together personal tools, community membership and the software needed to run clubs, hospitality and business projects. We build the web experiences, native interfaces and integrations that connect those worlds: a member's account, a guest's view of a property, an operator's project work, or the accounting consequence of a commerce event.

<a id="architecture"></a>

## Architecture: applications, Core/BCC and independent services

**Target architecture · AWS integration in progress.** CRAYS connects application APIs, including GraphQL, to **Core/BCC identity, accounts, permissions and business rules**, then to independently operated services.

~~~mermaid
flowchart TD
    UI["Web / mobile: Pro · Personal<br/>Member / Club · Work / SaaS"] --> API["CRAYS application APIs / GraphQL"]
    API --> Core["Core / BCC: identity, accounts,<br/>permissions and business rules"]
    Core --> Adapters["CRAYS BFFs and service adapters"]
    Adapters --> Services["Independent service APIs and runtimes"]
    Services --> Business["Plane · Vendure · Frappe / ERPNext · Qlo"]
    Services --> Collaboration["Nextcloud · Postiz"]
    Services --> Chuck["Chuck: personal intelligence"]
    Chuck -. "documented component relationship" .-> OpenClaw["OpenClaw agent components"]
    Core --> RDS["Core data: RDS PostgreSQL"]
    Services --> Data["Service-owned databases and file storage"]
    classDef crays fill:#fff1f2,stroke:#b42335,color:#202124;
    class API,Core,Adapters crays;
~~~

In plain terms: the application asks for an operation; Core/BCC establishes its account and business authority; an adapter calls the responsible service. A **backend-for-frontend (BFF)** shapes application-specific requests and responses. It is distinct from Core/BCC and does not replace provider permissions.

**GraphQL is an application interface; not every provider uses GraphQL.** Plane handles projects, Vendure commerce, Frappe/ERPNext business and finance, Qlo hospitality, Nextcloud files/collaboration and Postiz publishing. Chuck has separate consumer, agent and workflow boundaries; OpenClaw supplies documented agent components rather than being the same product. Twenty is [archived and no longer used](https://github.com/CraysWorld/.github/blob/main/docs/legacy-projects.md); any CRM reintroduction would be a separately qualified plan.

The storage direction replaces **Neon PostgreSQL with Amazon RDS PostgreSQL** for Core data, while services retain appropriate PostgreSQL or MySQL/MariaDB databases. S3 adds object/file storage alongside provider-specific file services. These are architectural responsibilities, **not proof that every connection or end-to-end workflow is implemented or live**.

[Visual architecture guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/architecture.md) · [Member GraphQL source](https://github.com/CraysWorld/crays-platform/blob/main/services/member-club/source50/README.md) · [BFF source and contracts](https://github.com/CraysWorld/crays-platform/blob/main/services/clubs-commerce-bff/README.md) · [Service catalog](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/README.md)

Our work combines **CRAYS applications** with **open-source business, collaboration, commerce and agent systems**. The interesting engineering happens at their boundaries: which account is acting, which company or property an action belongs to, how a provider acknowledges it, and what the interface should show when the result is still uncertain.

This is where developers can understand that work, inspect the implementation and help improve it.

**[Explore the platform](https://github.com/CraysWorld/crays-platform) · [Understand the architecture](https://github.com/CraysWorld/crays-platform/blob/main/docs/architecture.md) · [Choose a contribution](https://github.com/CraysWorld/crays-platform/blob/main/CONTRIBUTING.md) · [Find a repository](https://github.com/CraysWorld/.github/blob/main/docs/repositories.md)**

[Architecture](#architecture) · [CRAYS Pro](#crays-pro--the-business-and-franchise-front-door) · [Personal, Chuck and OpenClaw](#personal-chuck-and-openclaw) · [Member and Club](#member-and-club) · [Work and business services](#work-and-business-services) · [Nostr and mobile](#nostr-mobile-and-connectivity) · [Websites](#the-crays-website-portfolio) · [Get involved](#build-with-us)

## CRAYS Pro — the business and franchise front door

**CRAYS Pro gives the business side of the ecosystem a public starting point.** Its frontend introduces the Coffee, Retail, Gym and Clubs concepts and provides distinct routes for property owners, franchise candidates, operating partners, financing partners, investors, vendors and suppliers.

The source describes a journey from understanding a concept and its property fit to introducing a property, reviewing opportunity information and choosing the relevant business relationship. Separate pages explain partner roles, the franchise process, account/portal entry and contact routes. This makes Pro a place to explain how CRAYS projects fit together for the people who may operate, supply or develop them.

For developers, the public Next.js source offers concrete work on navigation, concept pages, relationship entry, accessibility, localization and clear public/private information boundaries. The public frontend is separate from the deeper Franchise Manager and Targomo integrations.

**[Visit crays.pro](https://www.crays.pro)** · **[Explore CRAYS Pro source](https://github.com/CraysWorld/crays-pro)** · [Read its page and audience map](https://github.com/CraysWorld/crays-pro/blob/main/src/lib/crays-pro-public-metadata.ts) · [Development guide](https://github.com/CraysWorld/crays-pro/blob/main/docs/development-and-recovery.md)

## The experiences we connect

| Experience | Who it is for | What you can explore here |
| --- | --- | --- |
| **Personal** | People using their own CRAYS workspace | Personal interfaces, Chuck task interactions, training views and social/Nostr connections. |
| **Member and Club** | Members, guests and community participants | Membership interfaces, account/session boundaries, documents and provider-backed activities. |
| **Work** | Teams and operators | Project work, finance, collaboration and the operational consequences of commerce and hospitality activity. |
| **Pro** | Business and franchise participants | Public concepts, property and partner routes, business information and relationship entry. |

These are related experiences with different responsibilities. The sections below describe published implementation and documented integration work; individual guides explain their current development scope.

## Personal, Chuck and OpenClaw

Personal is the application workspace for an individual's tools and interactions. Its separate React/Vite frontend includes personal workspaces, training views, social interfaces and an embedded Member integration.

**Chuck is the personal-intelligence integration around that experience.** Application interactions meet separately maintained agent, broker, tool and workflow layers. The public frontend includes application connections, task starters and task-review links, so contributors can begin with a visible interaction and trace its contract toward the layer responsible for execution.

**OpenClaw has a concrete place in this agent work.** The published Personal-agent materializer records OpenClaw channel/startup, tool, reminder and reply-related components, including separate WhatsApp variants and CRAYS modifications. Its source map retains the original upstream and notice relationships. These are underlying implementation pieces; Chuck describes the broader CRAYS personal-intelligence integration, and Personal is the application experience. The complete current agent/broker environment has its own integration work.

Useful work here includes clearer task states, permission boundaries, tool contracts, review interfaces and synthetic tests that connect an application action to its expected outcome.

[Personal source](https://github.com/CraysWorld/crays-platform/blob/main/apps/personal/README.md) · [Personal and Chuck guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/personal-and-chuck.md) · [OpenClaw components and modifications](https://github.com/CraysWorld/crays-platform/blob/main/third-party/personal-agent-materializer/README.md) · [Task starters](https://github.com/CraysWorld/crays-platform/blob/main/apps/personal/source/src/chuckPublicStarters.mjs)

## Member and Club

Member and Club connect public discovery and community experiences to accounts, membership and provider-backed activities. Their implementation includes a shared Next.js application and a separately built Club/Member browser module.

A central engineering concern is preserving the relationship between the person signing in, the CRAYS application session and the provider principal acting on a particular request. Auth0 integration, CRAYS session mapping and the individual providers each have their own responsibilities. A signed-in account does not automatically become permission to access every document, business entity or service.

Published code gives contributors entry points into account/session handling, member document contracts, commerce interfaces and provider error states. Frontend, API and identity contributors can improve these flows with synthetic identities and clearly scoped provider responses.

[Shared web application](https://github.com/CraysWorld/crays-platform/blob/main/apps/web/README.md) · [Club/Member browser module](https://github.com/CraysWorld/crays-platform/blob/main/modules/club-member/README.md) · [Identity and Auth0 guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/identity.md)

## Work and business services

Work connects business activity to the systems responsible for projects, finance, documents and hospitality. CRAYS adds the contracts and adapters that carry company/property scope, correlate requests with their source records and distinguish an acknowledgement from a completed outcome.

### Projects with Plane

**Plane is the project and work-item provider for the Project area within Work.** CRAYS code prepares scoped work items, dispatches them to the intended workspace/project and reconciles signed webhook responses. Hospitality exception work is one of the documented integration paths.

This is useful engineering territory for contributors interested in reliable integrations: duplicate delivery, timeout handling, webhook validation and understandable submitted/accepted/reconciled states. Plane has one canonical home in this architecture.

[Plane integration](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/plane.md) · [Work-item adapter](https://github.com/CraysWorld/crays-platform/blob/main/apps/web/src/lib/member-commerce/plane-work-item-adapter.ts)

### Finance and business applications with Frappe / ERPNext

**ERPNext provides the finance/ERP domain; CRAYS connects commerce events to the appropriate accounting context.** The integration carries tenant, legal-entity, store, ERP-site and company scope and keeps queued consequences, provider responses and reconciled results distinguishable.

The recorded Frappe installation contains more than ERP alone: CRM, HRMS, Helpdesk, Insights, Lending, Drive, Gameplan, Builder, Payments, LMS, Telephony and Press are also in its installed-app set. That is an installed suite, not a declaration that every application's workflow is finished or enabled for every CRAYS user.

The CRAYS Team Scope extension adds another concrete contribution area: request hooks and policy constraints for dedicated synthetic test service principals. Its original Python source is available alongside the commerce-to-ERP adapters.

[Frappe / ERPNext guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/frappe.md) · [CRAYS Team Scope source](https://github.com/CraysWorld/crays-platform/blob/main/services/frappe/custom-apps/crays_team_scope/README.md) · [Commerce-to-ERP adapter](https://github.com/CraysWorld/crays-platform/blob/main/apps/web/src/lib/member-commerce/frappe-commerce-adapter.ts)

### Files and collaboration with Nextcloud

Nextcloud is the cloud-file and collaboration service family behind CRAYS document integrations. Our code handles member document relationships, WebDAV transport, byte/hash readback and scoped collaboration-group access.

The broader collaboration scope includes **Talk/calls, Office and Whiteboard**. Their provider/app and user-flow validation is separate from the narrower published document and access adapters. The documented member-document implementation is a protected test-authority path, giving contributors a specific starting point rather than an unrestricted upload service.

Contributions can improve document-state interfaces, byte/readback mismatch handling, ownership errors and membership reconciliation.

[Nextcloud integration](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/nextcloud.md) · [Member document provider](https://github.com/CraysWorld/crays-platform/blob/main/apps/web/src/lib/clubs/member-nextcloud-document-provider.ts)

## Commerce with Vendure

**Vendure is the commerce provider in the documented Member/Club integration.** The CRAYS Clubs Commerce BFF separates application-facing requests from provider operations, with contracts for commerce sessions, holds, carts and orders.

The architecture keeps different responsibilities visible: Vendure's commerce state, Booking Core's holds/bookings/capacity, ERPNext's accounting consequences and Plane's follow-up work. An event crossing those boundaries needs correlation and reconciliation, not an assumption that one provider's response completes the whole business process.

The published BFF implementation, original tests and dependency notices make this a practical area for API-contract examples, synthetic integration tests and safe response handling. Payment, fulfillment and current provider acceptance retain their own development status.

[Commerce and Vendure guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/commerce.md) · [Clubs Commerce BFF](https://github.com/CraysWorld/crays-platform/blob/main/services/clubs-commerce-bff/README.md)

## Hospitality with Qlo

The Qlo integration connects hotel content, room descriptions, property services and provider media to CRAYS-facing interfaces. The CRAYS gateway supplies a session boundary and projections for that information.

Content discovery and bookable inventory are different responsibilities. The documented room projection explicitly keeps booking, rates, availability and channel-manager/payment setup pending. Developers can improve the gateway and guest-facing presentation while keeping those states accurate.

Qlo is also a useful first contribution: the two small local projection tests use synthetic in-memory fixtures, without provider credentials or a running hospitality service.

[Qlo guide and first local check](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/qlo.md#first-local-check-the-two-projection-tests) · [Gateway implementation](https://github.com/CraysWorld/crays-platform/blob/main/services/qlo-gateway/README.md) · [Work/Qlo runtime](https://github.com/CraysWorld/crays-platform/blob/main/services/work-qlo-runtime/README.md)

## Gym and training

Gym gives training-focused experiences a place within the broader Personal workspace. The public Personal frontend contains Gym/training views; the wider Gym project and its evolving integrations have separate source responsibilities.

Frontend contributors can work on accessible training interfaces, clear workflow states, localization and documentation tied to the correct application layer. Begin with the public Personal source guide and the project map to understand which part of Gym a change affects.

[Personal frontend and Gym views](https://github.com/CraysWorld/crays-platform/blob/main/apps/personal/README.md) · [Gym project orientation](https://github.com/CraysWorld/.github/blob/main/docs/repositories.md#websites-and-web-applications)

## Nostr, mobile and connectivity

CRAYS's decentralized communication work spans web and native experiences. **Net** is the Primal-derived web application; Personal contains Nostr-facing interactions. The relay and Blossom blob-service layers have separate implementations and source responsibilities.

This separation matters when contributing: an application interaction, event transport, blob storage and access policy solve different problems. Public entry points include the Net application/hosting composition, Nostr identity and signature/session contracts, and Personal interaction interfaces.

Native work includes the CRAYS iOS application, separate Circle iOS and Android projects, BLE source and nearby-connectivity work. Use the mobile map to choose the project and understand its current access and integration scope.

[Network/Nostr guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/network.md) · [Net application source](https://github.com/CraysWorld/crays-web-codex) · [Mobile and connectivity projects](https://github.com/CraysWorld/.github/blob/main/docs/repositories.md#mobile-applications)

## Creator tools and Postiz delivery

Personal includes creator-studio and publishing interfaces. Postiz is a separate social-publishing delivery service family with frontend/API, Temporal workflows, PostgreSQL, Elasticsearch and Redis responsibilities.

The useful contribution question is how a draft or reviewed action becomes an authorized delivery request, which worker owns it and what happens after a timeout or retry. The interface and provider records are documented separately; their presence alone does not establish a completed end-to-end publishing integration.

[Creator and Postiz guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/delivery-and-social.md) · [Creator studio source](https://github.com/CraysWorld/crays-platform/blob/main/apps/personal/source/src/WebCreatorStudio.tsx)

## The CRAYS website portfolio

Eleven website compositions give different parts of the ecosystem their own entry points:

| Portfolio area | Websites and source orientation |
| --- | --- |
| Community, hospitality and personal activity | **Club, Coffee and Gym.** [Club](https://github.com/CraysWorld/crays-club) and [Coffee](https://github.com/CraysWorld/crays-coffee) have public website repositories; shared Club/Member and Personal/Gym implementation also lives in the platform. |
| Business and commerce | **Pro and Shop.** [Pro](https://github.com/CraysWorld/crays-pro) presents concepts and business relationships; [Shop](https://github.com/CraysWorld/crays-shop) contains the storefront source. |
| Association and network | **Org and Net.** [Org](https://github.com/CraysWorld/crays-org) includes multilingual association pages and Nostr/ecosystem directories; [Net](https://github.com/CraysWorld/crays-web-codex) retains the Primal-derived web project. |
| Wider portfolio | **Fund, World, Award and Fun.** The [website map](https://github.com/CraysWorld/.github/blob/main/docs/repository-structure.md#eleven-website-compositions) records their individual source relationships and remaining access/destination work. |

Website count and repository count are different. Shared applications belong in the platform; independent sites keep their own project context. The [repository guide](https://github.com/CraysWorld/.github/blob/main/docs/repositories.md) explains where to make a change.

## How the software fits together

| Layer | Responsibility | Developer entry |
| --- | --- | --- |
| Applications | Personal, Club/Member, native clients and independent websites present the user experience. | [Application map](https://github.com/CraysWorld/crays-platform/blob/main/README.md#find-a-component) |
| CRAYS integration code | Account/session mapping, document contracts, company/property scope, commerce consequences, provider adapters and webhook reconciliation. | [Service hub](https://github.com/CraysWorld/crays-platform/blob/main/docs/services/README.md) |
| Provider and agent systems | Frappe/ERPNext, Nextcloud, Plane, Vendure, Qlo, Postiz and the separately documented Chuck/OpenClaw layers retain their own responsibilities. | [Architecture guide](https://github.com/CraysWorld/crays-platform/blob/main/docs/architecture.md) |

The stack spans Next.js/React web code, a React/Vite Personal frontend, TypeScript/JavaScript services, Python integration code and native projects. Storage, queues and runtime dependencies belong to the relevant component's setup. There is no single command that installs and starts the entire ecosystem.

## Build with us

You do not have to understand every service before making a useful contribution.

| If you care about… | A concrete place to begin |
| --- | --- |
| A small first code change | Add a synthetic malformed-input case in the [Qlo projection-test exercise](https://github.com/CraysWorld/crays-platform/blob/main/CONTRIBUTING.md#a-small-first-test). |
| Personal tools and agents | Trace a [Chuck task starter](https://github.com/CraysWorld/crays-platform/blob/main/apps/personal/source/src/chuckPublicStarters.mjs) to its task/review contract; improve the interface or document its permission boundary. |
| Business-facing experiences | Improve [Pro navigation and public pages](https://github.com/CraysWorld/crays-pro), accessibility or the clarity of relationship entry. |
| Reliable business integrations | Add synthetic company-scope, timeout, duplicate-delivery or signed-webhook cases using the Frappe and Plane guides. |
| Documents and collaboration | Improve Nextcloud ownership/error states, WebDAV readback tests or group-membership reconciliation examples. |
| Web/mobile experience | Choose an application from the project map and work on accessibility, localization, interface states or integration documentation. |
| Open-source maintenance | Map exact upstream versions and CRAYS changes, preserve original notices and improve reproducible component setup. |

Start with [Contributing](https://github.com/CraysWorld/crays-platform/blob/main/CONTRIBUTING.md). Pick one component, read its setup requirements, use synthetic test data and describe the result you expect. The [platform issue tracker](https://github.com/CraysWorld/crays-platform/issues) is a place to propose a concrete problem or improvement; independent projects use their own repository.

## Source, licenses and development status

CRAYS-specific work and the upstream projects it connects remain identifiable. Original authorship, licenses and notices apply per component; explicit CRAYS-owned grants are documented in the [component license map](https://github.com/CraysWorld/crays-platform/blob/main/LICENSING.md). This profile does not add a blanket license.

Development and source publication are continuing. A published implementation describes inspectable work, not a promise that every integration is enabled or accepted in a current deployment. [Source and license status](https://github.com/CraysWorld/.github/blob/main/docs/source-and-license-status.md) records remaining work. [Historical projects](https://github.com/CraysWorld/.github/blob/main/docs/legacy-projects.md), including Twenty and OpenProject, are kept separate from the current product map.
