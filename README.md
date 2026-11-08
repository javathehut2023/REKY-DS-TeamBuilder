# 🏜️ Desert Storm Battle Planner (Last War: Survival)

A lightweight browser tool for alliance leadership to automate team allocations and quadrant zone deployments for Desert Storm matches.

---

## ⚡ Features

- **Automated CSV & Google Sheet Import**: Pulls player names, power, main squad type, and team assignments directly from your roster spreadsheet.
- **Smart 5-Zone Tactical Balancing**:
  - **Zone E (Center Silo)**: Top 4 highest-power players auto-assigned as Elite Roamers.
  - **Outer Zones (A, B, C, D)**: Remaining lane units balanced across quadrants using a snake-draft algorithm.
  - **Type Counter-Balancing**: Prevents single-type clustering and enforces balanced troop splits per lane.
  - **Priority Zone Allocation**: Squads are mapped to zones by strategic building priority (Zone C Science Hub $\rightarrow$ Zone D Merc Factory $\rightarrow$ Zone B Arsenal $\rightarrow$ Zone A Info Center).
- **Dual Team Management**: Generates synchronized battle plans for both **Team A** and **Team B** simultaneously.
- **One-Click Alliance Copy**: Instantly copies a clean, pre-formatted deployment announcement ready to paste directly into Alliance Chat, Mails, or Discord.
- **100% Client-Side Privacy**: All parsing runs locally in your browser — no roster or player data is ever sent to or stored on an external server.

---

## 📋 Spreadsheet Setup

Your roster CSV or Google Sheet should have the following column structure:

| Column | Header Example | Format / Notes |
| :--- | :--- | :--- |
| **Column 1** | `Name` | Player In-Game Name |
| **Column 2** | `T1 Power` / `CP` | Squad Power (e.g. `34.5` or `34.5M`) |
| **Column 3** | `TYPE` | `Tank`, `Air` / `Aircraft`, or `Missile` |
| **Column 4** | `Team` | `A`, `B`, `1`, `2`, or `Sub` (Optional) |

> **Google Sheets Link**: To use a live sheet link, go to `File` → `Share` → `Publish to web` → Choose `Entire Document` (or specific sheet) as **Comma-separated values (.csv)** and paste the link into the tool.

---

## 🚀 How to Use

1. Open `index.html` in any web browser (or visit your live GitHub Pages link).
2. Paste your Google Sheets CSV URL or click **Choose File** to select your `.csv`.
3. Adjust player team assignments (`Team A`, `Team B`, or `Sub`) using the dropdowns if needed.
4. Click **📋 Copy Full Alliance Plan (Team A & B)** to copy the battle plan.
