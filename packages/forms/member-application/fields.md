# Membership Application — Field Definitions

Canonical field list for the membership application. Every intake surface derives from
this file and must not add fields of its own:

- the public web form on the website,
- the application issue template in `aoc-board`,
- § 3 of the membership admission rules (`aoc-governance`, `bylaws/member-admission.md`).

Submitted applications are stored board-only and never in this repository.

## Fields

Labels are given in German (primary) and English, because the website is bilingual.
`key` is the stable identifier used by consuming systems.

| key | Label (DE) | Label (EN) | Type | Required | Basis |
| --- | --- | --- | --- | --- | --- |
| `name` | Name | Name | text | yes | identifies the applicant |
| `email` | E-Mail | Email | email | yes | § 5 (3) decision is sent in text form |
| `membership_type` | Art der Mitgliedschaft | Type of membership | choice | yes | § 4 (1)–(3) statutes |
| `organisation_name` | Organisation | Organisation | text | if organisation | § 4 (2) statutes |
| `organisation_representative` | Benannte Person | Designated person | text | if organisation | § 4 (2) — exercises the membership rights |
| `organisation_category` | Größe / Art der Organisation | Organisation size / type | choice | if organisation | fee bracket per contribution schedule |
| `relation` | Fachlicher oder praktischer Bezug | Professional or practical connection | textarea | yes | § 4 (4) statutes — core admission criterion |
| `github_username` | GitHub-Benutzername | GitHub username | text | no | optional onboarding into the members team |
| `public_naming` | Veröffentlichung der Mitgliedschaft | Publication of membership | choice | yes | § 4 (7) statutes — consent, see below |
| `message` | Fragen oder Anmerkungen | Questions or remarks | textarea | no | lets an applicant ask instead of writing a separate mail |

### Choice values

`membership_type`

| value | DE | EN |
| --- | --- | --- |
| `ordinary_individual` | Ordentlich – Einzelmitgliedschaft | Ordinary – individual |
| `ordinary_organisation` | Ordentlich – Organisationsmitgliedschaft | Ordinary – organisation |
| `supporting` | Fördermitgliedschaft | Supporting membership |

`organisation_category` — mirrors the brackets of the contribution schedule

| value | DE | EN |
| --- | --- | --- |
| `small` | Bis 20 Mitarbeitende | Up to 20 employees |
| `large` | Über 20 Mitarbeitende | More than 20 employees |
| `nonprofit` | Forschung, öffentliche Körperschaft oder gemeinnützig | Research, public body or non-profit |

`public_naming`

| value | DE | EN |
| --- | --- | --- |
| `consented` | Einverstanden mit öffentlicher Nennung | Consents to public naming |
| `objected` | Widerspruch gegen öffentliche Nennung | Objects to public naming |

## Deliberately not collected at application time

| Not asked | Why |
| --- | --- |
| Postal address | Only needed to invoice dues, i.e. **after** admission. Collecting it up front would store the address of every rejected applicant for no purpose. |
| Exact headcount | The contribution schedule only distinguishes brackets, so the bracket is sufficient. |
| Date of birth, bank details | Not required for the admission decision. Payment data is handled separately and never in a repository. |

## Data protection

- **Legal basis.** Processing the application is based on Art. 6 (1) (b) GDPR (steps
  prior to, and performance of, the membership relationship). It is **not** based on
  consent, so no consent may be requested for it.
- **Consent applies to one field only.** `public_naming` implements § 4 (7) of the
  statutes and is a genuine consent: it must be given separately and can be withdrawn
  at any time in text form.
- **Information duty.** The form must link to the privacy notice and state the purpose,
  the controller and the retention period at the point of collection (Art. 13 GDPR).
- **Storage.** Applications are stored board-only. Personal data must not reach public
  repositories or member-readable views; public and member-facing lists are derived and
  limited to what § 4 (7) allows.
- **Retention.** Rejected applications are deleted once the decision is final; only the
  record needed to evidence the decision is kept. The board sets the concrete period.
- **Minimisation applies to the free-text fields too.** `relation` and `message` should
  not invite applicants to volunteer more personal detail than the criteria require.

## Change discipline

Changing this list means changing the web form, the issue template and § 3 of the
admission rules together. The rules take precedence: no intake surface may require an
entry that the statutes do not support.
