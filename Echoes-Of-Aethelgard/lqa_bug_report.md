# Echoes of Aethelgard - LQA Bug Report (TR)

> **Disclaimer:**  
> This document is a simulated Localization Quality Assurance (LQA) bug report. The issues listed below (Visual Overflow, Context/Gender Mismatch, and Unresolved Variable Tags) are hypothetical test cases created to demonstrate standard LQA reporting protocols, JIRA-style bug tracking formatting, and severity categorization for game localization workflows.

---
 
* **Language Tested:** Turkish (tr_TR)  

---

### Bug #1: Inventory Item Description Text Overflow
* **Bug ID:** `EAE-TR-001`
* **Category:** Visual / Cosmetic
* **Severity:** Major
* **Steps to Reproduce:**
  1. Open the Game Main Menu and select "Resume Journey".
  2. Open Inventory by pressing `[I]`.
  3. Hover over the "Elixir of Concealment" (Gizlenme İksiri) item.
  4. Observe the item description box at the bottom right.
* **Current Result:** The last sentence of `item_potion_shadow_desc` overflows the UI bounding box and is cut off (`"...oranında azalır."` is invisible).
* **Expected Result:** Reduce font size by 2pt or adjust line breaks (`\n`) so the full sentence fits inside the UI panel.

---

### Bug #2: Unresolved String Variable in Achievement Pop-up
* **Bug ID:** `EAE-TR-002`
* **Category:** Functional / Localization Code
* **Severity:** Major
* **Steps to Reproduce:**
  1. Escape the Iron Dungeon without triggering any guard alerts.
  2. Wait for the achievement notification pop-up.
* **Current Result:** The pop-up reads `"BAŞARI KİLİDİ AÇILDI: {achievement_name}"` (the variable tag is displayed literally).
* **Expected Result:** The game engine should pull the localized achievement title string (e.g., `"BAŞARI KİLİDİ AÇILDI: Hayalet Adımlar"`).