# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it? 
it looked fine no such thing broken, i ran it and it showd the hint as a correct then it started to crash as i swithc the number it still saying the same hint i assumed  the number that i am guessing is still higher as the hint says then i tried the last number and it still says higher so i figured it out that the hints are not working   correctly
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
the difficulity is not right with easy you got less attempts than normal.
when you put a geuss that is a string wich start with a number the attempt still counts but the hint says insert a number. 
the hints were backwards.
**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input  | Expected Behavior | Actual Behavior | Console Output / Error |
|------- |-------------------|-----------------|------------------------|
| 14     |go higher          |go lower         |none                    |
|new game|load new game      |nothing change   |none                    |
|easy    |more attempts      |less attempts    |none                    |

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? claude
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result). the AI suggested that the new game doesn't reset the game because of the streamlit state persists while everything else doesn't and he suggested to reset all the state.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed? I decided a bug was fixed first by testing it manually with different inputs and then i used pytest to run automated tests.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code. one test I tried was entering differnet inputs to check if the game behaved correctly in normal and edge cases. these tests helped me understand the issue and find a solution.
- Did AI help you design or understand any tests? How? yes AI helped me understand what kinds of test cases to create and suggested examples of inputs. 

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
streamlit session state works as a memory that stores vlaues between reruns so informations does not disappear every time the app refreshes that's way we need to change the state everytime we need to upload a new game.  
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
- This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
One habit that i'd like to reuse is testing frequently instead of waiting until the end. running tests help me undersstand the issue and solve it quicker.
next time i will try different prompts more specific and verify ai generated code more carefully.
this project made me understand AI generated code can help speed up developement and debugging but still needs human review and testing. 