# Australia Post (australia-post)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Australia Post is Australia's primary postal operator, offering a developer platform with REST APIs for e-commerce merchants, logistics providers, and delivery partners. APIs cover shipping label creation, parcel tracking, postage calculation, parcel locker and post office location lookup, delivery choice and scheduling, and delivery partner event reporting for an integrated end-to-end fulfilment ecosystem.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Address Validation
- Click and Collect
- Delivery
- E-Commerce
- Labels
- Locations
- Logistics
- Parcel Locker
- Postal
- Postage
- Shipping
- Tracking

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### Australia Post Shipping and Tracking API

Enables eParcel and StarTrack contract customers to lodge orders, create and print shipping labels (including dangerous goods forms), generate order summaries, despatch parcels, estimate prices and international landed costs, and track parcel progress from source to destination through a single REST integration. Requires an active Australia Post or StarTrack billing account number; a sandbox test-bed environment is provided before going live.

- **Human URL:** [https://auspost.com.au/integrate-shipping-and-tracking-apis](https://auspost.com.au/integrate-shipping-and-tracking-apis)
- **Base URL:** `https://digitalapi.auspost.com.au`

#### Tags

- Shipping
- Labels
- Tracking
- Logistics
- E-Commerce

#### Properties

- [Documentation](https://auspost.com.au/integrate-shipping-and-tracking-apis)
- [Getting Started](https://auspost.com.au/developers/help-support/how-to-get-credentials/)
- [API Reference](https://developers.auspost.com.au/apis/shipping-and-tracking/reference)

### Australia Post Postage Assessment Calculator API

Lets businesses and developers embed a postage calculator into websites or applications to retrieve standard retail postage rates for domestic and international parcels and letters. Accepts weight, dimensions, origin, and destination to return eligible services with pricing. Uses HTTP GET requests returning JSON or XML; authentication via AUTH-KEY header. Free API key available via self-serve registration. Note — this API returns retail rates only; contract rates require the Shipping and Tracking API.

- **Human URL:** [https://developers.auspost.com.au/apis/pac/](https://developers.auspost.com.au/apis/pac/)
- **Base URL:** `https://digitalapi.auspost.com.au`

#### Tags

- Postage
- Pricing
- E-Commerce
- Rating

#### Properties

- [Documentation](https://developers.auspost.com.au/apis/pac/)
- [API Reference](https://developers.auspost.com.au/apis/pac/reference)
- [Getting Started](https://developers.auspost.com.au/apis/pacpcs-registration)
- [A P I Explorer](https://developers.auspost.com.au/apis/pac/explorer)

### Australia Post Locations API

Returns Australia Post outlet and facility information based on postcode or GPS coordinates, enabling applications to surface nearby post offices, parcel lockers, and parcel collect points to customers at checkout or on a store-finder map. Current version is 2.3.0. Available at no cost; API key obtained via the Developer Portal.

- **Human URL:** [https://auspost.com.au/developers/openapi/partner/locations/overview/](https://auspost.com.au/developers/openapi/partner/locations/overview/)
- **Base URL:** `https://digitalapi.auspost.com.au/locations/v2`

#### Tags

- Locations
- Post Office
- Parcel Locker
- Click and Collect

#### Properties

- [Documentation](https://auspost.com.au/developers/openapi/partner/locations/overview/)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/locations-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Australia Post Delivery Choices API

Allows customers to select preferred delivery options at checkout, including delivery speed, delivery or collection location, and specific day, date, and time of delivery. Supports parcel locker delivery, authority to leave, nominated safe place, and click-and-collect at Australia Post outlets. Access requires meeting eParcel contract minimum volumes.

- **Human URL:** [https://developers.auspost.com.au/apis/dce/](https://developers.auspost.com.au/apis/dce/)
- **Base URL:** `https://digitalapi.auspost.com.au`

#### Tags

- Delivery
- Click and Collect
- Parcel Locker
- E-Commerce
- Checkout

#### Properties

- [Documentation](https://developers.auspost.com.au/apis/dce/)

### Australia Post Delivery Partner API

Enables authorised Australia Post delivery network partners to report delivery events back to Australia Post systems in near real-time. Partners push scan events and delivery outcomes via POST requests to a single endpoint; the data feeds Australia Post's consumer tracking and operational reporting. Current version is 1.3.0; OpenAPI definition available for client code generation.

- **Human URL:** [https://auspost.com.au/developers/openapi/partner/delivery-partner/1.3.0/overview/](https://auspost.com.au/developers/openapi/partner/delivery-partner/1.3.0/overview/)
- **Base URL:** `https://digitalapi.auspost.com.au/delivery-partner`

#### Tags

- Delivery
- Logistics
- Tracking
- Partners

#### Properties

- [Documentation](https://auspost.com.au/developers/openapi/partner/delivery-partner/1.3.0/overview/)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/australia-post/refs/heads/main/openapi/delivery-partner-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Website](https://auspost.com.au/)
- [Developer Portal](https://auspost.com.au/developers/)
- [Developer Portal](https://developers.auspost.com.au/)
- [Documentation](https://auspost.com.au/developers/help-support/about-our-apis/)
- [Getting Started](https://auspost.com.au/developers/help-support/how-to-get-credentials/)
- [Catalog](https://auspost.com.au/developers/api-documentations/)
- [Sign Up](https://developers.auspost.com.au/apis/pacpcs-registration)
- [Login](https://developers.auspost.com.au/)
- [Status Page](https://status.developers.auspost.com.au/)
- [Terms of Service](https://auspost.com.au/developers/help-support/)
- [Contact](mailto:customer_connectivity@auspost.com.au)
- [Integrate Page](https://auspost.com.au/integrate-shipping-and-tracking-apis)
- [LinkedIn](https://www.linkedin.com/company/australia-post)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
