# Hybrid Workplace Seating Optimization
### A Case Study for the Technical Account Manager / Implementation Intern Role at WorkInSync (by MoveInSync)

**Live calculator:** https://utkarsh1454.github.io/workinsync-hybrid-seating-case-study/

## 1. The Business Problem

As the Facility Manager responsible for three offices across three countries, I need to accommodate 2,000 employees who attend the office three days per week.

The challenge is to determine how many desks are required to maintain a reliable employee experience while avoiding unnecessary office space costs. The solution must account for differences in attendance patterns, local office capacity, employee preferences, and peak day demand.

My objective is to balance space utilization, employee satisfaction, and operating costs.

## 2. Seating Capacity: Minimum, Maximum, and Recommended

### Step 1: Calculate Weekly Seat Demand

- Total employees: 2,000
- Office attendance: 3 days per employee per week
- Working days: 5 per week

**Total weekly seat demand**

2,000 × 3 = **6,000 seat days per week**

A seat day represents one desk occupied by one employee for one working day.

### Step 2: Calculate the Theoretical Minimum

If attendance is distributed evenly across five working days:

6,000 ÷ 5 = **1,200 seats**

This is the theoretical minimum, assuming every desk can be shared across different days, attendance is evenly distributed, and desks are available at the required locations.

### Step 3: Calculate the Maximum

If all 2,000 employees attend simultaneously, the organization needs:

**Maximum capacity = 2,000 seats**

This represents the scenario where everyone attends on the same day.

### Step 4: Account for Midweek Peaks

Weekly averages do not capture when employees actually attend. Consider three possible attendance patterns.

| Scenario | Monday | Tuesday | Wednesday | Thursday | Friday | Seats Required |
|---|---:|---:|---:|---:|---:|---:|
| Balanced attendance | 1,200 | 1,200 | 1,200 | 1,200 | 1,200 | 1,200 |
| 70% midweek peak | 900 | 1,400 | 1,400 | 1,400 | 900 | 1,400 |
| 80% midweek peak | 600 | 1,600 | 1,600 | 1,600 | 600 | 1,600 |

All three scenarios produce the same total of 6,000 weekly seat days. However, the busiest day determines the minimum capacity needed to accommodate the attendance pattern.

**Seat demand by weekday under three attendance patterns:** `seat-demand-chart.png`

### My Recommendation

I would use **1,500 seats as an initial planning scenario**, with a provisional range of 1,400 to 1,600 seats.

This is a planning assumption, not a final capacity commitment. The actual requirement must be validated against historical attendance, booking demand, peak day occupancy, and the distribution of employees across the three offices.

The 1,500 seat scenario provides 300 seats above the theoretical minimum of 1,200. However, it would not accommodate a peak of 1,600 employees without additional capacity or changes to attendance schedules.

Each office must be planned independently because desks cannot be shared across countries. I would allocate capacity based on each site's headcount, attendance patterns, local constraints, and peak demand rather than simply dividing the global total by three.

## 3. Interactive Seating Calculator

**[Open the live calculator](https://utkarsh1454.github.io/workinsync-hybrid-seating-case-study/)**

The calculator allows users to change workforce size, office attendance frequency, and midweek attendance assumptions. It estimates weekly seat demand, theoretical minimum capacity, peak day demand, and seating requirements across the three offices.

With the default assumptions of 2,000 employees attending three days per week and a 70% midweek peak, the model illustrates:

- Theoretical minimum: 1,200 seats
- Peak day requirement: 1,400 seats
- Maximum simultaneous requirement: 2,000 seats

The calculator is intended for scenario planning. Actual site level requirements depend on local attendance data and whether the assumed weekday distribution is achievable.

## 4. How I Would Optimize Seating Over Time

I would use a data driven, phased implementation approach.

**Phase 1: Establish the Baseline**

Collect available badge swipe, desk booking, occupancy, and employee location data. Analyze attendance by office and weekday, including peak demand, booking failures, cancellations, and no shows.

**Phase 2: Configure the Workplace Platform**

Work with the implementation team to configure office and floor layouts, desk availability, booking windows, capacity limits, access permissions, and automatic release rules. Validate the configuration against each client's requirements.

**Phase 3: Coordinate Attendance**

Collaborate with team leads to encourage staggered office days where business needs allow. The objective is to reduce avoidable midweek congestion without undermining collaboration or employee flexibility.

**Phase 4: Pilot and Validate**

Pilot the configuration at one or two sites. Compare actual occupancy with predicted demand, collect employee feedback, and resolve configuration or onboarding issues before expanding.

**Phase 5: Monitor and Improve**

Review performance monthly during rollout and quarterly once operations stabilize. Adjust capacity, booking rules, and attendance recommendations based on observed demand, cost, and employee experience.

## 5. KPIs to Evaluate the Facilities Team

I would evaluate performance across five dimensions rather than relying on a single utilization target.

| Dimension | KPI | Measurement | Purpose |
|---|---|---|---|
| Space efficiency | Desk utilization | Occupied desk hours ÷ available desk hours | Identify unused capacity |
| Capacity planning | Peak occupancy | Peak occupied desks ÷ usable desks | Detect overcrowding risk |
| Employee experience | Booking success rate | Successful booking attempts ÷ total valid attempts | Measure access to workplace resources |
| Employee experience | Satisfaction score | Workplace survey results | Assess convenience and comfort |
| Cost efficiency | Cost per occupied seat day | Facilities operating cost ÷ occupied seat days | Track cost relative to actual use |
| Service quality | SLA compliance | Issues resolved within agreed SLA ÷ issues resolved | Assess responsiveness |
| Operational readiness | Workplace readiness | Required workstations ready ÷ workstations required | Verify desks and essential services are available |
| Governance | Safety and compliance | Audit findings, incidents, and corrective action closure | Maintain a safe and compliant workplace |

### The Three KPIs I Would Prioritize

**1. Desk Utilization and Peak Occupancy**

These show whether the organization is using its space efficiently and whether the busiest days create capacity constraints. I would monitor them separately for each office and weekday.

**2. Cost per Occupied Seat Day**

This connects facilities expenditure with actual usage. It helps identify opportunities to optimize office space without confusing lower costs with better service.

**3. Booking Success Rate and Employee Satisfaction**

These protect the employee experience. High utilization is not a success if employees cannot find a desk, suitable facilities are unavailable, or workplace issues remain unresolved.

I would establish baseline performance before setting targets. For example, a booking success target above 98% could be proposed for discussion and finalized after reviewing the platform's measurement method and operational requirements. Safety, accessibility, and service standards would remain non negotiable.

## 6. What Is Included in This Repository?

| File | Purpose |
|---|---|
| `case-study.txt` | Written analysis, calculations, optimization plan, and KPIs |
| `seat-demand-chart.png` | Visual comparison of balanced, 70%, and 80% midweek attendance |
| `index.html` | Interactive seating capacity calculator hosted on GitHub Pages |
| `README.md` | Project overview, assumptions, methodology, and usage instructions |

## 7. Assumptions and Limitations

The attendance distributions, capacity recommendation, and proposed KPI targets are illustrative. They are not actual WorkInSync customer data or established company benchmarks.

The theoretical minimum assumes attendance can be distributed evenly across the working week. In practice, capacity depends on peak attendance, office specific headcount, employee access restrictions, and the ability to coordinate schedules.

The 1,500 seat recommendation should therefore be treated as a planning scenario to validate, not a guaranteed optimal solution.

## 8. Management Summary

The organization generates 6,000 seat days of weekly demand. Although this equates to a theoretical minimum of 1,200 seats, midweek attendance peaks can increase the required capacity to 1,400 or 1,600 seats. The maximum simultaneous requirement is 2,000 seats.

I would begin with a provisional 1,500 seat planning scenario, validate demand separately across all three offices, and use workplace booking and occupancy data to refine the allocation.

Success would be measured through space utilization, peak occupancy, cost per occupied seat day, booking reliability, employee satisfaction, service quality, and safety compliance.

**The objective is not simply to minimize the number of desks. It is to provide the right capacity, at the right location, on the right day, while delivering a reliable employee experience at an efficient cost.**
