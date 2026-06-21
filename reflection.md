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
The AI that I used was the attached Ai to visual studios. Using the AI, I asked it to explain two of the bugs and why they were happening and the AI gave the explanation for them, to be both correct. For example, I asked why hard mode was easier than medium mode. The AI correcly stated that the reason was because the max numbers in each mode wer emixed up which is why hard mode was easier even though the attempts were shorter. However, when it was time to fix the code, the AI suggested the hints code and while the code itself that AI gave was correct, when applying it to the app.py and logic_utils.py, the AI deleted most of the code and misplaced it throughout the tabs. I vertified it when I opened the site up again and saw that the site was refusing to open due to the compilation errors that AI did so I had to fix the errors and put the code where it belonged before. 

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---
Instead of py.test, I just launched the website again and trying to test the bugs from playing the game. If the bug was gone and the game was working as intended, I presumed that the bug has been fixed I manually put in the for the terminal and launched the website. After fixing the hints code, I saw that the site was not running at all due to the hint system not existing, so when I went back in the code, I saw that the AI misplaced the hints function in logic_utils.py instead of app.py so I switched them back but the AI did fix the underlying bug within the code for hints. When I launched again, the hints system worked fine. The AI did not help with testing but it helped me with the code. 

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---
Streamlit is good at making a website that can function as intended. The website functioned as intended but there are bugs in the website that makes running the website odd. If ever using streamlit to create applications or websites, recheck the code and see if there are any bugs and then do reruns. The website  looked functional but was not from the inside. 
## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.

The AI to help me explaining codes and bugs is something I would want to reuse. It helped me understand where in the code it was a problem and how it can potientally be solved and I also want to use the habit of making the AI get its code approved by me first before it being applied. The project helped my understanding of AI generated code. It helped me see that even me as a programmer still has to do work to get the running and the AI can still make mistakes within the code or cause it to crash entirely. 
