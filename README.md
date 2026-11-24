# project-genai-post-generator
This tool will analyze posts of a LinkedIn influencer and help them create the new posts based on the writing style in their old posts  

<img src="resources/tool.jpg"/>

Let's say Mohan is a LinkedIn influencer and he needs help in writing his future posts. He can feed his past LinkedIn posts to this tool and it will extract key topics. Then he can select the topic, length, language etc. and use Generate button to create a new post that will match his writing style. 

## Stage 2 Technical Architecture
<img src="resources/stage2.jpg"/>

Use the selected topic, language, and length to generate a new post. Past posts matching the topic, language, and length are used as few-shot examples to guide the LLM's writing style.

## Set-up
1. To get started we first need to get an API_KEY from here: https://console.groq.com/keys. Inside `.env` update the value of `GROQ_API_KEY` with the API_KEY you created. 
2. To get started, first install the dependencies using:
    ```commandline
     pip install -r requirements.txt
    ```
3. Run the streamlit app:
   ```commandline
   streamlit run main.py
   ```
Copyright (C) Codebasics Inc. All rights reserved.


**Additional Terms:**
This software is licensed under the MIT License. However, commercial use of this software is strictly prohibited without prior written permission from the author. Attribution must be given in all copies or substantial portions of the software.
