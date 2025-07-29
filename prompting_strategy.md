## Prompting Strategy

To classify recycling facility data, I used Gemini (`gemini-pro`) with the following prompt:

You are a classification assistant. Given the following raw material description, classify it into:

materials_category: (choose from: Electronics, Batteries, Paint & Chemicals, Medical Sharps, Textiles/Clothing, Other Important Materials)

materials_accepted: (choose items from the sublist provided in the official accepted materials list)

Respond in JSON only.

### Why This Prompt Works
- Forces structured output (JSON).
- Standardizes categories.
- Handles ambiguity and inconsistent raw data via LLM.

### Why Gemini
- Fast, cheap, and efficient for classification tasks.
- Better zero-shot reasoning in some extraction use cases.
