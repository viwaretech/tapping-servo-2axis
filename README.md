# 🔧 Tapping Auto 2 Axis

![License](https://img.shields.io/badge/License-Commercial-red)
![PLC](https://img.shields.io/badge/PLC-Mitsubishi-blue)
![HMI](https://img.shields.io/badge/HMI-Samkoon-green)
![Automation](https://img.shields.io/badge/Grade-Industrial--Automation-orange)

⚙️ Automation project for a **2-Axis Automatic Tapping Machine** using **Mitsubishi PLC** and **Samkoon HMI**.

This system automates tapping operations with two motion axes:

- **X Axis** → positioning to tapping location  
- **Z Axis** → tapping motion (down / up)

Designed for **industrial automation**, **machine retrofit**, and **production tapping stations**.

---

# 🏗 System Architecture

The control system follows a standard **industrial automation hierarchy**.

```
👤 Operator
   │
   ▼
🖥 HMI (Samkoon)
   │
   ▼
🧠 PLC (Mitsubishi)
   │
   ▼
⚙ Actuators
   ├─ X Axis Motor
   ├─ Z Axis Motor
   └─ Tapping Spindle
```

---

# 🔄 Machine Flow Chart

```mermaid
flowchart TD

A[🔌 Power ON] --> B[🧠 PLC Initialization]

B --> C[🏠 Homing Axis]

C --> D[👤 Wait Operator Start]

D --> E[➡ Move X Axis]

E --> F[⬇ Lower Z Axis]

F --> G[🔩 Tapping Process]

G --> H[↩ Reverse Tap]

H --> I[⬆ Raise Z Axis]

I --> J{Next Position?}

J -- Yes --> E
J -- No --> K[✅ Cycle Complete]

K --> D
```

---

# ✨ Features

✔ Mitsubishi PLC based control  
✔ Samkoon HMI operator interface  
✔ Automatic tapping cycle  
✔ Dual axis motion control  
✔ Homing system  
✔ Emergency stop support  
✔ Expandable tapping positions  
✔ Industrial automation ready

---

# 🧰 Hardware Configuration

Typical machine setup:

| Component | Description |
|--------|--------|
| 🧠 PLC | Mitsubishi PLC |
| 🖥 HMI | Samkoon Touch HMI |
| ⚙ X Axis Motor | Stepper / Servo |
| ⚙ Z Axis Motor | Stepper / Servo |
| 🔌 Motor Driver | Stepper / Servo driver |
| 🛑 Limit Switch | Homing & safety |
| 🔋 Power Supply | 24V industrial power |

---

# ▶ Machine Operation

Typical operation sequence:

1️⃣ 🔌 Power ON machine  
2️⃣ 🧠 PLC initializes system  
3️⃣ 🏠 Axis homing process  
4️⃣ 👤 Operator presses **START** on HMI  
5️⃣ ➡ X axis moves to tapping position  
6️⃣ ⬇ Z axis lowers tapping tool  
7️⃣ 🔩 Tapping process begins  
8️⃣ ↩ Tap reverses  
9️⃣ ⬆ Z axis returns up  
🔟 🔁 Repeat for next position or finish

---

# 🔮 Future Development

Possible future improvements:

- 🔩 Multi-hole tapping pattern
- 🤖 Automatic workpiece clamping
- 📊 Production counter
- ⚡ Torque monitoring
- 🚨 Alarm diagnostics
- 🏭 Conveyor system integration

---

# 🚀 Download

- **Tapping Auto 2 Axis Project(Latest)**  
   ![Release](https://img.shields.io/github/v/release/viwaretech/tapping-servo-2axis?display_name=release&label=Release&style=flat) ![Version](https://img.shields.io/github/v/release/viwaretech/tapping-servo-2axis?display_name=tag&label=Version&style=flat&color=4CAF50) ![Build](https://img.shields.io/badge/Build%20date-20260309-E7352C)<br>
  ➡️ [Release Page](https://github.com/viwaretech/tapping-servo-2axis/releases/latest)  
   ➡️ [Download Project](https://github.com/viwaretech/tapping-servo-2axis/releases/latest/download/tapping-servo-2axis.zip)

---


# 📜 License

This project is distributed under a **Commercial License**.

Use of this software requires **purchasing a license from the author**.

📄 Full license terms:

➡ **[LICENSE](LICENSE)**

---

# 👨‍💻 Author
**HARLEY AD**  
Industrial automation project for **2-axis tapping machine development** using **Mitsubishi PLC** and **Samkoon HMI**.

⚙️ Focus:  
Industrial Automation • PLC Programming • Machine Control Systems
