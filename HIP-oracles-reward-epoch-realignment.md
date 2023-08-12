# Oracle Reward Epoch Alignment

- Author(s): @bbalser (Nova Labs, Inc.)
- Start Date: 2023-08-11
- Category: Technical
- Original HIP PR: <!-- leave this empty; maintainer will fill in ID of this pull request -->
- Tracking Issue: <!-- leave this empty; maintainer will create a discussion issue -->
- Vote Requirements: <!-- veHNT Holders, veIOT Holders, or veMOBILE Holders -->

## Summary

Change the oracle reward epoch from 01:00:00 UTC - 00:59:59 UTC to 00:00:00 UTC - 23:59:59 UTC.  

## Motivation

Because the reward curve always changes at 00:00:00 UTC, ex. 2023-08-01 00:00:00 UTC, having the rewards epoch
start at 00:00:00 UTC and end at 23:59:59 UTC allows all the rewards in the epoch to be earned at the
same rate.

## Stakeholders

This proposal impacts all current and future participants in the Helium IoT & Mobile Community.

## Detailed Explanation

On a date to be specified, the reward epoch will be a 23 hour epoch from 01:00:00 UTC to 23:59:59 UTC.
After this date, the rewards epoch will always be a 24 hour epoch that start at 00:00:00 UTC and ends at 23:59:59 UTC.

## Drawbacks

There will be one day where rewards will be for a 23 hour epoch.

