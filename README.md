# Text-to-SQL

Writing queries to solve analytical problems is a core task for a lot of data users. The challenge is to find the right data and translate the problem into correct and efficient SQL code. This becomes more difficult when data is spread across different domains. 

I'm trying to build a text-to-SQL feature that translates the analytical query into SQL code.

## Phase 1

This will be a straightforward solution where we use an LLM.

![image](https://github.com/aniket-mish/text-to-sql/assets/71699313/33a6a568-07ab-46d5-84c2-b8bea9b07ab9)

1. The user asks an analytical question and chooses the tables to be used.

2. Relevant table schemas are retrieved from the store.

3. Prompt is created with the question and table schemas.

4. The prompt is then fed to the LLM.

5. Streaming response is generated and displayed to the user.
