# Output formats

## 1. Findings (chat and saved summaries)

Use this order unless the user asks for a different format. Keep table cells short. If there are no readable ads, give the coverage table and explain why findings are unavailable; skip the takeaway, mix and chart.

1. **Takeaway:** one sentence about the strongest pattern in the sample.
2. **Themes and offers:** use the table below. Show up to five rows per type, highest count first within each type. Use one primary theme and one primary offer per reviewed ad. If the offer is not visible, label it “Unknown”; use “No explicit offer” only when you could inspect it and saw none. Include a short example headline with a direct ad link if available. For multiple competitors, compare by competitor using each one's own reviewed total.

| Type | Theme or offer | Ads reviewed | Example ad |
|---|---|---:|---|
| Theme | <label> | <count>/<reviewed total> | <short linked headline> |
| Offer | <label> | <count>/<reviewed total> | <short linked headline> |

3. **Platform comparison:** include every requested platform. Put the country and date checked directly above the table. Show the actual window and reviewed count per platform. Note a sample cap, shorter coverage, no results, or an access block. Use “—” for unknown totals or unavailable findings. For leading offers, use the platform's own reviewed count as the denominator. If windows differ, call it out and avoid ranking activity across platforms.

| Platform | Actual window | Reviewed / shown | Leading offer | Coverage note |
|---|---|---:|---|---|
| <platform> | <window> | <reviewed>/<shown or —> | <offer> (<count>/<reviewed>) | <coverage or limitation> |

Only use a “shown” count when the library gives a total for that same scope. A blocked library is different from a library that returned zero results.

4. **Chart, when useful:** add at most one horizontal bar chart for the theme or offer mix when at least three categories have comparable counts and the chart makes the ranking easier to see. Label it “Ads reviewed (n = <total>)”, label each bar with its count, and keep the same categories and order as the table. Use a rendered chart when available or compact text bars in chat and plain Markdown. Skip the chart for sparse or incomparable data. Counts describe this sample; they do not measure spend, reach, or performance.
5. **What stands out:** up to three short bullets, each grounded in an observed count, date, or linked example. Useful signals include long-running ads, recent clusters of starts, visible creative variants, platform differences, or a buyer concern absent from the reviewed ads. Describe duration and variants without assuming success or an A/B test.

End by offering to save the full ad list to the computer or Notion.

## 2. Saved to the computer
Folder `competitor-ads/<competitor>-<YYYY-MM-DD>/`:
- `summary.md`: the findings above
- `ads.csv`: one row per ad, with these columns:
  `competitor, platform, country, period, checked_on, ad_link, format, headline, about, problem, speaks_to, proof, offer, call_to_action, started, still_running, versions`
- `screenshots/`: one image per ad, named `<platform>-<number>.png`, if you have them

## 3. Saved to Notion
One database, reused for every competitor, called **Competitor ads**:

| Column | Type |
|---|---|
| Headline | title |
| Competitor | select |
| Platform | select: LinkedIn, Google, Meta, TikTok, Microsoft, X, Pinterest, Snapchat |
| Country | select |
| Period | select: Running now, Last 30 days, Last 90 days, Last 12 months |
| Checked on | date |
| About | select (the theme label) |
| Offer | select: Demo, Free trial, Download, Webinar, Event, Discount, Other |
| Format | select: Image, Video, Carousel, Text, Other |
| Started | date |
| Still running | checkbox |
| Versions | number |
| Problem named | text |
| Speaks to | text |
| Proof | text |
| Call to action | text |
| Ad link | URL |

Plus one page per check, **"<Competitor> ads, <date>"**, with the findings and a link to the database filtered to that competitor and date. If screenshots exist, attach each one to its row.

Before creating the database, search Notion for an existing **Competitor ads** database and reuse it, so every check lands in the same place.
