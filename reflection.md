# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
  
The game looked normal at the beginning, before I ran it. It just told me to guess a number and I did. When I first guessed a number, it told me to go higher but the answer was below my first guess. This told me that the hints were most likely backwards. I tried it again doing the opposite, and it confirmed that the hints were backwards. Another bug I saw was that the New Game button was not working. I expected that after  It was not starting a new game after the orginal game ended. Bug number 3 that I found is that if I change the difficulty level to hard, it will lower the range in turn making it easier to guess rather than harder.
**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|guess of 40| hint says too high | hint says low| no console error
| press button for new game | new game starts with new number| nothing happens| no console error
| change difficulty to hard | the range is larger making it difficult to guess the right number | the range is lower | no console error

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
