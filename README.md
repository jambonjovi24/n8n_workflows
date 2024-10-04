# n8n_workflows
# Joke Fetcher Workflow

This repository contains a simple n8n workflow that fetches a random joke from a public API using an HTTP Request node. The workflow is triggered by a Cron node that runs every 5 minutes to get a new joke.

## Workflow Overview

- **Trigger**: Cron (runs every 5 minutes)
- **Action**: HTTP Request to fetch a random joke from [Official Joke API](https://official-joke-api.appspot.com/random_joke).

## Workflow Details

- **HTTP Request Node**:
  - **Method**: GET
  - **URL**: `https://official-joke-api.appspot.com/random_joke`
  
- **Cron Node**:
  - **Interval**: Every 5 minutes

## How to Use

1. **Import Workflow**:
   - Download the `joke-fetcher-workflow.json` file from this repository.
   - In n8n, go to your dashboard and click on the three dots menu.
   - Select **Import** and choose the `joke-fetcher-workflow.json` file to import the workflow.

2. **Test and Execute**:
   - Run the workflow manually or wait for it to run automatically based on the set schedule.

## Requirements

- You need an n8n instance (cloud or locally installed) to import and run the workflow.
- Make sure you have internet access to make the HTTP request to the API.

## License

This project is open-source and available under the MIT License.
