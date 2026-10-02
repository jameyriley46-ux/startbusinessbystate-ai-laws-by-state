# State AI Laws and Bills by State, 2025-2026 (startbusinessbystate.com)

Which state AI laws reach ordinary businesses: bill and law counts by state and topic, plus law-level tables for chatbots, hiring, deepfakes, pricing algorithms and health care.

Main page: https://startbusinessbystate.com/ai-laws-by-state/

## Summary

State legislatures filed 1,351 AI bills in the 2025 and 2026 sessions, and 149 became law in 38 states. This dataset counts bills and laws by state and topic and lists, in plain language, the laws most likely to reach an ordinary business: chatbot disclosure, AI in hiring, deepfakes, pricing and rent algorithms, and AI in health care.

## Files

| File | Rows | What it is |
|---|---|---|
| `data/ai_chatbot_laws.csv` | 19 | State laws on chatbots and AI companions. |
| `data/ai_healthcare_bills_by_state.csv` | 43 | Health care AI bills by state. |
| `data/ai_healthcare_insurer_laws.csv` | 7 | Insurer AI rules that affect claims (utilization review). |
| `data/ai_healthcare_practice_laws.csv` | 5 | Rules for any medical practice or clinic using AI. |
| `data/ai_healthcare_therapy_laws.csv` | 8 | Laws that ban or limit AI therapy. |
| `data/ai_hiring_laws_by_state.csv` | 51 | AI in hiring and employment laws, one row per state. |
| `data/ai_laws_by_state_summary.csv` | 51 | AI bills and enacted laws by state, 2025-2026 sessions. |
| `data/ai_laws_by_topic.csv` | 22 | AI bills and laws by primary topic. |
| `data/ai_laws_key_business_laws.csv` | 32 | The 32 laws that reach ordinary businesses, in plain language. |
| `data/algorithmic_pricing_bills_by_state.csv` | 26 | Pricing and rent-algorithm bills by state. |
| `data/algorithmic_pricing_laws.csv` | 8 | Laws on pricing and rent-setting algorithms. |
| `data/deepfake_laws.csv` | 81 | Enacted state deepfake laws, one row per law. |

All files are UTF-8 CSV with a header row in snake_case. Blank cells mean the value is not available, not applicable, or suppressed by the source.

## Data dictionary

### data/ai_chatbot_laws.csv

State laws on chatbots and AI companions. Rows: 19. Columns: 9.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Law and session law citation. | text |
| `type` | Business chatbots, companion chatbots, mental health chatbots and similar. | category |
| `who_it_covers` | Who the law reaches. | text |
| `what_it_requires` | What it requires. | text |
| `starts` | Effective date. | text |
| `enforcement` | Who enforces it and penalties. | text |
| `source_url` | LegiScan or official bill page. | URL |

### data/ai_healthcare_bills_by_state.csv

Health care AI bills by state. Rows: 43. Columns: 3.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `bills_2025_2026` | Health care AI bills filed in 2025 and 2026 sessions. | bills |

### data/ai_healthcare_insurer_laws.csv

Insurer AI rules that affect claims (utilization review). Rows: 7. Columns: 6.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Law. | text |
| `starts` | Effective date or In force. | text |
| `what_it_requires` | What it does. | text |
| `source_urls` | Links (space separated). | URLs |

### data/ai_healthcare_practice_laws.csv

Rules for any medical practice or clinic using AI. Rows: 5. Columns: 6.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Law. | text |
| `starts` | Effective date or In force. | text |
| `what_it_requires` | What it means. | text |
| `source_urls` | Links (space separated). | URLs |

### data/ai_healthcare_therapy_laws.csv

Laws that ban or limit AI therapy. Rows: 8. Columns: 7.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Law. | text |
| `starts` | Effective date. | text |
| `what_it_requires` | What it means for a practice. | text |
| `penalty_or_enforcer` | Penalties and enforcer. | text |
| `source_urls` | Links (space separated). | URLs |

### data/ai_hiring_laws_by_state.csv

AI in hiring and employment laws, one row per state. Rows: 51. Columns: 9.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `status` | Law, rules, city law, or No AI hiring law. | category |
| `law` | Law or rule. | text |
| `what_it_requires` | What it requires. | text |
| `who_it_covers` | Employers covered. | text |
| `starts` | Effective date. | text |
| `ai_at_work_bills_2025_2026` | State bills on AI at work filed in 2025 and 2026 (hand-built list of 48 bills). | bills |
| `source_urls` | Links to official pages (space separated). | URLs |

### data/ai_laws_by_state_summary.csv

AI bills and enacted laws by state, 2025-2026 sessions. Rows: 51. Columns: 5.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `ai_bills_2025_2026` | State AI bills in 2025 and 2026 sessions (excludes resolutions, data center bills and incidental mentions). | bills |
| `ai_laws_enacted_2025_2026` | Curated count of AI laws enacted in 2025 and 2026 sessions. | laws |
| `key_laws_for_businesses` | Plain-language list of the state laws most likely to reach businesses. | text |

### data/ai_laws_by_topic.csv

AI bills and laws by primary topic. Rows: 22. Columns: 4.

| Column | Meaning | Units |
|---|---|---|
| `topic` | Primary topic. | category |
| `bills_filed_2025_2026` | State bills with this primary topic. | bills |
| `laws_enacted_2025_2026` | Curated enacted laws with this primary topic. | laws |
| `states_with_a_law` | Number of states (including DC) with at least one such law. | states |

### data/ai_laws_key_business_laws.csv

The 32 laws that reach ordinary businesses, in plain language. Rows: 32. Columns: 7.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Bill or law number. | text |
| `who_it_covers` | Who the law reaches. | text |
| `what_it_requires` | What it means for a business. | text |
| `starts` | Effective date or status. | text |
| `source_urls` | Links to the bill or official page (space separated). | URLs |

### data/algorithmic_pricing_bills_by_state.csv

Pricing and rent-algorithm bills by state. Rows: 26. Columns: 4.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `bills_2025_2026` | Bills filed in 2025 and 2026 sessions. | bills |
| `laws_and_notes` | Laws and pending items. | text |

### data/algorithmic_pricing_laws.csv

Laws on pricing and rent-setting algorithms. Rows: 8. Columns: 8.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `law` | Law. | text |
| `who_it_covers` | Who it hits. | text |
| `what_it_requires` | What it means for a business. | text |
| `starts` | Effective date or status. | text |
| `enforcement` | How it is enforced. | text |
| `source_urls` | Links (space separated). | URLs |

### data/deepfake_laws.csv

Enacted state deepfake laws, one row per law. Rows: 81. Columns: 7.

| Column | Meaning | Units |
|---|---|---|
| `state` | State name (50 states plus District of Columbia). | text |
| `abbr` | Two-letter USPS state code. | text |
| `category` | election, sexual, or fraud_likeness_other. | category |
| `law` | Bill number. | text |
| `year` | Session year enacted. | year |
| `note` | Notes. | text |
| `source_url` | LegiScan bill page. | URL |

## Sources

| Source | Link | License or status |
|---|---|---|
| LegiScan API (session lists, master lists, bill search and bill details), pulled September 29, 2026 | https://legiscan.com/ | CC BY 4.0 (LegiScan). Bill data courtesy of LegiScan. |
| Official state legislature bill pages and session laws (linked in the source_url and source_urls columns) | https://www.ncsl.org/about-state-legislatures/state-legislative-websites-directory | Facts from government sources |
| startbusinessbystate.com plain-language summaries and classifications | https://startbusinessbystate.com/ai-laws-by-state/ | Our own compilation |

## Methodology

- We ran 25 LegiScan keyword searches (artificial intelligence, deepfake, chatbot, algorithmic discrimination, automated decision, synthetic media, digital replica, and others) for 2025 and 2026, then matched every hit to the session master lists.
- A bill counts as an AI bill only if its title or description uses an AI term. Bills that mention AI only in the full text (budgets and similar) are left out. Data center bills are tracked separately in the startbusinessbystate-data-center-boom dataset and are not in these counts.
- Each bill gets one primary topic by keyword rules, followed by a hand review. Enacted laws were then checked by hand against bill texts, which is why the curated law counts (149 laws) are lower than raw LegiScan "enacted" status counts.
- Resolutions and federal bills are not in the state counts.
- The law tables (chatbot, hiring, deepfake, pricing, health care, key business laws) were written by hand from bill texts and official pages.

## Limitations

- This is a research screen, not legal advice. Read the law and check effective dates before acting.
- A law is missed if its title and description never mention AI.
- City laws (such as New York City Local Law 144) and agency rules are not legislation and are only noted where relevant.
- Many states never mark dead bills as failed, so bills shown as filed include bills that are effectively dead.
- Status can change daily during sessions. The governor actions after September 29, 2026 that we know of (California SB 947 and SB 951, signed September 30) are reflected in the state summary and hiring tables only. The topic table was not updated for them, so its law column sums to 147 while the state table sums to 149.

## As-of date

LegiScan pulled September 29, 2026. Hub and hiring tables updated October 1, 2026 (California SB 947 and SB 951 signed September 30, 2026).

Version 1.0.0, released 2026-10-02.

## How to cite

StartBusinessByState. (2026). *State AI Laws and Bills by State, 2025-2026 (startbusinessbystate.com)* (Version 1.0.0) [Data set]. startbusinessbystate.com. https://github.com/jameyriley46-ux/startbusinessbystate-ai-laws-by-state

Please also credit the original sources listed above. When you use the data, a link back to https://startbusinessbystate.com/ai-laws-by-state/ is appreciated.

## Related pages on startbusinessbystate.com

- https://startbusinessbystate.com/ai-laws-by-state/
- https://startbusinessbystate.com/ai-chatbot-laws-by-state/
- https://startbusinessbystate.com/ai-hiring-laws-by-state/
- https://startbusinessbystate.com/deepfake-laws-by-state/
- https://startbusinessbystate.com/algorithmic-pricing-laws-by-state/
- https://startbusinessbystate.com/ai-healthcare-laws-by-state/

## License

This dataset is released under the Creative Commons Attribution 4.0 International license (CC BY 4.0). See `LICENSE`. You may share and adapt it, including for commercial use, as long as you give credit.
Underlying public domain data from U.S. government agencies stays public domain. Data from CC BY sources (such as LegiScan, PatentsView, Epoch AI or the Anthropic Economic Index, where used) also requires credit to those sources.

## Contact

StartBusinessByState (startbusinessbystate.com) (https://startbusinessbystate.com/)
