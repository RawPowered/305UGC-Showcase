# Security and access practices

[← Return to the showcase](../README.md)

The security story is a set of specific engineering boundaries. A successful login, account approval, or CRM match should not silently authorize every customer or staff record.

| Boundary | Approach |
|:---|:---|
| Authentication | WordPress sessions establish the signed-in identity |
| Feature access | Role and capability checks limit module access |
| Record access | Module-specific membership, assignment, status and ownership checks narrow the allowed records |
| Protected changes | Nonce checks protect applicable form handlers, alongside authorization |
| Customer enrollment | Mailbox verification and explicit request attachment; email matching alone is insufficient |
| Customer projects | Account approval, request approval and operational job membership are separate decisions |
| CRM credentials | OAuth access stays in server-side integration components |
| Portal caching | Private/no-store responses on the portal routes inspected in the October 16 review |
| Private documents | Protected storage, controlled release and authorized download paths; document release still needs acceptance evidence |
| Portfolio publishing | Public pages and fictional demonstration records only; no production exports or installable software |

## Website-level protection and maintenance

Security review extends to the 305UGC website and its hosting, as well as portal permissions:

| Measure or review | What the evidence establishes |
|:---|:---|
| HTTPS delivery | The inspected public site and portal were served over HTTPS on October 24; no claim about every TLS or redirect setting is made |
| Portal response privacy | The October 24 customer-portal response included private/no-store caching, `noindex, nofollow`, and `Referrer-Policy: no-referrer` |
| Login and firewall tooling | The October 16 deployment review recorded Loginizer Pro and Wordfence administration; their presence is not proof of completed hardening or protection against every attack |
| WordPress core integrity | An October 21 assessment recorded a successful core checksum verification, with additional warnings requiring review; this did not verify all plugins, uploads or database content |
| Public access regression | The October 21 assessment recorded 12/12 scoped public HTTP assertions passing, including anonymous identity denial and crew login redirection |
| Protected changes and private uploads | Application-level authorization, applicable nonce checks and controlled document-release rules complement hosting measures |
| Recovery readiness | Backup and isolated-restore verification remain release requirements; installed backup tooling is not itself evidence of a recoverable backup |
| Hosting maintenance | Provider remediation and subsequent runtime validation remained unverified in the October 21 assessment; this showcase does not mark them complete |

The portfolio omits sensitive diagnostic details and internal infrastructure identifiers. It does not publish exploit information or portray an unresolved maintenance review as completed remediation. A fresh maintenance and security acceptance review is required before asserting that outstanding findings are closed.

## Checks and their limits

The October 16 review observed authentication requirements on selected identity APIs and a login redirect on the crew entry route. Selected portal responses carried private/no-store headers. These checks establish behavior for the inspected paths and time, rather than proving every endpoint or every role combination.

The remaining release work includes ordinary-user role testing, cross-customer denial, access revocation, controlled signed-document release, and recovery verification. Security and compatibility require revalidation after relevant changes.

No independent penetration test, regulatory certification, universal authorization guarantee, or recovery-time commitment is asserted by this showcase. Avoid posting credentials, customer information, or sensitive security details in public issues.
