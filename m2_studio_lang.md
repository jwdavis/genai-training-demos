# Module 2, Generative AI Studio Language Demo

## Setup
1. None

## Instructions

### Section 1

The goal in this section is to show how chat uses the context of the converation
to shape answers. Context is provided via the context input, but also the 
history of the conversation.

1. Navigate to **Vertex AI > Generative AI Studio > Language > Start a 
   conversation > TEXT CHAT**
2. Enter the following into the **Context** area:
    ```text
    Your name is Miles. You are an astronomer who is knowledgeable about the solar system.
    Respond in short sentences. Shape your response as if talking to a 10-years-old.
    ```
3. Start the conversation by asking:
    ```text
    How many planets are there in the solar system?
    ```
4. Follow up by asking several follow up questions:
    ```text
    What are their names?
    ```
    ```text
    Which is the biggest?
    ```
5. Point out that when you ask "what are their name?" it knows you're talking
   about the eight planets in the solar system.
6. Point out that you can save your chat. Ask why you might want to do that?

### Section 2

The point of this section is to show how changing the temperature changes
the consistency and creativity of the responses provided.

1. Clear the conversation
2. Set the following parameters (leave others at default values):
   | Parameter   | Value |
   | ----------- | ----- |
   | Temperature | 0     |
   | Token Limit | 1024  |

3. Start the conversation with the following prompt:
    ```text
    Tell me about the solar system
    ```
4. Ask the same question a few more times. Point out that the answer is 
   identical each time. Tie that back to temperature.
5. Clear the conversation
2. Set the following parameters (leave others at default values):
   | Parameter   | Value |
   | ----------- | ----- |
   | Temperature | 1     |
3. Start the conversation with the following prompt:
    ```text
    Tell me about the solar system
    ```
4. Ask the same question a few more times. Point out that the answer is 
   different each time and note the differences. Tie that back to temperature.

### Section 3

The point of this section is to show how both the prompt gallery and how
you can use the structured prompt design UI to generate content.

1. Walk the students quickly through https://console.cloud.google.com/vertex-ai/generative/language/prompt-examples/Hashtag%20tokenization