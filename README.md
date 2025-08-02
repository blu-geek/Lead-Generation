# Lead Generation

<img width="592" height="614" alt="Screenshot 2025-08-01 at 18 04 49" src="https://github.com/user-attachments/assets/e88995a0-e732-4ea2-98e8-b1c483243433" />

# Overview

This cutting-edge n8n workflow is a powerful automation tool designed to revolutionize how businesses and marketers identify and qualify leads directly from YouTube video comments. By leveraging specialized Apify Actors and an intelligent AI agent, this workflow seamlessly transforms raw comment data into comprehensive lead profiles, saving valuable time and resources.

This workflow automatically:

# Discovers & Scrapes Comments:

Monitors a Google Sheet for new YouTube video URLs.
Automatically extracts all comments from specified YouTube videos using a dedicated Apify Actor.
Marks videos as "scrapped" to avoid reprocessing.
Intelligent Lead Enrichment:

# Retrieves unprocessed comments from Google Sheets.
Activates an advanced AI agent (powered by OpenRouter's cutting-edge models) to research comment authors.
Utilizes Google Search (via Serper API) and specialized Apify scrapers (for website content and Instagram profiles) to find publicly available information like social media links, bios, and potential contact details.
Generates concise descriptions for each lead based on gathered data.

# Organized Data Storage:

Creates new entries in a dedicated Google Sheet for each new lead.
Updates lead profiles with all discovered enriched data (email, social media, short bio, etc.).
Marks comments as "processed" once their authors have been researched and enriched.
Key Benefits

🤖 Full Automation: Eliminates manual data collection and research, freeing up your team for strategic tasks.
💡 Smart Lead Enrichment: AI intelligently sifts through information to build rich, actionable lead profiles.
⏱️ Time-Saving: Instant, scalable lead generation without human intervention.
📈 Enhanced Lead Quality: Go beyond basic contact info with comprehensive social and professional context.
📊 Centralized Data: All leads are neatly organized in Google Sheets for easy access and integration.

# Setup Requirements

n8n Installation:
Install n8n (cloud or self-hosted).
Import the workflow configuration.
Configure API credentials.
Set up scheduling preferences for continuous operation.
Google Sheets Credentials:
A Google Cloud API key with access to Google Sheets.
Set up OAuth2 authentication in n8n for read/write access to your "youtube leads" spreadsheet (containing "videos", "comments", and "leads" sheets).
OpenRouter API Access:
Create an OpenRouter account.
Generate an API key to access their chat models (e.g., google/gemini-2.5-flash-preview-05-20) for AI agent operations.
Apify API Access:
Create an Apify account.
Generate a personal API token to run Apify actors for: This token is used to run the following Apify Actors:
for comment extraction, website content extraction, and Instagram profile details
Serper API Key:
Sign up for an account on Serper.dev.
Obtain an API key for performing Google searches to find social media profiles and other information.

# Potential Use Cases

- Content Creators: Identify highly engaged audience members for community building or direct outreach.
Marketing Teams: Discover potential customers or influencers interacting with competitor content.
Sales Professionals: Build targeted lead lists based on specific interests expressed in comments.
Market Researchers: Analyze audience demographics and interests by enriching profiles of commenters on relevant videos.
Recruiters: Find potential candidates based on their expertise or engagement in industry-specific discussions.
Future Enhancement Roadmap

- CRM Integration: Directly push enriched leads into popular CRM systems (e.g., HubSpot, Salesforce).
Automated Outreach: Implement automated email or social media messaging for qualified leads.
Sentiment Analysis: Analyze comment sentiment before enrichment to prioritize positive interactions.
Multi-Platform Support: Expand comment extraction and lead enrichment to other platforms (e.g., TikTok, Facebook).
Advanced Lead Scoring: Develop a scoring model based on engagement, profile completeness, and relevance.
Ethical Considerations

# Data Privacy: Ensure all collected data is publicly available and used in compliance with relevant privacy regulations (e.g., GDPR, CCPA).
# Platform Guidelines: Adhere strictly to YouTube's Terms of Service and Apify's usage policies.
# Transparency: If engaging with leads, be transparent about how their information was obtained (if applicable).
No Spam: This tool is designed for lead identification, not for unsolicited mass messaging.
Technical Requirements

n8n v1.0.0 or higher (recommended for latest features and stability)
Google Sheets API access
OpenRouter API access
Apify API access
Serper API access
Stable internet connection
