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

## Checks and their limits

The October 16 review observed authentication requirements on selected identity APIs and a login redirect on the crew entry route. Selected portal responses carried private/no-store headers. These checks establish behavior for the inspected paths and time, rather than proving every endpoint or every role combination.

The remaining release work includes ordinary-user role testing, cross-customer denial, access revocation, controlled signed-document release, and recovery verification. Security and compatibility require revalidation after relevant changes.

No independent penetration test, regulatory certification, universal authorization guarantee, or recovery-time commitment is asserted by this showcase. Avoid posting credentials, customer information, or sensitive security details in public issues.
