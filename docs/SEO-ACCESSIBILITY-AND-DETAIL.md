# SEO, accessibility and attention to detail

[← Return to the showcase](../README.md)

The website work extends beyond its visible layout. Metadata, structured content, navigation semantics, crawler guidance, responsive behavior and portal privacy each support a different part of the experience. Public checks below were repeated October 24, 2026; the documented homepage SEO release is dated October 11.

## Search presentation and content structure

| Work completed | Purpose and evidence |
|:---|:---|
| Descriptive homepage SEO title | “Florida Remodeling, Construction & Storm Repair \| 305UGC” aligns the search presentation with the business's current service focus; observed in live sharing metadata |
| Homepage description | A 144-character description introduces remodeling, construction, storm recovery, customer access and a quote action; observed live |
| Self-referencing canonical URLs | Homepage and contact page identify their intended canonical URL; observed live |
| Search and sharing consistency | Open Graph title, description, URL, site identity and selected project imagery give shared links a deliberate presentation |
| Service-oriented content | The October 11 release introduced clearer storm and portal messaging, revised service and portfolio section headings, and replaced internal editorial wording with customer-facing copy |
| Internal navigation | Service, project, storm-recovery and portal links connect relevant topics and next steps |
| Business and service structured data | Live JSON-LD includes LocalBusiness identity and a nine-service OfferCatalog, alongside the existing website, page and breadcrumb entities |
| XML discovery | The sitemap index is reachable and points to content sitemaps; the October 11 review also verified the storm service in the page sitemap |
| Relevant imagery | The release added descriptive disaster-recovery image alt text; live homepage markup includes descriptive image alternatives |

Structured data helps describe the content; it does not guarantee rich results. Metadata and sitemap availability do not establish Google indexing, ranking, traffic or conversion improvements. Search Console acceptance and measured mobile Core Web Vitals remain separate work.

## Blog SEO and publishing continuity

On October 24, the anonymous WordPress post listing returned **12 published guides**, dated September 22–29. Each article and the Guides hub was fetched independently: all **13 pages** returned HTTP 200 with descriptions, self-referencing canonical URLs, index/follow directives and JSON-LD blocks. These are implementation checks, not evidence of Google-selected canonicals, ranking or traffic gains.

Selected public examples:

- [Construction planning: from site walk to project ready](https://305undergroundconstruction.com/2026/09/29/florida-construction-planning-guide-from-site-walk-to-project-ready/)
- [Shingle, metal and tile roof comparisons](https://305undergroundconstruction.com/2026/09/27/shingle-vs-metal-vs-tile-roof-florida/)
- [Home-addition cost and planning guide](https://305undergroundconstruction.com/2026/09/27/florida-home-addition-cost-guide/)
- [Browse the Guides hub](https://305undergroundconstruction.com/guides/)

Original records document a ten-post Buffer queue, a second ten-entry social plan and a later correction of two guide promotions scheduled for September 28–29. The second plan also records queue-capacity pressure; it must not be presented as ten independently confirmed deliveries. These records demonstrate historical publishing work, not a current active schedule or verified delivery of every post.

The newest public article found was September 29. Current scheduled/draft articles, missed schedules, Buffer delivery and the present queue require authenticated review. Future or draft posts cannot be ruled out from a public listing.

## Backlink strategy and measurement

No backlink campaign ledger or referring-domain report was located in the reviewed project records. The portfolio therefore does not claim completed link acquisition or a measured increase in authority. This does not establish that the website has no backlinks.

The next measurable step is an authorized baseline of referring domains and linked pages, followed by a ledger of relevant opportunities, editorial rationale, target resource, approval, placement URL and verification date. Genuine project/supplier credits, relevant local associations and useful original project reporting are potential avenues to evaluate. No outreach, paid listing, placement or resulting link is claimed here.

Avoid buying ranking links, automated link creation, excessive exchanges and low-quality directory submissions. These are covered by [Google's link-spam policies](https://developers.google.com/search/docs/essentials/spam-policies#link-spam).

## Crawler files and AI-readable guidance

Replacement `llms.txt` and `bots.txt` assets were subsequently prepared in the private 305UGC build on October 24. Their release status is **prepared; not verified live**. They are separate website-root assets, so plugin-only deployment does not install them.

| Public path | October 24 observation | Portfolio interpretation |
|:---|:---|:---|
| `/robots.txt` | HTTP 200, with a sitemap reference and portal/operations exclusion lines | Crawler guidance is present, but exclusions precede the `User-agent` group and require grouping review; effective blocking is not claimed |
| `/llms.txt` | HTTP 404 | AI-readable site guidance is not verified as deployed at this path; keep it in the remaining-work list |
| `/bots.txt` | HTTP 404 | No deployed file verified at this path; the site's observed crawler guidance is in `robots.txt` |
| Customer portal | `noindex, nofollow` in meta and HTTP header | Separates the portal's search policy from public marketing pages; this is not an access-control mechanism |

An `llms.txt` file can be documented as completed only after its intended contents and public deployment are verified. No crawler file replaces authentication or guarantees that every bot follows a policy. The sitemap index still lists header and footer template sitemaps; index hygiene needs further review.

Public references: [robots.txt](https://305undergroundconstruction.com/robots.txt), [sitemap index](https://305undergroundconstruction.com/sitemap_index.xml), [homepage](https://305undergroundconstruction.com/).

## ARIA and accessible interface intent

The live homepage, quote page and customer portal contain ARIA markup. The portfolio describes concrete examples rather than treating an attribute count as a quality score.

- **Named regions and controls:** `aria-label` gives navigation, gallery controls and other interface regions an accessible name.
- **Named sections:** `aria-labelledby` associates sections and dialogs with their headings.
- **Expandable navigation:** `aria-expanded` and `aria-controls` expose the intended relationship between a trigger and the area it opens.
- **Status feedback:** quote and portal markup includes `aria-live` regions for dynamic announcements.
- **Decorative content:** `aria-hidden` is present for content intended to be excluded from the accessibility tree.
- **Bypass navigation:** the inspected pages include a skip link.
- **Image meaning:** descriptive alternatives provide context for relevant project imagery.

These are observed markup patterns, not proof of correct behavior in every state. The full HTML response contains multiple H1 elements, including template markup; visible heading order and hidden-template behavior still need an accessibility review. Screen-reader operation, focus order, contrast, error announcements and WCAG conformance have not been certified by this portfolio check.

## Details that connect the experience

The October 11 release also removed entrance-animation waiting from hero text, retained the original layout and SEO fields in a backup draft, and verified layouts at desktop and 390px phone width. Site components use named sections, responsive grids, descriptive links and reduced-motion rules in the reviewed custom markup. Quote links preserve page-of-origin context, while the guided intake offers both step-by-step and full-form presentation.

These decisions explain the care taken in the build. They are not a claim that every template, interaction, or device combination has passed a complete audit.
