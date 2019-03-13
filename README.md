# iCalEvents

Simple Python 3 library to download, parse and query iCal sources.

## Details

See https://github.com/irgangla/icalevents

This fork includes fixes to make sure that each occurrence of a
repeating event has the correct start and end time, even when the
repeating event crosses over a daylight saving time boundary.
