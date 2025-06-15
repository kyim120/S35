
### 🔌 Relay Circuit Diagram (ASCII with Color Labels & Arrows)

```plaintext
                         🧠 RELAY CONTROL CIRCUIT

                   +----------+    +----------+    +----------+    +----------+
                   |  S1 🔴    |    |  S2 🔴    |    |  S3 🔴    |    |  S4 🔴    |
                   +----+-----+    +----+-----+    +----+-----+    +----+-----+
                        |               |               |               |
                        |               |               |               |
                    [W1 🔴]         [W5 🔴]         [W9 🔴]         [W13 🔴]
                        ↓               ↓               ↓               ↓
                   +----+----+     +----+----+     +----+----+     +----+----+
                   |  R1 🔻   |     |  R2 🔻   |     |  R3 🔻   |     |  R4 🔻   |
                   +----+----+     +----+----+     +----+----+     +----+----+
                        |               |               |               |
                    [W2 🔵]         [W6 🔵]         [W10 🔵]        [W14 🔵]
                        ↓               ↓               ↓               ↓
                   +----+----+     +----+----+     +----+----+     +----+----+
                   |  K1 ⚙️    |     |  K2 ⚙️    |     |  K3 ⚙️    |     |  K4 ⚙️    |
                   +----+----+     +----+----+     +----+----+     +----+----+
                        |               |               |               |
                    [W3 🟡]         [W7 🟡]         [W11 🟡]        [W15 🟡]
                        ↓               ↓               ↓               ↓
                        +---------------+---------------+---------------+
                                        ↓
                                    [W16 🟢]
                                        ↓
                                 +------+------+
                                 |   Ammeter ⚡  |
                                 +------+------+
                                        ↓
                                    [W17 ⚫]
                                        ↓
                                     [Ground]
```

---

### 📶 Wire Connections

| Wire ID | Color Emoji | From → To             | Purpose                       |
| ------- | ----------- | --------------------- | ----------------------------- |
| `W1`    | 🔴          | S1 → R1               | Power from switch to resistor |
| `W2`    | 🔵          | R1 → K1               | Signal from resistor to relay |
| `W3`    | 🟡          | K1 → Ammeter          | Current to Ammeter            |
| `W5`    | 🔴          | S2 → R2               | Branch 2 input                |
| `W6`    | 🔵          | R2 → K2               | Signal line                   |
| `W7`    | 🟡          | K2 → Ammeter          | Output to Ammeter             |
| `W9`    | 🔴          | S3 → R3               | Branch 3 input                |
| `W10`   | 🔵          | R3 → K3               | Signal line                   |
| `W11`   | 🟡          | K3 → Ammeter          | Output to Ammeter             |
| `W13`   | 🔴          | S4 → R4               | Branch 4 input                |
| `W14`   | 🔵          | R4 → K4               | Signal line                   |
| `W15`   | 🟡          | K4 → Ammeter          | Output to Ammeter             |
| `W16`   | 🟢          | Merge Point → Ammeter | Combined current path         |
| `W17`   | ⚫           | Ammeter → Ground      | Ground/return line            |

---
