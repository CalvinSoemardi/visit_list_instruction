# visit_list_instruction
How to create visit list or opportunity from cron in Odoo

Visit List/Opportunity Step by Step : 
1. Open Settings -> Scheduled Actions (Technical -> Automation) on Odoo
2. Disable Cron Automation Opportunity Slot
3. Run Cron Create Opportunity
4. Check on database, automation_opportunity_slot, around 50 data should be created with the ‘draft’ state
5. Then after there is no more data created on the database, disable the Cron Create Opportunity
6. Run the Cron Automation Opportunity Slot to update the data that is created before with the state ‘draft’ to state ‘completed’
