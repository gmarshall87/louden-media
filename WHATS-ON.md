# What's on (website feed)

`whats-on.json` feeds the "What's on" section on the home page of theloudentavern.co.uk.
The page reads it live from:
https://raw.githubusercontent.com/gmarshall87/louden-media/main/whats-on.json

The page hides anything dated before today and shows the next four items, so past
items can stay in the file. Changes show on the site within about five minutes of a commit.

## Fields

| Field | Meaning |
| --- | --- |
| date | YYYY-MM-DD, UK date of the fixture or event |
| kind | home, away, cup or event |
| title | e.g. "Rangers v Aberdeen". Home team first. |
| where | Ground or venue, e.g. "Ibrox", "Easter Road", "Hampden" |
| kickoff | e.g. "8pm", "7.45pm". Leave empty if not confirmed. |
| open | When The Louden opens that day, e.g. "11am", "4pm" |
| tv | UK channel if confirmed, else empty. Only fill for away or cup games. |
| note | One short line, e.g. bus details. Optional. |
| status | confirmed or provisional. Provisional shows "Kick-off TBC". |
| link / linkText | Optional button, e.g. Square booking link |

## Rules

- Celtic fixtures and Celtic results are never listed or promoted. Old Firm games are listed as Rangers events only.
- Opening times: 11am on Saturdays, Sundays and daytime kick-offs; 4pm for midweek evening kick-offs. Old Firm games kick off at 12:00 unless confirmed otherwise.
- Only list a kick-off time or TV channel when at least two sources agree, or one official source (Rangers, SPFL, broadcaster) confirms it. Otherwise status "provisional" and leave the field empty.
- Fixture dates, kick-offs, TV picks and the removal of postponed games are factual updates and can be committed without approval.
- New events, offers, prices or booking links (anything sold or promoted) need Greg's approval before they are added.
- UK English, no em dashes, "The Louden", no "craic".
