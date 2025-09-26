# AIMR-Brainstorm Study Data

This repository contains anonymized datasets from the AIMR-Brainstorm study, which evaluated an **AI-enhanced Mixed Reality (MR) brainstorming system** against traditional sticky-note brainstorming. The data support our MDPI 2025 submission



## Datasets

### `merged_data.csv`

- **Rows:** ~30 (one per participant/condition)  
- **Description:** Contains survey responses, demographic info, engagement/creativity ratings, and preference data.  

**Schema**

| Column | Type | Description |
|--------|------|-------------|
| `participant_id` | int | Unique anonymized participant ID |
| `condition` | string | `sticky` or `aimr` (brainstorming condition) |
| `engagement_score` | float | Likert-scale engagement rating |
| `creativity_score` | float | Likert-scale perceived creativity |
| `usability_score` | float | Usability rating |
| `preference` | string | Participant’s preferred system |
| … | … | Additional measures (see paper) |

**Preview (first 5 rows)**

```text
participant_id,condition,engagement_score,creativity_score,usability_score,preference
1,sticky,3.5,3.8,4.0,aimr
1,aimr,4.4,4.7,4.1,aimr
2,sticky,3.2,3.5,3.9,sticky
2,aimr,4.5,4.6,4.2,aimr
3,sticky,3.7,3.9,4.0,aimr
```

### `merged_data.csv`

- **Rows:** Same participants × conditions (NASA-TLX responses) 
- **Description:** NASA-TLX workload subscales for each condition. 

**Preview (first 5 rows)**

```
participant_id,condition,mental_demand,physical_demand,temporal_demand,performance,effort,frustration
1,sticky,45,20,40,70,50,35
1,aimr,40,25,45,75,48,30
2,sticky,42,22,41,68,49,34
2,aimr,38,21,39,73,46,29
3,sticky,44,19,42,72,51,36
```





