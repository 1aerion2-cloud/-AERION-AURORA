# ChartFox integration proposal

**AERION AURORA · 30 September 2026**

Status: proposal for review. Access approval and working integration are not claimed.

## Product and purpose

AERION AURORA is a flight simulation operations companion developed by Dereck Aubrey G. Rolle. It uses a locally running service and a browser dashboard to connect simulated dispatch, aircraft monitoring, turnaround awareness and flight review. Initial development focuses on Microsoft Flight Simulator and the ATR 72-600, with regional operations in the Bahamas and Caribbean.

The proposed ChartFox feature would help a user brief the departure, destination and alternate airports associated with a simulated flight. Chart availability and use would remain subject to ChartFox and publisher permissions.

## Requested experience

1. Import a SimBrief plan or select an airport manually.
2. Open Charts for that airport.
3. Complete the authorization required by ChartFox.
4. Browse available airport, ground, departure, arrival and approach charts.
5. Open a selected chart using an approved viewer or link.

Chart discovery and viewing would be initiated by the user. No bulk collection, chart mirror or chart redistribution is proposed. Missing coverage would be shown explicitly.

## Architecture to agree before implementation

The prototype dashboard runs at `http://127.0.0.1:8765`. This is a local application address, not the public product page and not a registered callback URI.

The public overview is https://github.com/1aerion2-cloud/-AERION-AURORA .

We request guidance on the supported authentication flow for a locally installed application, permitted callback arrangement, scopes, chart display method, request limits, caching and attribution. No endpoint names, scopes or redirect path are assumed in this proposal. Any secret that must remain confidential must not be shipped inside a distributed application.

## Questions for review

- Is this application eligible, and may its public GitHub overview serve as its product URL?
- Which authorization flow and redirect URI format should it use?
- Which permissions cover airport chart discovery and viewing?
- Is an embedded viewer permitted, or should the application open ChartFox externally?
- What publisher, attribution, retention, caching and request-limit conditions apply?
- Are test access and later public or commercial distribution subject to separate approval?

Commercial terms and future distribution arrangements are not asserted here and must be confirmed by the project owner when applying.

## Boundaries

This feature is for flight simulation only. It is not intended for real-world navigation or operational dispatch. A structured navigation database, radio frequencies, navaids and runway wind calculations are separate features; this proposal does not assume ChartFox provides these through its API.

ChartFox, chart publishers and other third parties retain their respective rights. AERION does not claim partnership or endorsement.

Project owner: Dereck Aubrey G. Rolle. Public project questions: https://github.com/1aerion2-cloud/-AERION-AURORA/issues . Private application contact details will be supplied through the application channel.
