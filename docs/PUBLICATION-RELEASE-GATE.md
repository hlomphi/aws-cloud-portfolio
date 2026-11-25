# Portfolio publication release gate

**Status: BLOCKED — internal review only.** This checklist is a release control, not evidence of publication clearance. Do not merge the draft pull request or publish its diagrams to LinkedIn until every item is supported by review evidence.

## Confidentiality and intellectual property

- [ ] Inspect all seven current SVGs and editable diagram sources for client names, emblems, logos, domains, email addresses, account IDs, ARNs, endpoints, network identifiers and identifying operational detail.
- [ ] Visually inspect original and retained PNGs, including earlier branches and historical commits. Removing a file in the proposed pull request does **not** remove it from Git history.
- [ ] Compare each replacement diagram with its source architecture. Document intentional redactions and confirm that service relationships and implementation status remain accurate.
- [ ] Establish that the publisher has rights to disclose each case study and diagram, including any employer/client-owned material. Removal of branding alone does not establish IP rights.
- [ ] If historical sensitive content is discovered, contain exposure and seek **separate explicit approval** before any destructive history rewrite.

## Architecture and documentation quality

- [ ] Replace generic Graphviz service boxes with appropriately licensed official AWS Architecture Icons, retaining editable source or a reproducible build path.
- [ ] Validate AWS service naming, boundaries, authentication and data flows, encryption, logging, archival lifecycle and the distinction between deployed and proposed components.
- [ ] Render all seven diagrams and check legibility, clipped labels, mobile viewing and accessibility text.
- [ ] Validate internal Markdown links, image links and external links on the published rendering.
- [ ] Check all outcome metrics and certification claims against evidence; label unverified figures accordingly.

## Release and distribution

- [ ] Record reviewer evidence and clear every release gate before changing PR #3 from draft.
- [ ] Merge only after confidentiality, architecture, technical quality and IP publication conditions are verified.
- [ ] Verify the merged default branch and rendered portfolio.
- [ ] Verify LinkedIn integration and any manually uploaded media attachments before declaring completion.

**Owner instruction:** Conditional approval is granted for anonymised publication with client names and emblems removed. It does not authorise destructive history changes, nor does it replace third-party publication rights.

## Review evidence — 2026-11-23

- **Confirmed:** Seven case-study Markdown files and seven editable Graphviz architecture sources exist on the draft branch. Case studies distinguish implementation, proposal and proof-of-concept status. These checks do not prove original-diagram fidelity.
- **Corrected in branch:** README no longer asserts the unverified AI Practitioner credential; the media archive description explicitly distinguishes direct browser-to-S3 multipart transfers from Lambda coordination and identifies S3 Lifecycle as the archival mechanism; the generative AI case study clarifies OIDC role assumption and unspecified ingress.
- **Still unverified:** visual inspection of original PNGs and all historical revisions; confidential information in historical Git objects; employer/client publication rights; official AWS Architecture Icon usage; rendered SVG visual review and link checks; LinkedIn media publication.
- **Decision:** Keep PR #3 draft and unmerged. GitHub's mergeability flag is a technical conflict check, not a confidentiality or publication-rights clearance.
