# Central Bank Meeting Dates

See below for notes on each CSV file. **Every central bank operates distinctly, and many of their policies change over time**.

This data is featured in *"Who's the Leader? Evaluating International Monetary Policy Spillovers"* (Weiland & Yeo 2024).

A useful resource can also be found on the [BIS website](https://www.bis.org/mc/currency_areas.htm).

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
- **ecb_projection_materials_indicator**: Equals 1 for ECB meetings accompanied by projection materials (first released in 2005).
- **ecb_minutes_date_indicator**: Equals 1 for minute releases (first released in 2015, usually with a lag after policy meetings), 0 otherwise.

## Bundesbank (Buba)
Range: 1975-1988.

**The Bundesbank met ~24 times anually, though not all of their meetings correspond to policy decisions. Historical minutes from the Bundesbank archive were only available as recent as 1988.**

- **buba_activity_date**: Corresponds to all Buba activity: regularly scheduled meetings.
- **buba_meeting_date_indicator**: Equals 1 for regularly scheduled meetings (all samples are 1. It is unknown if any of the meetings were unscheduled).
- **buba_policy_decision_indicator**: Equals 1 for Buba meetings with significant policy decision (interest rate, reserve requirements, monetary supply, etc.), 0 otherwise (which corresponds to meetings only with discussion). In order to classify each meeting, the minutes (in German) were summarized by GPT 3.5 and hand-coded either 0 or 1.

## Bank of Canada (BOC)
Range: 2000-2023.

**The BOC does not release minutes after MPC meetings, only projection materials.**

- **boc_activity_date**: Corresponds to all BOC activity: regularly scheduled meetings.
- **boc_meeting_date_indicator**: Equals 1 for regularly scheduled meetings (there are no non-scheduled BOC meetings in sample).
- **boc_projection_materials_indicator**: Equals 1 for BOC meetings accompanied by projection/inflation materials.

## Bank of Japan (BOJ)
Range: 2000-2023.

- **boj_activity_date**: Corresponds to all BOJ activity: regularly/non-regularly scheduled meetings and minute releases.
- **boj_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise.
- **boj_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled meetings and 0 for regularly scheduled meetings.
- **boj_projection_materials_indicator**: Equals 1 for BOJ meetings accompanied by projection/inflation materials.
- **boj_minutes_date_indicator**: Equals 1 for minute releases (released with a lag), 0 otherwise.

## Reserve Bank of Australia (RBA)
Range: 2006-2023.

- **rba_activity_date**: Corresponds to all RBA activity: regularly scheduled meetings, projection materials and minute releases (latter two are on separate days from monetary policy meetings).
- **rba_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise.
- **rba_projection_materials_indicator**: Equals 1 for date of RBA projection material release (released with a lag), 0 otherwise.
- **rba_minutes_date_indicator**: Equals 1 for date of RBA minute release (released with a lag), 0 otherwise.

## Reserve Bank of New Zealand (RBNZ)
Range: 2000-2023.

**The RBNZ does not release minutes after MPC meetings.**

- **rbnz_activity_date**: Corresponds to all RBNZ activity: regularly scheduled meetings.
- **rbnz_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **rbnz_projection_materials_indicator**: Equals 1 for date of RBNZ projection material release (released on date of MP meeting), 0 otherwise.

## Bank of Mexico (Banxico)
Range: 2000-2023 (meetings and projection materials), 2018-2023 (minutes).

**Banxico releases their MP decision, projection materials, and minutes on separate days, much like the BOE before 2015.**

- **banxico_activity_date**: Corresponds to all Banxico activity: regularly scheduled meetings, projection materials, and minute releases.
- **banxico_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **banxico_projection_materials_indicator**: Equals 1 for date of Banxico projection material release (released with a lag), 0 otherwise.
- **banxico_minutes_dates_indicator**: Equals 1 for date of Banxico minute release (released with a lag), 0 otherwise.

## Central Bank of Chile (CBC)
Range: 2000-2023

**The CBC also releases minutes with a two-week lag, but the exact dates were not able to be obtained. Before 2018, the CBC released their projection materials with a delay after MP meetings, but after 2018, they released projection materials concurrently.**

- **cbc_activity_date**: Corresponds to all CBC activity: regularly scheduled meetings and projection materials.
- **cbc_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **cbc_projection_materials_indicator**: Equals 1 for date of CBC projection material release (released with a lag before 2018), 0 otherwise.

## Central Bank of Colombia (BanRep)
Range: 2000-2023 (projection materials), 2008-2023 (meetings and minutes)

- **banrep_activity_date**: Corresponds to all BanRep activity: regularly scheduled meetings, projection materials and minute releases.
- **banrep_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **banrep_projection_materials_indicator**: Equals 1 for date of BanRep projection material release (released with varying lag over the sample), 0 otherwise.
- **banrep_minutes_dates_indicator**: Equals 1 for date of BanRep minute release (released with varying lag over the sample), 0 otherwise.

## Bank of Israel (BOI)
Range: 2006-2023 (meetings and minutes), 2014-2023 (projection materials)

**Bank of Israel Law 5770-2010 established the monetary policy committee, which started holding meetings in 2011, but the Governor still made interest rate announcements prior, which are recorded dating back to 2006. Minutes were previously released with a lag after MP meetings, but starting in 2018, they were released concurrently.**

- **boi_activity_date**: Corresponds to all BOI activity: regularly scheduled meetings, projection materials and minute releases.
- **boi_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **boi_projection_materials_indicator**: Equals 1 for date of BOI projection material release (relased bi-anually with a lag), 0 otherwise.
- **boi_minutes_dates_indicator**: Equals 1 for date of BOI minute release, 0 otherwise. Note the policy change stated above.

## South African Reserve Bank (SARB)
Range: 2000-2023

**The SARB does not publish minutes after MPC meetings.**

- **sarb_activity_date**: Corresponds to all SARB activity: regularly scheduled meetings and projection materials.
- **sarb_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **sarb_projection_materials_indicator**: Equals 1 for date of SARB projection material release (relased quarterly with a lag), 0 otherwise.

## Reserve Bank of India (RBI)
Range: 2000-2023 (meetings), 2014-2023 (projection materials), 2016-2023 (minutes)

**The RBI switched policies starting in 2014. Before, they released an annual MP statement, followed by a first, second, and third quarter review (with no projection materials or minutes). They then switched to six annual MP meetings, with bi-annual projection material releases (April and October), and regular minutes starting in 2016. Before 2014, mid-quarter reviews were not accounted for as RBI activity.**

- **rbi_activity_date**: Corresponds to all RBI activity: regularly scheduled meetings, projection materials, and minute releases.
- **rbi_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are no unscheduled meetings in sample).
- **rbi_projection_materials_indicator**: Equals 1 for date of RBI projection material release (relased bi-anually on same day as MPC meeting), 0 otherwise. Note the policy change stated above.
- **rbi_minutes_dates_indicator**: Equals 1 for date of RBI minute release (released with two week lag), 0 otherwise. Note the policy change stated above.

## Bank of Thailand (BOT)
Range: 2000-2023 (meetings), 2011-2023 (minutes)

**The BOT publishes a quarterly MP report, but release dates were not able to be obatined. Moreover, it appears that a Thai version of the MP report is released one week before the English version, making it unclear how information from the publication is disseminated.**

- **bot_activity_date**: Corresponds to all BOT activity: regularly scheduled meetings and minute releases.
- **bot_meeting_date_indicator**: Equals 1 for regularly scheduled meetings, 0 otherwise (there are 2 unscheduled meetings in sample).
- **bot_non_scheduled_meeting_date_indicator**: Equals 1 for non-scheduled (surprise) meetings and 0 for regularly scheduled meetings.
- **bot_minutes_dates_indicator**: Equals 1 for date of BOT minute release (released with two week lag), 0 otherwise.

