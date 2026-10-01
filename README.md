# AERION AURORA
### Flight Simulation Operations Intelligence
**Operate Like an Airline.**

AERION AURORA is an independently developed flight simulation companion that brings dispatch preparation, live aircraft monitoring, turnaround awareness, and flight review into one operations workspace.

The project focuses on regional airline simulation, beginning with Microsoft Flight Simulator and the ATR 72-600, with a particular interest in operations across the Bahamas and wider Caribbean.

**Development status:** Active prototype and iterative simulator flight testing.  
**ChartFox status:** Proposed integration; access and implementation are subject to ChartFox review and approval.  
**Intended use:** Flight simulation only. Not for real-world navigation, dispatch, or aircraft operation.

---

## The product

AERION is designed to connect the planning and operational stages of a simulated flight. A local service communicates with the simulator, while the user works through a browser-based dashboard on their own computer.

The development workflow covers:

| Area | Purpose |
| --- | --- |
| Dispatch | Bring flight-plan context and operational preparation into one workspace, including SimBrief import. |
| Live flight monitoring | Display simulator telemetry and track progress through ground and airborne flight phases. |
| Aircraft systems and digital twin | Present aircraft state visually, including doors, lighting, electrical power, and propeller-related indications where supported. |
| Turnaround awareness | Follow boarding and ground-service progress, with GSX and FS2Crew awareness under development and testing. |
| Map and streaming overlay | Show flight progress and provide an OBS-oriented view. |
| Flight review | Use recorded events and telemetry to identify issues and refine the next test build. |

Feature availability and reliability vary by development build, aircraft, and connected add-ons. This repository is the public product overview; it does not currently distribute the simulator application.

## Why ChartFox fits

Chart access would help users move from a flight plan to the relevant airport and procedure briefing within the same workflow.

The proposed integration would let a user select the departure, destination, or alternate airport and access available charts through a ChartFox-approved method.

Requested chart categories, where available, include:

- Airport and ground-movement charts.
- Standard Instrument Departures (SIDs).
- Standard Terminal Arrival Routes (STARs).
- Instrument approach charts, including ILS and RNAV procedures.
- Other relevant airport briefing material made available through the service.

Coverage would depend on the airport, publisher, and ChartFox availability. AERION would clearly indicate unavailable charts and would not promise complete Bahamas, Caribbean, or worldwide coverage.

## Proposed user workflow

1. Import a SimBrief flight plan or select an airport in AERION.
2. Open the airport's Charts section.
3. Complete any authentication required by ChartFox using its approved authorization flow.
4. Browse the available chart categories.
5. Open the selected chart using the viewing or linking method authorized by ChartFox.

This is the intended workflow, not a claim that ChartFox functionality is already implemented.

## Integration approach for review

AERION seeks guidance and permission for a limited, user-driven integration:

- Use documented, authorized interfaces and request only the access needed for chart discovery and viewing.
- Preserve required ChartFox and chart-publisher attribution.
- Follow applicable limits on requests, caching, display, and redistribution.
- Keep chart requests tied to user actions; avoid bulk collection or mirroring.
- Keep credentials and tokens out of public repositories, browser URLs, shared logs, and OBS overlays.
- Provide clear disconnected, unavailable, and authorization-expired states.

AERION's current development dashboard runs locally at `http://127.0.0.1:8765`. This is a local application address, **not a public product URL or a registered OAuth callback**.

The authentication model, permitted redirect URI, token storage, required scopes, and viewing method must be agreed before implementation. Any client secret required to remain confidential must not be embedded in a distributed desktop application.

## Questions for the ChartFox team

1. Is this local-service and browser-dashboard application eligible for integration access?
2. Which authentication flow and redirect arrangement should a locally installed application use?
3. What permissions are available for airport chart discovery and viewing?
4. Is in-application viewing permitted, or should charts open in ChartFox?
5. What attribution, caching, request-limit, and publisher restrictions apply?
6. Are there additional review requirements before a broader release?

A runway wind calculator, radio frequencies, navaids, and a structured navigation database are separate development topics. This proposal does not assume ChartFox supplies those data or grants permission to extract them from charts.

## Project ownership and contact

**Project creator:** Dereck Aubrey G. Rolle  
**GitHub account:** [1aerion2-cloud](https://github.com/1aerion2-cloud)  
**Project questions:** [Open a repository issue](https://github.com/1aerion2-cloud/-AERION-AURORA/issues)

Please keep credentials, access tokens, and private account information out of public issues.

AERION AURORA is an independent project. References to ChartFox, Microsoft Flight Simulator, SimBrief, GSX, FS2Crew, and other third-party products describe intended or development workflows and do not imply partnership, endorsement, or integration approval.

---

**Product overview and integration proposal · Updated 30 September 2026**


## Further information

- [ChartFox integration proposal](docs/CHARTFOX_INTEGRATION.md)
- [Development status and roadmap](docs/STATUS_AND_ROADMAP.md)
- [Proposed data handling](docs/DATA_HANDLING.md)



## Flight Tests & Demonstrations

The following streams document flight-simulation testing during AERION AURORA’s development:

- [Flight-test stream 1](https://www.youtube.com/watch?v=Y26e11WAUqU)
- [Flight-test stream 2](https://www.youtube.com/watch?v=S85aNV5ZgLw)

These recordings show development builds. Features, appearance and reliability may change as testing continues. They do not represent a finished release or an approved ChartFox integration.
