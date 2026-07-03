# Solv Health (solv-health)

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
