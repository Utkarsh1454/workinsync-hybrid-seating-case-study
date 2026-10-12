# Hybrid Workplace Seating Optimization

A case study I wrote for the Technical Account Manager / Implementation Intern role at WorkInSync (by MoveInSync).

## 1. The question

I am the facility manager for three offices in three countries. 2,000 employees need to be seated, and each one comes in three days a week. How many seats are needed at the minimum and at the maximum, and how would I judge whether the facilities team is doing a good job?

## 2. The short answer

- Minimum: 1,200 seats. That is 2,000 x 3 = 6,000 seat-days a week, spread perfectly over five days.
- Maximum: 2,000 seats, if everyone comes in on the same days.
- Realistic starting point: about 1,400 to 1,600 seats, opening near 1,500, then tuned using real booking data.

The weekly average never changes, but people cluster midweek, so the busiest day is what sets the seat count. Each country is sized on its own because desks cannot be shared across borders.

## 3. What is in this repo

- case-study.txt: the full written answer (seat calculation, optimization approach, KPIs, how I would present it to management)
- seat-demand-chart.png: seat demand by weekday under three attendance patterns
- seating_calculator.html: a small interactive calculator to test your own numbers

## 4. Try the calculator

Live version: <index.html>

Change the headcount, days in office and midweek attendance, and it shows the fewest, most and needed desks, plus a split by office.

## 5. KPIs I would use

I would judge the team on five groups together, because any single metric can be gamed: space and utilization, employee experience, cost efficiency, service quality, and safety and compliance. The three that matter most are desk utilization with peak occupancy, cost per occupied seat-day, and booking success rate with employee satisfaction.

## 6. Notes

The figures for peak attendance and the KPI targets are illustrative starting points. In a real rollout I would set them after a baseline period using actual WorkInSync booking and badge data.
