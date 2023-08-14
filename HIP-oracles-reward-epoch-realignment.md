# Oracle Reward Epoch Alignment

- Author(s): @bbalser (Nova Labs, Inc.)
- Start Date: 2023-08-11
- Category: Technical
- Original HIP PR: <!-- leave this empty; maintainer will fill in ID of this pull request -->
- Tracking Issue: <!-- leave this empty; maintainer will create a discussion issue -->
- Vote Requirements: <!-- veHNT Holders, veIOT Holders, or veMOBILE Holders -->

## Summary

Change the oracle reward epoch, which currently starts at 01:00:00 UTC and goes until the 01:00:00 UTC the following day, 
to starting at 00:00:00 UTC and going until 00:00:00 UTC the following day.

## Motivation

Because the reward curve always changes at 00:00:00 UTC, ex. 2023-08-01 00:00:00 UTC, having the rewards epoch
start and end at 01:00:00 UTC allows all the rewards in the epoch to be earned at the
same rate.

## Stakeholders

This proposal impacts all current and future participants in the Helium IoT & Mobile Community.

## Detailed Explanation

On a date to be specified, the reward epoch will be a 23 hour epoch from 01:00:00 UTC to 
After this date, the rewards epoch will always be a 24 hour epoch that start at 00:00:00 UTC and ends at 00:00:00 UTC.

The following table outlines the total reward pool for a 24 hour epoch and what the rewards would be for a 23 hour epoch.

|   | 24 hour epoch | 23 hour epoch |
| - | ------------- | ------------- |
| IOT | 88,797,814.21 | 85,097,905.28 |
| MOBILE | 81,967,213.11 | 78,551,912.57 |


## Drawbacks

There will be one day where rewards will be for a 23 hour epoch.

* All time ranges have an inclusive start and exclusive end