# Design Decisions

## Decision 001
### PCB Topographic Cover

#### Idea
Create the cover using PCB traces and copper layers to represent the terrain of Japan.
The cover itself becomes an artwork instead of a plain enclosure.

#### Why It Was Considered
- Unique appearance
- Integrates electronics into industrial design
- Creates a strong first impression

#### Why It Was Rejected
Although visually interesting, the terrain itself does not improve the user’s experience.

The complexity and manufacturing cost outweigh the practical value.

### Decision

Rejected

The project should focus on preserving memories rather than decorative electronics.

---

## Decision 002
### LED Shrine Map

#### Idea
Embed LEDs beneath the fabric cover.

Every visited shrine lights up its corresponding location on the map of Japan.

#### Why It Was Considered
- Beautiful ambient lighting
- Creates an emotional “memory map”
- Light diffusing through fabric would produce a subtle glow

#### Challenges
- Precise LED alignment
- Light guide design
- PCB complexity

### Decision

Deferred

A beautiful concept, but hardware complexity is too high for the first generation.

---

## Decision 003
### E-paper Display

#### Idea
Replace LED visualization with an E-paper display.

#### Why It Was Chosen
- Extremely low power consumption
- Power is only required during screen refresh
- Able to display Goshuin artwork, text, maps and memories
- Better suited to the philosophy of a digital Goshuin book

### Decision

Acceopted
The E-paper display becomes the core user interface.

---
## Decision 004
### NFC Energy Harvesting

#### Idea
Power the entire device using NFC energy harvesting.

A battery-less Goshuin book would greatly simplify maintenance.

#### Why It Was Considered

Combined with E-paper, the system only requires energy while updating the display.

If harvested power can be stabilized, a battery may become unnecessary.
#### Prototype Result

Experiments revealed significant differences between Android and iPhone.
Android

- Continuous NFC field
- Stable harvested voltage
- Suitable for energy harvesting experiments

iPhone

- Pulsed NFC field
- Intermittent harvested voltage
- Difficult to maintain stable power

#### Engineering Challenges

- Voltage regulation
- Super capacitor sizing
- Startup current
- Brown-out protection

### Decision

Partially Accepted

Energy harvesting remains useful for reducing battery consumption, but current smartphone behavior makes a fully battery-less design impractical.

---