# Evidence for the Computing Budget

## Rates and their sources

| Item | Value | Source |
|---|---|---|
| Ohio Supercomputer Center (OSC) standard compute, Ohio academic | $0.003 per core-hour | OSC Service Costs, https://www.osc.edu/book/export/html/4887 |
| OSC GPU compute, Ohio academic | $0.090 per GPU-hour | Same page |
| OSC project storage, Ohio academic | $3.20 per TB-month | Same page |
| OSC annual credit per principal investigator | $1,000 | Same page; https://www.osc.edu/content/academic_fee_model_faq |
| Fiscal year 2026 pricing unchanged for existing services | — | https://www.osc.edu/content/academic_fee_model_faq/fy26_budgets_action_may_be_required%EF%BB%BF |
| GPU jobs charge core-hours and GPU-hours together; storage billed daily on quota | — | https://www.osc.edu/supercomputing/knowledge-base/job_and_storage_charging |
| Storage billed on quota, not usage | — | https://osc.edu/sites/default/files/supercomputing/policies/docs/Project%20Filesystem%20Storage%20Policy%20-%201.2.pdf |
| Claude Max licence | $50 per seat per month | Ohio State negotiated price, given by the investigator |

## Verification status

- osc.edu could not be opened from the working environment on 9 October 2026 because the network policy blocked it. The rates above come from search-indexed copies of the pages listed. Confirm them on the live Service Costs page before submission.
- The Service Costs page gives one standard compute rate for Ohio academic clients and does not name Cardinal specifically. The budget assumes Cardinal is billed at that rate. OSC states that newer clusters (Ascend) follow the same pricing structure as earlier ones.

## Usage assumptions

| Scenario | Runs per week | Cores per run | Hours per run | Weekly core-hours | Weeks per year | Yearly core-hours |
|---|---|---|---|---|---|---|
| Off-peak | 10 | 32 | 2 | 640 | 20 | 12,800 |
| Average | 25 | 64 | 3 | 4,800 | 24 | 115,200 |
| Peak | 2 | 96 | 120 | 23,040 | 8 | 184,320 |
| Total | | | | | 52 | 312,320 |

Basis: the investigator reported a typical test run of 32 cores for about 2 hours, test batches of 10 to 33 runs, production runs of several days, and a maximum of 96 cores. The split of weeks and the 5-day production run length are assumptions and can be edited in `computing_budget.xlsx`.
