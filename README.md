# Central Bank Meeting Dates

See below for notes on each CSV file. **Every central bank operates distinctly, and many of their policies change over time**.

This data is featured in *"Who's the Leader? Evaluating International Monetary Policy Spillovers"* (Weiland & Yeo 2024).

## Federal Reserve (Fed)
Range: 1975-2023.
- **fed_activity_date**: Corresponds to all FOMC activity: regularly scheduled meetings, conference calls, and minute releases.
- **fed_meeting_date_indicator**: Equals 1 for regularly scheduled meetings/conference calls and 0 for minute releases.
- **fed_non_scheduled_meeting_date_indicator**: Equals 1 for conference calls and 0 for regularly scheduled meetings.
- **fed_projection_materials_indicator**: Equals 1 for FOMC meetings accompanied by projection materials (4 times annually, starting in 2009), 0 otherwise.
- **fed_minutes_date_indicator**: Equals 1 for minute releases (usually with a lag after policy meetings), 0 otherwise.

## Bank of England (BOE)
Range: 2000-2023.

**The BOE switched policies on 08/06/2015. Before, they held a MP decision meeting, released minutes with a 1-2 week lag, and then projection materials 2-4 weeks later. After 08/06/2015, the BOE released all three (decision, projection materials, minutes) on every MP day.**
- **boe_activity_date**: Corresponds to all BOE activity: regularly scheduled meetings, projection materials, and minute releases.
- **boe_meeting_date_indicator**: Equals 1 for regularly/non-scheduled meetings and 0 for projection material/minute releases before 08/06/2015.
- **boe_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled meetings and 0 for regularly scheduled meetings.
- **boe_projection_materials_indicator**: Equals 1 for BOE meetings accompanied by projection/inflation materials. Note the policy change stated above.
- **boe_minutes_date_indicator**: Equals 1 for minute releases, 0 otherwise. Note the policy change stated above.

## European Central Bank (ECB)
Range: 2000-2023.
- **ecb_activity_date**: Corresponds to all ECB activity: regularly scheduled meetings, non-regularly scheduled meetings, and minute releases.
- **ecb_meeting_date_indicator**: Equals 1 for regularly scheduled/non-scheduled meetings and 0 for minute releases.
- **ecb_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled meetings and 0 for regularly scheduled meetings (only one such date in sample).
- **ecb_projection_materials_indicator**: Equals 1 for FOMC meetings accompanied by projection materials (first released in 2005).
- **ecb_minutes_date_indicator**: Equals 1 for minute releases (first released in 2015, usually with a lag after policy meetings), 0 otherwise.

## Bundesbank (Buba)
Range: 1975-1988.

**The Bundesbank met ~24 times anually, though not all of their meetings correspond to policy decisions. Historical minutes from the Bundesbank archive were only available until 1988.**
- **buba_activity_date**: Corresponds to all Buba activity: regularly scheduled meetings.
- **buba_meeting_date_indicator**: Equals 1 for regularly scheduled meetings (all samples are 1. It is unknown if any of the meetings were unscheduled).
- **buba_policy_decision_indicator**: Equals 1 for Buba meetings with significant policy decision (interest rate, reserve requirements, monetary supply, etc.), 0 otherwise (which corresponds to meetings only with discussion). In order to classify each meeting, the minutes (in German) were summarized by GPT 3.5 and hand-coded either 0 or 1.

## Bank of Canada (BOC)
Range: 2000-2023.

**The BOC does not release minutes, only projection materials.**
- **boc_activity_date**: Corresponds to all BOC activity: regularly scheduled meetings.
- **boc_meeting_date_indicator**: Equals 1 for regularly scheduled meetings (there are no non-scheduled BOC meetings in sample).
- **boc_projection_materials_indicator**: Equals 1 for BOC meetings accompanied by projection/inflation materials.

## Bank of Japan (BOJ)
Range: 2000-2023.

- **boj_activity_date**: Corresponds to all BOJ activity: regularly and non-regularly scheduled meetings.
- **boj_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise.
- **boj_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled meetings and 0 for regularly scheduled meetings.
- **boj_projection_materials_indicator**: Equals 1 for BOJ meetings accompanied by projection/inflation materials.
- **boj_minutes_date_indicator**: Equals 1 for minute releases (released with a lag), 0 otherwise


