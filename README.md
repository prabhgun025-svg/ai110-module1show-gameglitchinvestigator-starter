# 🎮 Game Glitch Investigator: The Impossible Guesser

## 🚨 The Situation

You asked an AI to build a simple "Number Guessing Game" using Streamlit.
It wrote the code, ran away, and now the game is unplayable. 

- You can't win.
- The hints lie to you.
- The secret number seems to have commitment issues.

## 🛠️ Setup

1. Install dependencies: `pip install -r requirements.txt`
2. Run the broken app: `python -m streamlit run app.py`

## 🕵️‍♂️ Your Mission

1. **Play the game.** Open the "Developer Debug Info" tab in the app to see the secret number. Try to win.
2. **Find the State Bug.** Why does the secret number change every time you click "Submit"? Ask ChatGPT: *"How do I keep a variable from resetting in Streamlit when I click a button?"*
3. **Fix the Logic.** The hints ("Higher/Lower") are wrong. Fix them.
4. **Refactor & Test.** - Move the logic into `logic_utils.py`.
   - Run `pytest` in your terminal.
   - Keep fixing until all tests pass!

## 📝 Document Your Experience

- [ ] Describe the game's purpose.
- [ ] Detail which bugs you found.
- [ ] Explain what fixes you applied.

The game's purpose is a simple guessing game in which the player will continue guessing with a limited number of attempts until they get it right. I found 3 particular bugs while playing this game. The first bug was the hint bug, where the hints were reversed. If the correct number was 50, I would guess 40, and it would tell me that 40 is too high, which is incorrect and the opposite. Another bug that I found was that the difficulties was backwards. Normal mode was more difficult compared to hard mode. The game would not also let me use the restart game button despite me pressing it. Using Prompt Engineering, I asked AI to explain the reason as to why I was facing 2 of the bugs. The hints were backwards because in the code, it switched the Low and high conditions and the reason that the difficulties were switched was because the max number was switched. I told AI to fix the code (and get it approved by me first before applying) and apply the code in app.py and logic_util.py. After a few errors, where the AI completely deleted some sections of the code and switched the code from one tab to another, I got the code fixed and the bugs, backward hints and difficluty, were both fixed. 

## 📸 Demo Walkthrough

Describe your fixed game in numbered steps so a reader can follow along without watching a video:

1. User Enters a guess of 50
2. Game returns too low
3. user enters a guess of 60
4.Game returns too high
5. game ends after correct guess
6. User restarts game and changes difficulty to hard
7. Same Steps from 1-5


## 🧪 Test Results

```
# Paste your pytest output here, e.g.:
# pytest tests/
# ========================= X passed in 0.XXs =========================
```
*Did not complete Challenge 1* 

## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, describe the Enhanced UI changes here — a screenshot is optional]
