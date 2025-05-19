Task is to fine-tune a Small Language Model to parse raw, unstructured text and extract relevant entities related to scheduling a calendar event. The scheduling requests can vary widely in how they are written—for example: “Let’s have a meeting next Monday with Alice for 30 minutes at the main office”. The provided base SLM struggles with this task. Your fine-tuned model should be able to reliably extract the following fields (or return null if a field is missing):

- action (e.g. “meeting”)
- date
- time
- attendees
- location
- duration
- recurrence
- notes
- 
Base SLM: HuggingFaceTB/SmolLM-360M (as well as any of its quantized versions)
Note: You are not permitted to use the SmolLM-360M-Instruct model.
