



**Phase 1: Data Collection**                                         

                                                                    

User                                                               

&nbsp; │

&nbsp; ▼

Decision Tree

&nbsp; │

&nbsp; ▼

Session Object Created

&nbsp; │

&nbsp; ▼

Complex Case?

&nbsp;  ├── No ────────────────┐

&nbsp;  │                      │

&nbsp;  └── Yes                │

&nbsp;       │                  │

&nbsp;       ▼                  │

&nbsp;    AI Chat               │

&nbsp;       │                  │

&nbsp;       ▼                  │

&nbsp;    aiSummary Generated   │

&nbsp;       │                  │

&nbsp;       └──────────┬───────┘

&nbsp;                  ▼

&nbsp;             Final Check

&nbsp;                  │

&nbsp;                  ▼

&nbsp;     POST /cheatsheet/generate







**Phase 2: CheatSheet Ganeration**





Backend Receives Request

&nbsp;       │

&nbsp;       ▼

Session + aiSummary Validation

&nbsp;       │

&nbsp;       ▼

AI Engine Generates Steps

&nbsp;       │

&nbsp;       ▼

Step Builder Enhances with GuideLibrary

&nbsp;       │

&nbsp;       ▼

Return Structured Cheatsheet JSON

&nbsp;       │

&nbsp;       ▼

Frontend Renders:

&nbsp; - Layer 1: Action Plan

&nbsp; - Layer 2: Detailed Guides

&nbsp; - Layer 3: Update Enabled





**Phase 3: Dynamic update flow**





User Clicks:

"My Situation Changed"

&nbsp;       │

&nbsp;       ▼

POST /cheatsheet/update

&nbsp;       │

&nbsp;       ▼

Backend:

&nbsp; - Preserve Completed Steps

&nbsp; - Send Remaining Context to AI

&nbsp;       │

&nbsp;       ▼

AI Replans Remaining Steps

&nbsp;       │

&nbsp;       ▼

Updated Cheatsheet Returned

&nbsp;       │

&nbsp;       ▼

Frontend Re-renders Plan

