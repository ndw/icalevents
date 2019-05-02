# iCalEvents

Simple Python 3 library to download, parse and query iCal sources.

## Details

See https://github.com/irgangla/icalevents

This fork includes several fixes:

* Make sure that attendee and organizer are universally present
* Fix mangling of timezone, see https://github.com/irgangla/icalevents/issues/12#issuecomment-456121570
* Keep track of all the timezones defined in the file; attempt to map events to the right timezone
* Ignore dates listed as exceptions (i.e., handle EXDATE)
* Recompute start time of recurring events in the current timezone (prevent recurring events from
  being off by an hour if the recurrence crosses a daylight saving time boundary)

2 May 2019: the upstream repo seems to have taken a different approach
to dealing with repeating all-day events where the timezone isn’t
present. I haven’t tested the results extensively.
