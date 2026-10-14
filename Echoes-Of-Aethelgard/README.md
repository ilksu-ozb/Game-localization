# Echoes of Aethelgard - Turkish Localization Case Study

> **Disclaimer:**  
> This case study was developed as a hands-on localization exercise. The source JSON strings, character dialogue scenarios, and game context were AI-generated to simulate a realistic indie Dark Fantasy RPG localization workflow. All Turkish translations, style guidelines, glossary terms, and quality control passes were executed and validated manually to demonstrate end-to-end game localization and LQA skills.

---

## 1. Project Overview
* **Game Genre:** Dark Fantasy / Narrative RPG
* **Target Audience:** Core RPG players, 18+
* **Tone & Atmosphere:** Grim, eerie, medieval, serious.

---

## 2. Style Guide & Localization Rules

### A. Tone of Voice 
* **General Tone:** Formal and atmospheric medieval Turkish.
* **NPC Interaction:** Elder/Guide NPCs use singular informal ("Sen") with a maternal/paternal advisory tone. Smugglers and merchants use colloquial/hostile tone ("Dostum").
* **UI & System Prompts:** Polite formal ("Siz / Ediniz") for system errors and save confirmations (`"İnternet ayarlarınızı kontrol edin"`).

### B. Technical Rules
* **Variables:** All variables (`{player_name}`, `{gold_cost}`, `{duration}`) are strictly preserved and adapted to Turkish grammar rules.
* **Escape Characters:** Line breaks (`\n`) maintained for UI layout consistency.
* **Character Limits:** UI button strings strictly kept under 25 characters to prevent box overflow.

---

## 3. Key Terminology (Glossary)

| Source Term (EN) | Target Term (TR) | Context / Usage Notes |
| :--- | :--- | :--- |
| **Miasma** | Miasma / Zehirli Sis | World concept. Left untranslated as proper noun in narrative contexts. |
| **Dreadveil** | Dreadveil | Main antagonistic force/realm. Left untranslated as proper noun in narrative contexts. |
| **Keepers** | Koruyucular | Enemy faction guards. |
| **Warden** | Başgardiyan | Dungeon administrator title. |
| **Lockpick** | Maymuncuk | Inventory interaction item. |
| **Iron Dungeon** | Demir Zindan | Key location name. |