# Solv Health (solv-health)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Solv Health operates a consumer marketplace (solvhealth.com and the Solv app) for booking same-day urgent care, primary care, and lab appointments, plus a provider-facing platform (scheduling, intake, patient acquisition, reputation management, messaging, payments) sold to clinics and health systems. There is no self-serve public developer API or published API reference on solvhealth.com; API access is gated behind a sales-led partnership. Solv states it exposes "interoperable APIs" that power custom booking experiences on partner websites and apps, a "Final Mile" API/network that lets digital-first and virtual-care partners (e.g. Included Health) hand patients off to real-time same-day appointment availability at Solv's national network of urgent care clinics, and bidirectional EHR interoperability (APIs, HL7, FHIR, and RPA) that syncs patient demographics, appointment status, and documents with systems like Epic, Athena, Cerner, Allscripts, DrChrono, eClinicalWorks, Experity, and NextGen. None of these capabilities have a published base URL, endpoint reference, or self-serve API key signup; access is provisioned per partner/clinic inside a commercial contract.

**Access model:** Gated / partner-provisioned. No public developer portal, no `api.solvhealth.com` or `docs.solvhealth.com`, no self-serve API keys. See [review.yml](review.yml) for the full findings.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/solv-health/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/solv-health/refs/heads/main/apis.yml)

## Tags

- Healthcare
- Urgent Care
- Appointment Booking
- EHR Interoperability
- HL7
- FHIR
- Digital Health

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Solv Final Mile API

Real-time same-day appointment availability and booking capability that lets digital-first and virtual-care partners (telehealth navigators, health plans) hand a patient off to an in-person visit at a clinic in Solv's national urgent care network. Announced publicly via the "Solv Final Mile Network" (partners include Included Health); described in marketing only as "proprietary APIs and tools" with no published base URL, endpoint list, or request/response schema.

*This API is modeled from publicly available marketing language only (`endpointsModeled: true`); no endpoint paths, base URL, or request/response schema are published by Solv.*

- **Human URL:** [https://www.solvhealth.com/for-providers/build](https://www.solvhealth.com/for-providers/build)

#### Tags

- Availability
- Booking
- Virtual Care Handoff
- Final Mile

#### Properties

- [Documentation](https://www.solvhealth.com/for-providers/build)
- [Documentation](https://www.prnewswire.com/news-releases/solv-launches-final-mile-network-enabling-handoff-between-virtual-care-navigators-and-local-in-person-providers-to-complete-a-critical-path-in-the-care-continuum-301743169.html)

### Solv Booking Widget API

Interoperable API that powers a custom, white-labeled digital patient-booking experience embedded on a health system or clinic's own website and mobile app - surfacing real-time local urgent care and lab availability under the partner's own brand. Solv markets this as "plug-and-play APIs and dedicated developers," but publishes no public API reference, base URL, or self-serve credential flow; delivery is hands-on with Solv's own developers as part of a paid engagement.

*This API is modeled from publicly available marketing language only (`endpointsModeled: true`); no endpoint paths, base URL, or request/response schema are published by Solv.*

- **Human URL:** [https://www.solvhealth.com/for-providers/health-systems](https://www.solvhealth.com/for-providers/health-systems)

#### Tags

- Widget
- Scheduling
- Website Embed
- Patient Experience

#### Properties

- [Documentation](https://www.solvhealth.com/for-providers/health-systems)
- [Documentation](https://www.solvhealth.com/for-providers/integrations)

### Solv EHR Interoperability API

Bidirectional interoperability layer that automatically syncs patient demographics, appointment details, and media (insurance cards, ID, consent forms) into a clinic's electronic health record, and syncs patient status back out in real time to support wait-time and throughput metrics. Solv states it connects "through standard healthcare interfaces, including APIs, HL7, FHIR, and robotic process automation (RPA)" to EHR/EMR systems such as Epic, Athena, Cerner, Allscripts, DrChrono, eClinicalWorks, Experity, NextGen, and Advanced. No public API reference, base URL, or self-serve credentials are published; each connection is configured by Solv's implementation team per EHR vendor and per customer.

*This API is modeled from publicly available marketing language only (`endpointsModeled: true`); no endpoint paths, base URL, or request/response schema are published by Solv.*

- **Human URL:** [https://www.solvhealth.com/for-providers/integrations](https://www.solvhealth.com/for-providers/integrations)

#### Tags

- EHR
- EMR
- HL7
- FHIR
- Sync

#### Properties

- [Documentation](https://www.solvhealth.com/for-providers/integrations)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/solvhealth)
- [Website](https://www.solvhealth.com/)
- [Documentation](https://www.solvhealth.com/for-providers/integrations)
- [Plans](plans/solv-health-plans-pricing.yml)
- [Fin Ops](finops/solv-health-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
