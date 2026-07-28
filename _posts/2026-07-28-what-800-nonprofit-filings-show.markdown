---
layout: post
title: "What 800 nonprofit filings show about proving your own numbers"
date: 2026-07-28 09:00:00 +0530
---

I spent a week reading the public filings of 800 American nonprofits, and I want to
describe one pattern I did not expect to find, along with the thing that made it
visible.

The organizations are all mid-sized — between five and twenty-five million dollars
of annual revenue — working in human services, education, youth development and
international development, spread across 54 states and territories. I pulled every
Form 990 available for each, up to thirteen years apiece.

I was looking for something narrow: whether the numbers these organizations report
to their funders can be traced back to the systems that produced them. What I found
first was something simpler, and stranger.

## Revenue that moves without the business moving

A Form 990 splits incoming money into a few lines. Two of them carry almost
everything a service organization receives. **Contributions and grants** covers
donations, foundation grants and government grants. **Program service revenue**
covers money earned by delivering the mission — fees, contracts, payments for
services rendered.

In 118 of these organizations — **16% of those with at least five years of
comparable filings** — one of those two lines moves by at least 25 percentage points
of total revenue in a single year, *while total revenue stays essentially flat.*

Not the organization growing. Not a funder arriving or leaving. The same money,
landing on a different line.

One organization reported 93 to 96% of its revenue as contributions for eleven
consecutive years, then 5% the following year — with total revenue slightly *up*.
Another sat at 98–99% for nine years, then dropped to 11%, while revenue rose by
five and a half million dollars. A third has crossed that boundary in both
directions, twice, and currently sits roughly where it started a decade ago.

Thirteen organizations oscillate — the line moves one way, then back again.

## Why this is not an accounting scandal

I want to be careful here, because the obvious reading is wrong.

There is a genuine, well-known ambiguity underneath this. When a government pays a
nonprofit, someone has to decide whether the government is *buying a service* — an
exchange transaction, which belongs in program service revenue — or *funding a
mission* without receiving commensurate value in return, which makes it a
contribution. For Medicaid-funded services, state contracts and pass-through county
money, that question is arguable in good faith.

It was arguable enough that in 2018 the Financial Accounting Standards Board issued
a standard, ASU 2018-08, specifically to reduce the inconsistency. It pushes in one
direction: most government grants and contracts are contributions, because the
government does not receive commensurate value.

So a reasonable person would expect these moves to cluster around 2019 to 2021, when
that standard took effect, and to run in one direction.

They do not.

| Year of move | Count |
|---|---|
| 2012–2018 | 76 |
| 2019–2021 | 30 |
| 2022–2024 | 32 |

More than half the moves predate the standard entirely. They run in both
directions. And when I read the audited financial statements behind a sample of
these organizations, only two of twenty-three reports mention ASU 2018-08 at all —
one of them as boilerplate about a pronouncement not yet adopted.

I also went looking for the most obvious false positive. Federal relief money
arriving in 2020 and leaving again produces exactly this signature: a line jumps,
then returns. I found 30 organizations in that pattern and excluded every one of
them. The 118 are what remains after that.

So this is not fraud, and it is mostly not a standard being adopted. It is
something less dramatic and more interesting: **a judgment call that gets made
again each year, by whoever is closest to the filing at the time.**

## Why it matters more than it looks

If this were only about presentation, it would be a curiosity. It isn't, for three
reasons.

**The public support test.** A public charity has to demonstrate, on a rolling
five-year lookback, that its money comes from a broad base. Contributions and
program service revenue are weighted differently in that calculation. A line that
moves eight million dollars inside the lookback window doesn't just make
year-over-year comparison awkward — it moves an input to the test that determines
the organization's tax status.

**Funder reporting.** Grant reports, board packets and renewal applications are
built on multi-year comparisons drawn from these same categories. If the underlying
definition changed in year three and the comparison wasn't rebuilt, the report
quietly compares two different things. Nobody notices, because the report is
assembled by a person who knows what they meant.

**That last clause is the actual finding.** A number that shifts category without a
documented reason is a number that no system is producing. It is being decided. And
a decision that lives in one person's judgment rather than in a rule is a decision
that leaves when they do.

## The document nobody reads

Partway through this I realized I was using the wrong source.

The Form 990 is the famous one — public, searchable, the basis of every charity
rating site. But it is a derived document, and it is old. Because organizations take
the automatic six-month filing extension and the IRS then needs months to process
and publish, the most recent fiscal year with near-complete coverage in my sample
was 2023. Only 12% had a 2024 filing available.

Meanwhile, any organization spending a million dollars or more in federal awards
must file a Single Audit — a full financial statement audit plus a compliance audit
against each major federal program — with the Federal Audit Clearinghouse. Those are
due nine months after fiscal year end, with no extension, and they post quickly.

In a 250-organization sample, **42% had a Single Audit on file. Of those, 82% had a
2024 or 2025 audit available** — against 12% with a 2024 Form 990.

The audit package contains the audited financial statements the 990 is derived
from, the notes that explain the accounting policies, every finding the auditor
raised, and the name and title of the person who signed for the organization. It is
free, public, and available through an API.

It is a strictly better document, roughly two years fresher, and almost nobody
outside the compliance world reads it.

The most interesting thing I found came out of that comparison. One organization's
audited statements state plainly that it adopted ASU 2018-08, under which grants and
contracts are treated as contributions. Its Form 990 for the same fiscal year shows
contributions falling from 100% of revenue to 20%. Two documents, one year, one
organization, pointing in opposite directions.

I am not naming it, and I want to be explicit about why. There is almost certainly
an explanation, the organization has done nothing wrong, and publishing a list of
charities whose filings look odd would be a way of manufacturing alarm in order to
sell a remedy. The pattern is worth writing about. The names are not mine to
publish.

## What I think this says

Every organization here has an auditor, a finance lead and a board. The
inconsistency isn't a competence problem, and it isn't a software problem — most of
them have perfectly good accounting systems.

It is a seam problem. Financial data lives in the accounting system. Delivery data —
who was served, how often, with what result — lives in case management systems,
service logs, timesheets and spreadsheets. Funder reports need both, cut on
calendars that match neither the fiscal year nor each other. Federal awards run
October to September, many state contracts July to June, foundations on their own
grant anniversaries.

Nobody's job title covers the join. So it gets done by hand, by someone who is good
at it, every reporting cycle, forever. It works. The reports go out. The audits come
back clean.

And the cost of it is invisible, because it's absorbed rather than spent — until the
person who knew how the spreadsheet worked takes another job, and the organization
discovers that a decade of its reported history rested on their memory.

---

*The analysis used the ProPublica Nonprofit Explorer API for Form 990 data and the
Federal Audit Clearinghouse API for Single Audit data. Both are public and free.
Figures are counts from the sample described, not national estimates.*

*I do independent assessments of exactly this problem for nonprofits — whether the
data can prove what the programs actually do. If it's relevant to you, my email is
[ravi@helloravi.com](mailto:ravi@helloravi.com).*
