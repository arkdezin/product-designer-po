# Solution Exploration

## Options Considered
### Optoion A - Structured Email + Shared Spreadsheet (Minimal)
Standardise the current Excel handoff with a shared cloud spreadsheet (Google Sheets or SharePoint), define email templates for approval actions, and add a shared mailbox for flagging. No new tooling or engineering required.
> `Effort: Very Low`    
> `Solves: Versioning and visibility partially`  
> `Does not solve: Structured workflow, audit trail, or feedback loop` 

### Option B - Centralised Workflow Layer in Admin Portal (Balanced)
Build a dedicated Catalog Maintenance module in the existing Intrics Admin portal. DE sends data to a structured intake queue instead of emailing Excel files. DM reviews, accepts or overrides AI suggestions, and approves products for publish - within the same weekly cycle. Business users flag issues through the platform with structured justification. DM handles secondary review in the same interface.
> `Effort: Medium`    
> `Solves: All five identified hotspots`    
> `Preserves: Existing upstream systems; no replacement required` 

### Option C - Full Automated Pipeline with ML Confidence Thresholds (Ideal State)
Replace manual review with automated acceptance for high-confidence AI outputs. Only low-confidence records are routed to DM for human review. Introduce a quality scoring system, full audit log, and real-time dashboards per team. DM review capacity scales without headcount growth.
> `Effort: Very High`    
> `Solves: Everything, and reduces manual review further`   
> `Risk: Requires ML confidence thresholds that do not exist; premature automation without baseline data` 

## Option Evaluation Matrix
| Criterion | Weight | Option A | Option B | Option C |
| -- | -- | -- | -- | -- |
| Impact on primary metric | High | Low | High | High |
| Engineering effort | High | Low | Medium | High |
| User value | High | Low | High | High |
| Strategic alignment | Medium | Low | High | Medium |
| Time to ship | Medium | High | Medium | Low |
| Risk level | Medium | Low | Low | High |

## Recommendation
> **Option B** - Centralised Workflow Layer
