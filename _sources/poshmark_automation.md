# Poshmark Automation

[Here ia a Youtube link (11:06 long), with a brief explanation of my code base and a demo of it running](https://www.youtube.com/watch?v=ubEhBm30mq8)


[Here is a link to my GitHub Gist repo to see the code](https://gist.github.com/ChollieDawg/fc9015be63caaca0f82c7f759bbeee65)


My Poshmark Automation project is a comprehensive solution designed to streamline key processes for online sellers on Poshmark. This system uses automation to enhance engagement, track account activity, and simplify listing management, ultimately boosting productivity and brand reach.
Key Features

1. Automated Account Engagement Tracking
The automation script navigates Poshmark’s interface to capture essential engagement metrics:

    Follower Tracking: Records usernames and timestamps of followers, enabling analysis of follower growth.
    Share Monitoring: Logs when other users share your listings and even avoids cross-platform shares, ensuring the focus stays on Poshmark-specific interactions.
    New User Targeting: Identifies and tracks “New Poshers,” providing a list of fresh users who may be more likely to engage back. The system logs interactions with these users in a dedicated database table, helping prioritize engagement opportunities with newcomers.

2. Robust Data Storage and Retrieval
All collected data is systematically stored in an organized SQLite database, making it easy to analyze and retrieve engagement insights:

    Activity Database: Separate tables for different engagement types, with unique record keys for efficient tracking and retrieval of activities over time.
    New Poshers Database: Dedicated to tracking whether you’ve shared an item for each new user, complete with username and share_date fields to manage ongoing interactions.

3. Listing Automation & Cross-Platform Compatibility
One of the core goals of the project is to streamline listing management:

    Automated Listings: Simply drop a folder containing images, descriptions, and tags, and the automation tool prepares the item for listing on Poshmark.
    Cross-Listing Capability: Designed with scalability in mind, the project will support listing items across platforms like Etsy, Instagram, Square, and WordPress, making it a versatile tool for multi-platform sellers.

4. Enhanced Workflow Efficiency
This automation saves valuable time on repetitive tasks, freeing up bandwidth to focus on strategy, customer relations, and inventory management. It ensures that engagement and listings are maintained consistently, enhancing visibility on Poshmark and beyond.
Impact and Future Plans

This project optimizes Poshmark operations by combining efficient data handling, user engagement, and simplified listing management. Moving forward, I plan to expand its cross-platform functionality, enabling seamless listing and activity management across major e-commerce and social media platforms. This work represents a powerful step towards smart, automated e-commerce management tailored to the needs of small business owners and online sellers.




