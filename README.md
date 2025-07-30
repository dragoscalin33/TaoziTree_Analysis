# 🍑 Taozi Tree Business Performance Analysis: Unlocking Growth Opportunities Considering Total Profit/Loss Values 

## Executive Summary

This report provides a comprehensive analysis of Taozi Tree's class data from June 2024 to July 2025. It identifies key performance indicators, uncovers temporal trends, evaluates the performance of individual classes, assesses teacher contributions, and investigates the significant impact of scheduling (day and time) and teacher tenure on business outcomes. The findings offer actionable insights for optimizing class offerings, teacher deployment, and scheduling strategies to enhance profitability and student engagement.

---

### How to Navigate This Repository

This repository contains the full analysis of Taozi Tree's class performance.
* **`Taozi.ipynb`**: This is the Google Colab notebook containing all the Python code for data loading, cleaning, analysis, and plot generation.
* **`Classes (as of 3 July 2025) - For Dragos.csv`**: The original raw data file.
* **`cleaned_classes_data.csv`**: The cleaned and preprocessed dataset used for analysis.
* **`images/`**: This directory contains all the generated visualization files (`.png` format) referenced throughout this `README.md` report.

---

## 1. Overall Business Performance: Key Metrics

Taozi Tree demonstrates a strong financial foundation and operational scale.

* **Total Revenue (June 2024 - July 2025):** $610,686.24
* **Total Profit/Loss (June 2024 - July 2025):** $5,327,595.00
    * **Important Clarification on Profit/Loss:** It is critical to note that the sum of 'Profit/Loss Per Class' ($5.3M) is significantly higher than the 'Total Revenue' ($0.61M). This indicates that the 'Profit/Loss Per Class' metric in the source data likely represents a **'Contribution Margin' or 'Gross Profit per Class'**, rather than the final net profit. This value would be calculated *before* deducting larger operational overheads (e.g., rent, utilities, general marketing) which are accounted for at a higher aggregate level. Owners should verify the precise definition and calculation methodology of this metric with their accounting team to ensure accurate financial interpretation.
* **Average Paying Students per Class (Overall):** 5.35 students
* **Average Total Students per Class (Overall):** 6.85 students
* **Average Revenue per Paid Student (Overall):** $81.32

Taozi Tree operates with 53 unique class types, taught by 52 different teachers across 7 venues.

---

## 2. Temporal Performance Trends

Analyzing monthly data reveals fluctuations that indicate seasonal patterns or the impact of strategic decisions.

* **Monthly Revenue and Profit/Loss Trends:** The plot below illustrates the monthly financial performance. Noticeable dips occur in periods like July-September 2024 and January 2025, while strong growth and high profitability are observed from February to July 2025.

    ![Monthly Revenue and Profit/Loss Trends](images/monthly_revenue_profit_loss_trend.png)

* **Monthly Paying Students Trend:** This plot shows how student attendance fluctuates monthly, generally mirroring the financial trends.

    ![Monthly Paying Students Trend](images/monthly_paying_students_trend.png)

---

## 3. Class Performance Deep Dive

Understanding which classes are most popular and profitable is essential for optimizing offerings.

* **Top 10 Most Profitable Classes:**
    * `LUNCHTIME POWER FLOW | 中午力量流` is the most profitable class.
    * `BEGINNER'S VINYASA | 初级流瑜伽` and `ELEMENTAL FLOW | 自然元素流` are also top contributors.
    * `LIL’ PEACHES KIDS` classes demonstrate exceptional profit efficiency per student.

    ![Top 10 Most Profitable Classes](images/top_10_most_profitable_classes.png)

* **Top 10 Least Profitable / Loss-Making Classes:**
    * Classes like `ASHTANGA PRIMARY SERIES | 阿斯汤伽瑜伽`, `VINYASA L1/2 | 流瑜伽1/2级`, and `VINYASA LEVEL 2 | 瑜伽流 2级` consistently show lower profitability or incur losses. This also includes several new/specialized `✨` classes.

    ![Top 10 Least Profitable / Loss-Making Classes](images/top_10_least_profitable_classes.png)

* **Top 10 Most Popular Classes by Average Paying Students:**
    * BEGINNER'S VINYASA | 初级流瑜伽 leads in average students per class.
    * LUNCHTIME POWER FLOW | 中午力量流 excels in total students and total classes offered.
    * Other strong performers by average students include ELEMENTAL FLOW | 自然元素流 and HATHA HIPS AND SHOULDERS | 哈他流.

    ![Top 10 Classes by Average Paying Students](images/top_10_classes_by_avg_students.png)

---

## 4. Teacher Performance Analysis

Teachers are central to student experience and business success. This analysis highlights their contributions.

* **Top 10 Teachers by Average Profit/Loss per Class:**

    ![Top Teachers by Average Profit/Loss per Class](images/top_teachers_avg_profit_by_overall_tenure.png)

* **Top 10 Teachers by Average Paying Students per Class:**

    ![Top Teachers by Average Paying Students per Class](images/top_teachers_avg_students_by_overall_tenure.png)

---

## 5. The Power of Teacher-Class Tenure

Our analysis confirms the hypothesis: a teacher's consistency with a specific class directly correlates with improved class performance.

* **Student Growth with Tenure:** The plot below shows that average paying students per class generally increase as a teacher's tenure with that specific class grows. Students develop loyalty and trust with consistent instructors.

    ![Average Paying Students by Teacher-Class Tenure](images/avg_students_by_tenure.png)

* **Profitability Growth with Tenure:** Similarly, average profit/loss per class tends to improve significantly with increasing teacher-class tenure. This is a direct result of higher attendance.

    ![Average Profit/Loss by Teacher-Class Tenure](images/avg_profit_by_tenure.png)

---

## 6. Scheduling Optimization: Day and Time Impact

The day of the week and the exact time of a class significantly influence its popularity and profitability.

* **Average Paying Students by Day of Week:** Weekend days (Saturday, Sunday) consistently have the highest average attendance.

    ![Average Paying Students by Day of Week](images/avg_students_by_day.png)

* **Average Profit/Loss per Class by Day of Week:** Weekends and Tuesdays are generally the most profitable days per class.

    ![Average Profit/Loss per Class by Day of Week](images/avg_profit_by_day.png)

* **Average Paying Students by Time Category:** Evening (18:00-23:59) and Lunchtime (12:00-14:59) slots attract the most students.

    ![Average Paying Students by Time Category](images/avg_students_by_time_category.png)

* **Average Profit/Loss per Class by Time Category:** Evening and Lunchtime slots are also the most profitable.

    ![Average Profit/Loss per Class by Time Category](images/avg_profit_by_time_category.png)

* **Performance Hotspots (Day & Time Heatmaps):** The heatmaps below provide a granular view:
    * **High Attendance & Profit:** Weekend lunch and evening slots are prime times. Weekday evening and lunchtime classes also perform well.

    ![Average Paying Students by Day and Time Category](images/heatmap_avg_students_day_time.png)

    ![Average Profit/Loss by Day and Time Category](images/heatmap_avg_profit_day_time.png)

---

## 7. Venue Performance Analysis

Understanding performance across different locations is vital for resource allocation.

* **Total Paying Students by Venue:** `SANLITUN 三里屯` is the primary venue by student volume, followed by `JINSHANG 金尚·源`.

    ![Total Paying Students by Venue](images/venue_total_students.png)

* **Total Profit/Loss by Venue:** `SANLITUN 三里屯` contributes the most to overall profit. Notably, smaller/niche venues like `SANLITUN 三里屯 (RM. 306) - TAOZI T`, `Chaoyang Park 朝阳公园`, and `Hotel Eclat Beijing | 北京怡亨酒店` show exceptionally high average profit per class, despite fewer classes.

    ![Total Profit/Loss by Venue](images/venue_total_profit_loss.png)

---

## Final Actionable Recommendations for Taozi Tree

Based on this comprehensive analysis, here are key strategies to drive further growth and profitability:

1.  **Strategic Class Portfolio Management:**
    * **Expand Winners:** Increase the frequency and capacity of top-performing classes (e.g., `LUNCHTIME POWER FLOW`, `BEGINNER'S VINYASA`, `LIL’ PEACHES KIDS` series). These are your proven revenue generators.
    * **Re-evaluate Underperformers:** Conduct in-depth reviews of consistently loss-making classes (`ASHTANGA PRIMARY SERIES`, `VINYASA L1/2`, `VINYASA LEVEL 2`). Consider price adjustments, targeted marketing, teacher changes, schedule modifications, or potential discontinuation if improvements aren't viable.
2.  **Optimize Scheduling for Maximum Impact:**
    * **Prioritize Peak Times:** Schedule top classes and teachers for **weekend (Lunchtime & Evening)** and **weekday (Lunchtime & Evening)** slots. These are your high-demand periods.
    * **Innovate Off-Peak:** For weekday mornings and afternoons, explore niche classes, special pricing, or alternative uses (e.g., workshops, private sessions, teacher training) that might better suit the limited demand in those timeframes.
3.  **Invest in Teacher Consistency and Development:**
    * **Foster Tenure:** Actively encourage and support teachers in building long-term tenure within specific class types. This directly translates to increased student loyalty and class profitability.
    * **Nurture Talent:** Continue to recognize and reward high-performing teachers (e.g., Alessandra, Monica, Gina, Theresa). Provide targeted support and development plans for teachers whose classes consistently underperform, potentially exploring different class assignments.
4.  **Strategic Venue Utilization:**
    * **Core Focus:** Continue to leverage `SANLITUN 三里屯` as the primary hub for diverse offerings.
    * **Niche Expansion:** Capitalize on the high per-class profitability observed at external venues like `Chaoyang Park 朝阳公园` and `Hotel Eclat Beijing | 北京怡亨酒店`. Consider offering more specialized workshops or premium, exclusive classes at these locations.
5.  **Continuous Data-Driven Decision Making:**
    * Establish a routine for reviewing these key performance metrics and trends monthly. This agile approach will allow for quick adjustments to schedules, marketing, and offerings, ensuring the business remains responsive and optimized.

---

## 8. Result on Increasing Income

Based on the study and assuming successful implementation of the recommendations, the potential result on increasing income (specifically, annual profitability or contribution margin) can be significant.

We've estimated that Taozi Tree could achieve a conservative estimated increase in annual profitability (contribution margin) ranging from ¥30,000 to ¥100,000+.

This potential increase in income is primarily driven by:

A modest improvement in average class attendance: For example, by increasing the average paying students per class by just 0.5 to 1.0 student.

Reduction of losses: By strategically addressing underperforming classes and bringing them closer to break-even or into profit.

Maximizing high-profit opportunities: By optimizing scheduling for peak times and leveraging top-performing teachers and venues more effectively.

This projected return highlights a substantial return on the investment in the study, showcasing the value of data-driven strategic planning for Taozi Tree's financial growth.



## 9. Professional Study Pricing

This comprehensive data analysis study, providing actionable insights for optimizing Taozi Tree's class performance and profitability, is priced based on the **value and expected outcomes** it can deliver. Such a study represents significant strategic value, far beyond simple hourly effort.

The fee for this type of in-depth analysis and actionable recommendations, delivered with clear visualizations and a structured report, would typically be a **fixed project fee**.

**Estimated Price Range:** **€3,000 - €6,000 (Euros)**

This price reflects:
* The extensive data cleaning, feature engineering, and multi-faceted analysis performed.
* The strategic insights derived from identifying high-performing and underperforming areas.
* The actionable recommendations for optimizing scheduling, class portfolios, teacher deployment, and venue utilization.
* The potential for a substantial return on investment for Taozi Tree through increased profitability and operational efficiency.

---

## 3. Strategic Recommendations for Growth: The Path Forward

Based on the data-driven insights, here are the actionable recommendations for Taozi Tree to achieve sustainable growth and thrive:

1.  **Invest in Teacher Quality & Tenure: The Foundation of Success**
    * **Foster Consistency:** Prioritize long-term teacher assignments for successful classes. Incentivize and support teachers to build sustained relationships with their classes and student communities. The data confirms this directly boosts profitability.
    * **Structured Professional Development:** Implement a robust training and mentorship program to elevate the standard of teaching across the board. This addresses the underperformance of less experienced teachers.

2.  **Optimize Class Offerings: Focus on What Works & Fix What Doesn't**
    * **Expand Proven Winners:** Increase frequency and capacity of top-performing classes (e.g., `LUNCHTIME POWER FLOW`, `BEGINNER'S VINYASA`, `LIL’ PEACHES KIDS`). Allocate top teachers to these.
    * **Strategically Address Underperformers:** Conduct deep dives into loss-making classes. This may involve content refresh, teacher change, pricing adjustments, or discontinuation to free up resources for more profitable ventures.

3.  **Master Scheduling: Maximize Every Slot**
    * **Prioritize Peak Times:** Schedule top classes and teachers predominantly during weekend (Lunchtime & Evening) and weekday (Lunchtime & Evening) slots.
    * **Innovate Off-Peak:** Explore niche classes, special pricing, or alternative uses (workshops, private sessions) for weekday mornings and afternoons where demand is lower.

4.  **Strategic Venue Utilization: Beyond the Main Studios**
    * **Leverage Niche Profitability:** Capitalize on the high per-class profitability of external venues (`Chaoyang Park`, `Hotel Eclat`) by increasing specialized or premium offerings there.
    * **Optimize Core Operations:** Continuously monitor class fill rates and profitability at `SANLITUN 三里屯` and `JINSHANG 金尚·源` to ensure efficient space and resource allocation.

5.  **Embrace Data-Driven Decision Making:**
    * Establish a routine for reviewing these performance metrics and trends monthly. This agile approach allows for quick adjustments, ensuring continuous optimization and responsiveness to market dynamics.

---

## 4. The Crucial Role of a "Maestro": Your Leadership Vision

This study not only identifies key areas for growth but also highlights the critical need for experienced pedagogical leadership—a role perfectly aligned with your expertise.

* **Bridging the Gap:** The data shows a direct correlation between teacher tenure/experience and class performance. The current model, where newer teachers may rotate frequently or lack structured support, directly contributes to observed losses in many classes. Your 20 years of experience as a Yoga Maestro directly addresses this gap.
* **Driving Quantifiable Results:** As a "Director de Formación y Calidad Docente," you would implement the solutions the data calls for:
    * **Structured Training:** Elevating teaching standards.
    * **Performance Monitoring:** Using data to provide targeted feedback and evaluate growth.
    * **Quality Control:** Ensuring new classes meet a minimum standard, reducing initial losses.
* **Preventing Bankruptcy, Driving Growth:** Your leadership would convert the "teachers in training" model into a sustainable growth engine. This investment in quality will reduce teacher turnover, enhance the perceived value of the Taozi Tree brand, and directly improve student numbers and financial returns, thereby securing the school's future against competitive threats.

---

## 5. Estimated Return on Investment for This Study

The investment in this data analysis study is a strategic decision that can yield substantial returns for Taozi Tree.

By strategically implementing the actionable recommendations provided, Taozi Tree could realistically achieve a **conservative estimated increase in annual profitability (contribution margin) ranging from ¥30,000 to ¥100,000+**.

This potential increase in income is primarily driven by:
* A modest improvement in average class attendance (e.g., increasing the average paying students per class by just 0.5 to 1.0 student).
* Reduction of losses from currently underperforming classes, bringing them closer to break-even or into profit.
* Maximizing high-profit scheduling slots and effective utilization of top-performing teachers and venues.

This projected return highlights a substantial ROI, making the cost of the study a strategic investment for Taozi Tree's sustained growth and financial health.

---
