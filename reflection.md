# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?




- List at least two concrete bugs you noticed at the start 
  (for example: "the hints were backwards").

    The game tells you to go higher when you should be going lower, and lower when you should be going higher.
    The game doesn't let you use enter to submit even though there's an enter to apply prompt

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|   70  | "go higher"          "go lower"        none
|  340  | "not in bounds"     "go higher         none
|  90   | "go lower"           "go higher"        none

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  I used the Copilot that was built into VS code
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  The AI suggested swapping the messages for the hints, I verified this would fix the backwards hints.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  The AI suggested a 1-100 range instead of ensuring the range was low to high

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  I played the game several times to ensure the bug did not reappear.
- Describe at least one test you ran (manual or using pytest)  
  I purposefully entered guesses out of range to make sure the game was no longer counting them as guesses.
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?


---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

Streamlit reruns mean streamlit re reads the entire code file every time you interact with the app, so the variables instantly reset. Session state is used to keep a memory, during reruns, during this game it would be used to keep a counter of guesses.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
  I want to keep my habit of using AI to help me understand why a bug happened and how to fix it, rather than trying to have to fix the whole app for me without looking for bugs myself.
- What is one thing you would do differently next time you work with AI on a coding task?
  I would utilize AI more for testing and spend more time understanding the code before starting to work. 
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  It made me realize I need to be more wary of what AI produces and I need to be intential with my prompts.
