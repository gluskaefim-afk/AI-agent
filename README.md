# Inventory & OTD Monitoring AI Agent

💻Overview:
This project is an automated AI-powered agent built in n8n that monitors inventory levels and delivery performance metrics using data from Microsoft Excel and interacts with users via Telegram.
The agent supports both on-demand checks via Telegram commands and scheduled automated checks, producing clean, action-oriented outputs without manual intervention.

# 📲Core Functions:
The main function of this AI agent is to monitor warehouse inventory and automatically generate daily operational reports.
Every morning at 10:00, the agent checks current warehouse stock levels and sends a report with the required replenishment quantity for each SKU that requires action.
At the same time, the agent performs a daily On-Time Delivery (OTD) check at 10:00, calculates the current OTD percentage, compares it with the previous period, and reports the percentage point change.
The agent operates both on a scheduled basis and via manual commands, providing continuous visibility into inventory status and delivery performance without manual intervention.


# ❗ The repository provides an example dataset used by the AI agent.
In a real production environment, the dataset is more complex, and OTD and stock levels are calculated dynamically within the Excel file as new orders are added.
The AI agent reads the latest computed values directly from the file, ensuring that all reports are based on up-to-date operational data without performing raw calculations externally.
