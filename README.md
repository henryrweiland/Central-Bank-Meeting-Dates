# Central Bank Meeting Dates

See below for notes on each CSV file. **Every central bank operates distinctly, and many of their policies change over time**.

This data is featured in *"Who's the Leader? Evaluating International Monetary Policy Spillovers"* (Weiland & Yeo 2024).

## Federal Reserve (Fed)
- **fomc_activity_date**: Corresponds to all FOMC activity: regularly scheduled meetings, conference calls, and minute releases.
- **fomc_meeting_date_indicator**: Equals 1 for regularly scheduled meetings/conference calls and 0 for minute releases.
- **fomc_non_scheduled_meeting_date_indicator**: Equals 1 for conference calls and 0 for regularly scheduled meetings.
- **fomc_projection_materials_indicator**: Equals 1 for FOMC meetings accompanied by projection materials (4 times annually, starting in 2009), 0 otherwise.
- **fomc_minutes_date_indicator**: Equals 1 for minute releases (usually with a lag after policy meetings), 0 otherwise.

Source: FOMC website.

## Bank of England (BOE)
**The BOE switched policies on 08/06/2015. Before, they held a MP decision meeting, released minutes with a 1-2 week lag, and then projection materials 2-4 weeks later. After 08/06/2015, the BOE released all three (decision, projection materials, minutes) on every MP day.**
- **boe_activity_date**: Corresponds to all BOE activity: regularly scheduled meetings, projection materials, and minute releases.
- **boe_meeting_date_indicator**: Equals 1 for regularly/non-scheduled meetings and 0 for projection material/minute releases before 08/06/2015.
- **boe_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled meetings and 0 for regularly scheduled meetings.
- **boe_projection_materials_indicator**: Equals 1 for BOE meetings accompanied by projection/inflation materials. Note the policy change stated above.
- **boe_minutes_date_indicator**: Equals 1 for minute releases, 0 otherwise. Note the policy change stated above.

Source: BOE website.


