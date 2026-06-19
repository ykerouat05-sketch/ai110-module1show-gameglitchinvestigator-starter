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

- [ ] Describe the game's purpose. the game is a secret guesser where the user enters a number and tries to guess the hidden secret number. the goal is to continue guessing until the coirrect number is found
- [ ] Detail which bugs you found. I found several bugs related to the game logic like hints were backward, the game doesn't reset with new game 
- [ ] Explain what fixes you applied. I used vs code AI assistant to help identify the bug and understand their causes and then i applied the suggested fixes and verified that the bugs were resolved using pytest

## 📸 Demo Walkthrough

Describe your fixed game in numbered steps so a reader can follow along without watching a video:

1. <!-- Describe this step --> user enters a guess of 50
2. <!-- Describe this step --> game returns "too high"
3. <!-- Describe this step --> user enters guess of 20 --> too low
4. <!-- Describe this step --> score updates correctly after each score and attempts decrease with each false guess
5. <!-- Add more steps as needed --> game ends after the correct score or after attempts hit 0

**Screenshot** *(optional)*: <!-- Insert a screenshot of your fixed, winning game here -->

## 🧪 Test Results

```
# Paste your pytest output here, e.g.:
#========================= test session starts ========================
#platform win32 -- Python 3.14.3, pytest-9.0.3, pluggy-1.6.0
#rootdir: C:\Users\kerouat\OneDrive - Morgan State University\Documents\ai110-module1tinker-playlistchaos-starter-main
#plugins: anyio-4.13.0
#collected 3 #items                                                                                                                                                                                                    

#ai110-module1show-gameglitchinvestigator-starter\tests\test_game_logic.#py ...                                                                                                                                  [100%]

=========================== 3 passed in 0.11s =========================
# pytest tests/
# ========================= X passed in 0.XXs =========================
```

## 🚀 Stretch Features

- [ ] [If you choose to complete Challenge 4, describe the Enhanced UI changes here — a screenshot is optional]
