ps-js-calendar
==============

Created by: Michał Buszkiewicz

## Purpose

Creating calendars with Photoshop is an utter nightmare if you really intend to do it manually. Slightly less so when you just need to create a single-page calendar with just months displayed on it, but when you want to make a full calendar with name-days printed, things get really complicated. That's what this script is for.

## Usage

Create a file for a specific month's calendar, containing a 'dayNumbers' layer set with the following structure (1 through 7 here are text layers):

### 
- dayNumbers
  * row1
    * 1
    * ...
    * 7
  * row(...)
    * (...)
  * row7
    * 1
    * ...
    * 7

Then create a similarly structured 'nameLabels' layer set for name-day display and just run the script in Photoshop.

Please note that as of now all name-day data are in Polish. Likewise, following the Polish convention, the first day of week is Monday. A certain degree of i18n is obviously a TODO.

## Tested on
For now, it's been tested on Photoshop CS6 only. I've no idea about backwards compatibility, but I reckon there's nothing as magical in this script that won't work on older versions supporting JS. Certainly a thing to check for the future.

## Task list
- [x] Puts day and name-day info on a laid-out PSD for a specific month
- [ ] Supports internationalization of name-day data
- [ ] Supports any additionay holiday info (Xmas, etc...)
- [ ] Creates all calendar files for a specific year automatically based on a template