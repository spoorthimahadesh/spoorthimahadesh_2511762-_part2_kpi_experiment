# spoorthimahadesh_2511762-_part2_kpi_experiment
Business Problem Statement

The company recently launched a new onboarding and activation campaign with the goal of helping more users get started with the product and ultimately convert into paying customers. Before rolling out this new experience to all users, leadership needs to determine whether it actually delivers better business outcomes than the existing onboarding process.

This decision affects several teams across the organization. For users, the onboarding experience influences how quickly they understand and engage with the product. For the product and marketing teams, it directly impacts activation and conversion goals. Customer support teams may also be affected if the new experience creates confusion and increases support requests.

The primary objective of this experiment is to improve key business metrics, including onboarding completion, trial starts, user engagement, and paid subscription conversions. However, improving conversion alone is not enough. The company must also ensure that the new onboarding experience does not negatively impact the overall user experience by increasing support tickets or refund requests.

To make an informed recommendation, the experiment results need to provide clear evidence that the treatment group performs better than the control group. This includes measuring the size of the improvement, determining whether the results are statistically significant, and evaluating whether any gains in conversion come with unacceptable business risks. The final recommendation should balance growth opportunities with customer experience and operational impact.
# KPI TREE PNG
<img width="1024" height="768" alt="KPI TREE GRAPH" src="https://github.com/user-attachments/assets/5ad0e246-9a0a-4c5d-9c88-bd15fe8af3b7" />

# TASK 4 Cleaning and Preaparing 

- Missing values were identified in the device_type and traffic source column. Since only a small number of records were affected, these rows were flagged with "UNKNOWN" in the analysis.
- ### Group Counts
The experiment groups were validated to ensure that users were assigned correctly. The dataset contained 670 users in the Control group and 709 users in the Treatment group.
### Duplicate User IDs
User IDs were checked for duplicates to ensure that each user was included only once in the experiment. 9 duplicate user IDs were found.
### Binary Variable Validation
Binary columns were reviewed to confirm that they contained only valid values (0 or 1). No invalid values were identified.



<img width="1111" height="417" alt="image" src="https://github.com/user-attachments/assets/0b9e347b-1542-4c39-819b-a10fe781498e" />


(was not able to upload this in md file)

#Task 8
Guardrail Metrics Evaluation
1. Refund Rate
Group	Refund Rate
Control	0.00%
Treatment	0.42%

The refund rate remained very low in both groups. Although the Treatment group showed a small increase in refunds, the overall rate is minimal and does not currently indicate a significant business risk. However, refund trends should continue to be monitored after rollout to ensure that the increase in conversions is not driven by low-quality subscriptions.

Risk Assessment: Low risk.

2. Support Ticket Rate
Group	Support Ticket Rate
Control	14.72%
Treatment	24.76%

The Treatment group generated a noticeably higher support ticket rate compared to the Control group. This suggests that some users may be experiencing confusion or friction while interacting with the new onboarding experience. An increase in support requests could create additional workload for customer support teams and negatively affect customer satisfaction.

Risk Assessment: Moderate risk. Further investigation is recommended to identify which steps in the onboarding process are causing user issues.

3. Average Engagement Score
Group	Average Engagement Score
Control	57.03
Treatment	62.93

Users in the Treatment group demonstrated higher engagement levels than users in the Control group. This indicates that the new onboarding experience is encouraging users to interact more with the product, which is a positive sign for long-term retention and product adoption.

Risk Assessment: No significant risk identified.

4. Average Days to Convert
Group	Average Days to Convert
Control	8.86 days
Treatment	6.40 days

Users exposed to the new onboarding experience converted faster than users in the Control group. A shorter conversion cycle is generally beneficial because it allows the company to generate revenue sooner. Since refund rates remain low, the faster conversion does not currently appear to be harming customer quality.

Risk Assessment: Low risk.

Overall Guardrail Assessment

The Treatment group delivered higher engagement and faster conversions without causing a meaningful increase in refund rates. However, the increase in support ticket volume represents a potential concern and should be closely monitored during rollout.

Overall, the guardrail metrics do not indicate major risks that would prevent launch, but the onboarding flow should be reviewed and optimized to reduce user confusion and support burden.




