# CRM API and automation walkthrough

[← Return to the showcase](../README.md)

The integration connects a WordPress customer experience to Zoho CRM through a shared server-side client. Company configuration, CRM mappings, customer identity, and operational membership remain distinct responsibilities.

## Request to CRM

1. Collect project type, goals, scope, service details, property context, photos, and contact information.
2. Save the request and its stable identifier locally before optional account setup.
3. Send the mapped Lead payload through the governed transport. A unique request key identifies retries of the same request.
4. Offer optional enrollment with mailbox verification. A matching email alone does not attach historical requests.
5. Read configured CRM progress only after checking request identity and ownership. Staff overrides remain authoritative until explicitly returned to CRM control.
6. Reconcile converted customers and project membership through a separate staff process. Lead conversion is not an automatic access grant.

These are documented implementation behaviors and contracts. The complete live request, delivery, invitation, returning-status and conversion sequence still requires a controlled acceptance run on the deployed versions.

## Integration responsibilities

| Layer | Responsibility |
|:---|:---|
| Brand and installation policy | Company identity, supported services, accepted state rules |
| Project intake | Durable receipt, uploads, request identifier, delivery state |
| Shared CRM client | Server-side OAuth, API budget, cache and circuit behavior |
| Customer enrollment | Verified identity and pending account approval |
| Operational portal | Explicit customer membership and authorized project access |
| Public property enrichment | Source provenance and reviewable suggestions |

## What the reviewed evidence supports

The October 16 read-only review demonstrated working administrative operational CRM reads and existing WordPress service requests linked to matching Zoho Cases. It confirmed enabled Lead delivery configuration and configured progress synchronization. It did not demonstrate a new production Lead transaction or a completed live customer invitation journey.

Cases evidence establishes existing outbound delivery. It does not establish complete two-way conversation, assignment, or lifecycle synchronization. Role synchronization workflows were configured; a fresh event and revocation sequence remained to be tested.

## Handling failure deliberately

The documented design preserves a local receipt, retries remote delivery using stable identity, and governs remote requests rather than assuming unlimited API capacity. Caching and throttling can delay visible updates. Immediate synchronization, measured throughput, guaranteed delivery time, and business-outcome improvements are not claimed without corresponding acceptance measurements.

The portfolio demonstrates architecture, implementation decisions, and bounded verification. It publishes no authenticated endpoints, account identifiers, payload captures, customer records, or credentials.
