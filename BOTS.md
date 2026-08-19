# Bots of Business Development  (docx S5 candidate menu)

These are the **Major sub-functions** of Business Development from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 7.

- `partner-strategy` — **Partner Strategy**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `partner-sourcing` — **Partner Sourcing**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `strategic-alliances` — **Strategic Alliances**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `channel-partnerships` — **Channel Partnerships**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `ecosystem-development` — **Ecosystem Development**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `partnership-operations` — **Partnership Operations**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
- `relationship-management` — **Relationship Management**  ·  titles: VP Business Development, VP Strategic Partnerships, BD Director, Partnerships Director, BD Manager, Strategic Alliances Manager
