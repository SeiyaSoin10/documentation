---
sidebar_label : Insights KPIs
title: Insights KPIs
---

:::note
All the mentioned KPIs are not readily available in form of widgets/tables.
:::

| **Metric**                             | **Description**                                                                                                                                                              | **Calculation/Logic**                                                                                                                                                                                            | **Use Cases**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|----------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Users**                              | Shows the unique number of users who conversed with the bot.                                                                                                                | Unique count of users from the list of messages exchanged on the bot, calculated using the [hyperloglog](https://en.wikipedia.org/wiki/HyperLogLog) algorithm.                                                   | - Measure the bot's reach and popularity through unique user count. <br/> - Monitor changes in user count to track bot adoption and growth.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **User Traffic**                       | Displays the total number of messages exchanged, categorized into messages between bot and users, and messages between live agents and users.                                | Sum of all messages exchanged, including user, bot, agent, and notification messages.                                                                                                                             | - Gain insights into communication volume and patterns between users, the bot, and live agents. <br/> - Track engagement and interaction levels to improve communication channels.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Sessions**                           | Provides an overview of user sessions, including the total number of sessions and their types (Bot-only sessions vs. Sessions with both bot and live agent).                 | Sum of all sessions created by the user in the selected period.                                                                                                                                                   | - Get an overview of user sessions, including bot-only sessions and sessions with both bot and live agent. <br/> - Monitor user engagement patterns and balance between bot and live agent interactions.                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Session Traffic**                    | Displays average time spent by users conversing with the bot. A session can last up to 24 hours, after which a new session starts.                                            | Average of the total time users conversed with the bot divided by the total number of sessions. This metric is captured for all sources.                                                                          | - Analyze average session duration to understand user engagement and satisfaction levels. <br/> - Use session duration as a metric to assess and improve the bot's effectiveness over time.                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Traffic Channels**                   | Frequency of unique users messaging the bot, categorized by source (traffic channel) and aggregated daily for the chosen date range.                                         |                                                                                                                                                                                                                  | - **User acquisition analysis**: Assess the effectiveness of traffic channels in acquiring new users. <br/> - **Channel performance evaluation**: Evaluate the performance of different channels based on daily user frequency.                                                                                                                                                                                                                                                                                                                                                                                                |
| **Platform/Medium**                    | Frequency of unique users messaging the bot, categorized by device origin, aggregated daily. Note: This data is only available for Yellow Web & Mobile, not for WhatsApp/Facebook. |                                                                                                                                                                                                                  | - **Platform/Medium analysis**: Analyze user frequency based on device or platform to tailor bot features and optimize user experience. <br/> - **Platform/Medium comparison**: Compare user engagement across platforms to inform resource allocation and marketing strategies.                                                                                                                                                                                                                                                                                                                                               |
| **Unique Users by Country**            | Shows the count of unique users conversing with the bot from various countries, highlighting the top 5 countries and their percentage contributions.                        | Calculated by capturing the IP address of the user and translating it to a standard location using the ip2location database.                                                                                      | - **Geographical user analysis**: Understand user distribution across countries to inform regional strategies. <br/> - **Localization and targeting**: Tailor content and features based on the unique users by country data.                                                                                                                                                                                                                                                                                                                                                                                                |
| **User Activity by Time**              | Displays user frequency over a specific period, organized by day and time. Useful for analyzing when user activity peaks and dips.                                           | Calculated by aggregating the number of unique users who interacted with the bot within each hourly interval for the selected period.                                                                             | - **Resource allocation**: Identify peak user activity hours to allocate resources effectively and ensure prompt responses to user inquiries. <br/> - **Scheduled maintenance**: Determine low-activity hours to schedule maintenance, minimizing service disruption. <br/> - **Marketing campaigns**: Identify optimal hours with high user engagement and conversion rates for launching targeted marketing campaigns.                                                                                                                                                                                                                                 |
| **Users by Device**                    | Shows the different types of user devices from which the bot was accessed.                                                                                                   | Frequency of unique users conversing with the bot, segregated by device and aggregated for the selected date range.                                                                                               | - **Device usage analysis**: Analyze user distribution across different devices for optimization. <br/> - **Device-specific optimization**: Optimize user experience based on device-specific data.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Bot Accuracy**                       | Shows the percentage of user messages identified by the bot with a certain level of confidence.                                                                              | Bot accuracy = `[1 - (Unidentified user messages / Total User Messages)]*100`                                                                                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Flow Completion Rate**               | Measures how many customer intents are fulfilled by the bot for every 100 intents started by users.                                                                           | Flow completion rate = `[(Flow Completed Events) / (Flow Started Events)]* 100`                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Deflection Rate**                    | Percentage of queries resolved by the bot without transferring the chat to a live agent, indicating self-service efficiency.                                                  | Deflection rate = `(Bot sessions without agent handover / Total sessions) * 100`                                                                                                                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **CSAT**                               | Customer satisfaction score given by users for both bot and agent sessions, rated on a scale of 0 to 5. The graph compares user feedback on bot sessions vs. agent sessions. |                                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Top Flows Visited**                  | Shows the most frequently triggered flows by users and the average time taken to complete these flows.                                                                         | Count of completed events for each flow, along with the average time users spent within the flow.                                                                                                                                                                                                                   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Business-Initiated Conversations**   | Conversations initiated by the bot or business to provide information, send notifications, or engage with users based on predefined triggers or events.                      |                                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **User-Initiated Conversations**       | Conversations initiated by users who send messages or queries to the bot, seeking information or assistance.                                                                  |                                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Referral-Initiated**                 | Conversations that occur when users refer the bot to others, allowing the bot to initiate personalized conversations with those referred contacts.                           |                                                                                                                                                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |