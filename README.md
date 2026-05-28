# Castalia WorldSchool Travel

Public shell and operating contract for worldschool travel organization.

This repository owns the travel organizer surface for:

- transportation planning
- housing and base selection
- visa, border, and document checklists
- packing, transit, and recovery rhythms
- budget and booking status
- family and pupil itinerary handoffs

The public site lives at:

```text
travel.worldschool.castalia.institute
```

## Data Boundary

Do not commit live booking records, passport data, addresses, private family
calendars, emergency contacts, confirmation numbers, or payment details here.

Family-specific operational data should live in the relevant private family
repository, for example:

```text
CastaliaInstitute/castalia-family-mcshan
```

This repo may contain public-safe schemas, templates, agent instructions, and
non-sensitive examples.

## Agent

The travel agent contract lives in:

```text
agents/worldschool-travel-agent.md
```

The intended agent reads a family Gazette destination spine, turns each stop into
practical travel tasks, and writes structured travel plans back to the private
family repo.

## Schemas

`schemas/travel-plan.schema.json` defines the current draft shape for a private
family travel plan. It is intentionally logistics-oriented rather than
curriculum-oriented; the Gazette and pupil repos handle learning plans.

## Destination Catalog

`data/worldschool-destinations.yml` is a broad candidate catalog for future
worldschool planning. It groups destinations by region and tags each place with
learning threads such as ecology, public memory, geology, language, design,
astronomy, food systems, and infrastructure.

The catalog is not a live safety or booking source. Before using any destination
for a real family plan, check current advisories, entry requirements, seasonal
conditions, health guidance, accessibility, and family-specific constraints.

## Deployment

This repo deploys by GitHub Actions to GitHub Pages. Configure the Pages custom
domain as:

```text
travel.worldschool.castalia.institute
```

DNS:

```text
travel.worldschool.castalia.institute CNAME castaliainstitute.github.io
```
