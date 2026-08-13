Retail Profitability Dashboard — Power BI
Power BI · DAX measures · margin-vs-target tracking · geographic and segment drill-downs
> Independent analysis project on a course-provided retail transaction dataset. The dataset is course-licensed and not redistributed; the dashboard is documented here through screenshots.
Problem
A retail business needs one screen that answers three management questions at once: are we hitting margin targets, where (geographically) is profit generated, and which product lines and customer segments drive or drag profitability?
Data
Retail transaction data with order dates, region/city, product sub-categories, customer segments, sales and profit fields.
Method
DAX measure layer: calculated gross-profit and operating-profit measures with explicit OPM / GPM target measures, so every margin visual reads actual-vs-target rather than actual alone.
Dashboard design (single page, eight coordinated visuals): date slicer driving the whole page; KPI cards for gross and operating profit; an Azure map of gross profit by region and city; two combo charts tracking operating-profit margin and gross-profit margin against their targets by sub-category; sales-mix donut by sub-category; customer-type pie and a segment-level gross-profit column chart.
Interaction model: cross-filtering between geography, sub-category and segment, so a manager can isolate any region-category-segment slice in two clicks.
So what
Margin-vs-target framing turns a reporting page into a management tool: the question shifts from "what were sales?" to "which slice of the business is missing its target, and by how much?" The same actual-vs-target measure pattern applies to any KPI dashboard — program outcomes, service delivery, budget tracking.
Repo contents
```
screenshots/   full-page dashboard capture
README.md
```
The .pbix file is available for a walkthrough on request — the underlying dataset is course-licensed and not redistributed.

