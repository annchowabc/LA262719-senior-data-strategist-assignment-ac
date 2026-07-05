# LA262719-senior-data-strategist-assignment-ac
LA262719-senior-data-strategist-assignment-ac
# Senior Data Strategist — Take-Home Submission
Start with `ASSIGNMENT.md`. The sensitivity-label deck (`INFORMATION_PROTECTION.pptx`)
is provided alongside this repository.
# How to run my work
> Replace this section. A reviewer should be able to clone the repo and reproduce
> your output from these instructions alone.

1. Create excel file: the_four_labels.xls from INFORMATION_PROTECTION.pptx. Add new columns as needed, for example, departments that fall into these categories.
2. Create excel file: the_eight_descriptors.xls from INFORMATION_PROTECTION.pptx. Add new columns as need, for example, departments that fall into these categories.
3. Clean up data in file: site_inventory.xls and add columns ac-label, ac-descriptor, copilot-label, copilot-descriptor, chatgpt-label, chatgpt-descriptor.
4. Add my selection to ac-label and ac-descriptor. Add copilot selection to copilot-label and copilot-descriptor.
5. Add chatgpt selection to chatgpt-label and chatgpt-descriptor. This shows that there are various interpretations for label and descriptor.
6. Create Power BI file: LA262719-senior-data-strategist-assignment-ac. Tab: labels-and-descriptors are based on INFORMATION_PROTECTION.pptx. Tab: site_id_scans have draft visualizations of tables: site_inventory, pii_detections, sharing_links.
7. If I had more time, I would determine the risk levels for site-id's based on label and descriptors and create more visuals. 
8. Ask copilot to 'please Propose the auto-labelling rules and the Copilot scoping you would configure for go-live. Ground every choice in the provided deck information_protection powerpoint'. Note copilot's thoughtful response and any actionable insights.
# Assumptions
> List the assumptions you made about the data and the rollout.
1. Assume the data is an initial extract and will have iterations to refine the data extract.
2. Assume the initial rollout could include site-id's where label.risk_level=none. This will give stakeholders a chance to get used to ai-copilot generated information where for example, Public information risk_level=none. 
# What I'd do with more time
> Be specific.
1. Compare my selection of label and descriptors with the current, copilot, and chatgpt selections.
2. Create a workflow of checkpoints to review the ai-generated label and descriptors and make notes as to why a human reviewer would approve or not approve the ai-generated selections. 
