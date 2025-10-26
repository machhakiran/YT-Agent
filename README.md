---
title: YT Agent
emoji: 🤖
sdk: docker
app_port: 8501
tags:
  - streamlit
license: apache-2.0
short_description: Example Space for running YT agent AI app.
---
# yt-agent-streamlit
Example code for creating a YouTube agent with Streamlit and hosting via Hugging Face Spaces.

Resources:
- [HF Spaces app](https://huggingface.co/spaces/machhakiran/yt-agent)

## How to Run This Example

1. Clone this repo

    ```
    git clone https://github.com/machhakiran/yt-agent.git
    ```
2. Open repo directory

    ```
    cd yt-agent-streamlit
    ```
3. Install dependencies

    ```
    uv sync
    ```
4. Run Streamlit app

    ```
    uv run streamlit run main.py
    ```

## Hosting on HF Space

1. [Create new](https://huggingface.co/new-space) Hugging Face Space

    ```
    Name: yt-agent
    Description: Example Space for running YT agent Streamlit app.
    Space SDK: Docker
    Docker Template: Blank
    Space Hardware: CPU
    ```
2. Add another remote to git repo

    ```
    # In your yt-agent-streamlit directory
    git remote add hf https://huggingface.co/spaces/{your_hr_username}/yt-agent.git
    ```
3. Push code to HF spaces (may need to force first push)

    ```
    git push --force hf
    ```