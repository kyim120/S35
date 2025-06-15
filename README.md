# *more visually attractive ASCII circuit diagram*

---

### ✅ Copy-Paste Ready `.md` Content:

````markdown
# 🔌 Relay Circuit Diagram (Enhanced ASCII View)

A neatly structured ASCII diagram showing a 4-switch, 4-relay circuit connected to an ammeter. Each connection is marked with wire names and purpose.

```plaintext
                        RELAY CONTROL CIRCUIT

                    +----------+    +----------+    +----------+    +----------+
                    |  Switch  |    |  Switch  |    |  Switch  |    |  Switch  |
                    |   S1     |    |   S2     |    |   S3     |    |   S4     |
                    +----+-----+    +----+-----+    +----+-----+    +----+-----+
                         |               |               |               |
                     [W1:Red]        [W5:Red]        [W9:Red]        [W13:Red]
                         |               |               |               |
                    +----v----+     +----v----+     +----v----+     +----v----+
                    | Resistor|     | Resistor|     | Resistor|     | Resistor|
                    |   R1    |     |   R2    |     |   R3    |     |   R4    |
                    +----+----+     +----+----+     +----+----+     +----+----+
                         |               |               |               |
                    [W2:Blue]       [W6:Blue]       [W10:Blue]      [W14:Blue]
                         |               |               |               |
                    +----v----+     +----v----+     +----v----+     +----v----+
                    |  Relay  |     |  Relay  |     |  Relay  |     |  Relay  |
                    |   K1    |     |   K2    |     |   K3    |     |   K4    |
                    +----+----+     +----+----+     +----+----+     +----+----+
                         |               |               |               |
                    [W3:Yellow]    [W7:Yellow]     [W11:Yellow]    [W15:Yellow]
                         |               |               |               |
                         +---------------+---------------+---------------+
                                                         |
                                                     [W16:Green]
                                                         |
                                                   +-----v-----+
                                                   |  Ammeter  |
                                                   +-----+-----+
                                                         |
                                                     [W17:Black]
                                                         |
                                                      [Ground]
````

---

## 🎛 Components

* **Switches (S1–S4):** Toggle switches used to activate each relay circuit.
* **Resistors (R1–R4):** Limit current to protect relays.
* **Relays (K1–K4):** Electromagnetic switches (K1–K3 = 6V, K4 = 3V).
* **Ammeter (A):** Measures total current from active branches.

---

## 🔌 Wire Line Labels

| Wire ID | Color  | From        → To      | Purpose                          |
| ------- | ------ | --------------------- | -------------------------------- |
| `W1`    | Red    | S1         → R1       | Power from switch to resistor    |
| `W2`    | Blue   | R1         → K1       | Signal from resistor to relay    |
| `W3`    | Yellow | K1         → Ammeter  | Current path to Ammeter          |
| `W5`    | Red    | S2         → R2       | Second branch switch to resistor |
| `W6`    | Blue   | R2         → K2       | R2 to relay                      |
| `W7`    | Yellow | K2         → Ammeter  | K2 to Ammeter                    |
| `W9`    | Red    | S3         → R3       | Third branch switch              |
| `W10`   | Blue   | R3         → K3       | R3 to K3                         |
| `W11`   | Yellow | K3         → Ammeter  | K3 to Ammeter                    |
| `W13`   | Red    | S4         → R4       | Fourth branch                    |
| `W14`   | Blue   | R4         → K4       | R4 to K4                         |
| `W15`   | Yellow | K4         → Ammeter  | K4 to Ammeter                    |
| `W16`   | Green  | Junction    → Ammeter | Combined signal to Ammeter       |
| `W17`   | Black  | Ammeter     → Ground  | Ground return path               |

---

## ⚙ How It Works

1. Toggle any **switch** (S1 to S4).
2. Current flows through its **resistor** (R1–R4).
3. Energizes the corresponding **relay** (K1–K4).
4. The relay closes, sending current via a **yellow wire** to the **ammeter**.
5. **Ammeter** measures total current depending on how many relays are active.
6. Current returns to ground completing the loop.

---
