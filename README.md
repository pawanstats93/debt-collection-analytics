# 📊 Debt Collection Analytics Project (US Collections)

## 🔍 Project Overview

This project simulates a real-world **US Debt Collection Analytics system** using a dataset of 50,000 customer accounts. The goal is to analyze delinquent accounts, improve recovery strategies, and design data-driven collection workflows.

---

## 🎯 Objectives

* Analyze delinquency trends (30/60/90+ days)
* Identify high-risk accounts for early intervention
* Track Promise-to-Pay (PTP) behavior
* Measure recovery performance
* Evaluate collector efficiency
* Design CRM-style collection workflows
* Ensure basic compliance awareness (FDCPA)

---

## 🛠️ Tools Used

* SQL (SSMS)
* Excel / Power BI (for dashboard)
* GitHub (project documentation)

---

## 📂 Dataset

* 50,000 simulated US customer debt accounts
* Includes:

  * Debt amount, payments
  * Delinquency days & buckets
  * Collector details
  * Contact attempts
  * Promise-to-Pay (PTP)

---

## 📊 Key Analysis Performed

### 1. Delinquency Analysis (DELINQUENCY BUCKET ANALYSIS (PRIORITIZATION STRATEGY))

Segmented accounts into buckets (0–30, 31–60, 61–90, 90+) to prioritize collections.

### 2. Risk Identification (Very HIGH-RISK ACCOUNT IDENTIFICATION)

Identified high-risk accounts based on delinquency and outstanding balance.

### 3. Recovery Metrics

Calculated overall and bucket-wise recovery rates to evaluate performance.

### 4. Delinquency Bucket-wise Recovery Rate

Compare recovery efficiency across delinquency buckets. Helps understand when recovery is most effective.

### 5. PTP (PROMISE TO PAY) Analysis

Evaluate how effective customer commitments (PTP) are.

### 6. Collector Performance Analysis

Evaluate performance of collection agents.

### 7. Aging Report

Show distribution of outstanding debt across time buckets. Core report used in collections industry.

### 8. Collection Workflow

COLLECTION WORKFLOW (REAL BUSINESS SIMULATION)
Simulate real-world collection action strategy. 

### 9. Payment Negotiation Simulation

Suggested settlement strategies based on risk and delinquency.

### 10. Compliance Awareness (FDCPA)

Maintain structured tracking for audit & compliance

## 📈 Key Insights

### 1. Delinquency Analysis (DELINQUENCY BUCKET ANALYSIS (PRIORITIZATION STRATEGY))

-> 90+ days delinquency is the biggest risk pool, holding the highest outstanding debt (~$132M), making it the top priority for recovery efforts.

-> Early-stage buckets (0–90 days) collectively hold significant debt (~$120M+), indicating strong opportunity for preventive collections before accounts worsen.

-> Account volume is heavily skewed toward 90+ days (25K vs ~8K), suggesting accounts are aging without timely intervention.

-> Average debt per customer is nearly identical (~$5.2K across all buckets), meaning delinquency timing—not loan size—drives risk.

-> Operational gap identified: High concentration in 90+ days implies inefficiencies in early collection strategies, highlighting the need for faster follow-ups and proactive outreach.

### 2. Risk Identification (Very HIGH-RISK ACCOUNT IDENTIFICATION)

-> Focus is on actionable risk (60+ days overdue):

The query filters only accounts with delinquency > 60 days, ensuring analysis targets customers who already require active collection intervention, not just monitoring.

-> Clear risk segmentation enables prioritization:

Accounts are categorized into Medium (61–90), High (91–120), and Critical (120+), helping teams align strategies based on urgency.

-> Highest financial impact is prioritized first:

Sorting by debt_amount (descending) ensures collectors focus on high-value defaulters first, maximizing recovery efficiency.

-> Critical Risk accounts represent immediate escalation cases:

Customers with 120+ days delinquency should be flagged for legal action, settlements, or external agencies, as recovery probability declines sharply.

-> Combination of risk + value supports smarter allocation:

By combining delinquency severity + outstanding balance, the query helps identify “high-risk, high-value” accounts, which are the most important segment for business impact.

### 3. Recovery Metrics

-> Overall recovery rate is ~30.1%, meaning the business is recovering only about one-third of total outstanding debt, indicating significant room for improvement.

-> High revenue leakage (~70%) remains uncollected, with ~$18.6M still outstanding, representing a major financial risk and lost opportunity.

-> Collection efficiency is relatively low, suggesting potential gaps in timing, prioritization, or collection strategies (e.g., late intervention or weak follow-ups).

Strong need for early-stage intervention:

-> Improving recovery in 0–60 day delinquency buckets could significantly boost this KPI, as recovery probability declines with time.

This KPI should be segmented for deeper insights:

-> The 30% average may hide performance differences—breaking it down by risk level, delinquency bucket, or region can reveal where collections are failing or succeeding.

### 4. Delinquency Bucket-wise Recovery Rate

-> Recovery rates are nearly identical (~30%) across all buckets → Indicates no strong advantage of early vs late collections, which is unusual.

-> 61–90 days shows the highest recovery (~30.55%) → Suggests this is the most responsive stage for collections.

-> 0–30 days has the lowest recovery (~29.66%) → Highlights inefficiency in early intervention, where recovery should be easiest.

-> 90+ bucket drives the highest total recovery (~$39.6M) → Due to large account volume, making it critical despite slightly lower efficiency.

-> Lack of recovery drop in late stages → Implies either strong late recovery efforts or weak early-stage strategy, needing optimization.

### 5. PTP (PROMISE TO PAY) Analysis

-> PTP effectiveness can be directly measured → “PTP Kept” shows successful commitments, helping evaluate how reliable customer promises are as a recovery strategy.

-> Broken and delayed PTPs indicate collection risk → High “PTP Broken/Delayed” suggests low customer reliability, requiring stricter follow-ups or alternative strategies.

-> “No PTP” segment highlights engagement gaps → Accounts without PTP indicate lack of customer interaction, signaling need for improved outreach and negotiation efforts.

### 6. Collector Performance Analysis

-> Top collectors handle more accounts and recover higher amounts, showing strong performance and capacity.

-> Total collected varies widely, highlighting differences in collector effectiveness and efficiency.

-> Average calls made per collector reveal effort levels, useful for linking activity to recovery success.

### 7. Aging Report

-> High delinquency risk: ~50% accounts & largest debt in 90+ bucket

-> Capital stuck in late stage: Majority outstanding in 90+ → difficult recovery

-> Inefficient recovery pattern: ~30% recovery across all buckets (no improvement)

### 8. Collection Workflow

-> All accounts in critical stage: Delinquency = 180 days → all fall into “Immediate Call + Escalation”

-> High recovery urgency: These are severely overdue accounts requiring aggressive action (calls, legal, escalation)

-> Operational focus needed: Team should prioritize top debt amounts first within this bucket to maximize recovery

### 9. Payment Negotiation Simulation

-> Remaining balance visibility: Shows exact unpaid amount → helps prioritize high-value recoveries

-> Dynamic settlement strategy: Higher delinquency → bigger discount (30% for 90+) to improve recovery chances

-> Business impact: Balances loss vs recovery → better to recover partial amount than risk full default

### 10. Compliance Awareness (FDCPA)

-> Compliance risk identified: Accounts with >5 contact attempts flagged “Review Required” → potential regulatory violation

-> Majority need review: Many records exceed limit → indicates over-aggressive collection approach

-> Action needed: Optimize contact strategy (limit frequency, smarter outreach) to ensure ethical & compliant collections

## 📬 Author

**Pawan Sharma**

* LinkedIn: (https://www.linkedin.com/in/pawan-sharma-6bb178132/)
* GitHub: (https://github.com/pawanstats93)
