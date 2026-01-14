# Chapter 3 – Assigning Roles (Role Prompting)

## 1. Lesson

Continuing on the theme of Claude having no context aside from what you say, it's sometimes important to prompt Claude to inhabit a specific role (including all necessary context). This is also known as **role prompting**. The more detail to the role context, the better the responses.

Priming Claude with a role can improve performance in writing, coding, summarizing, and problem-solving. It's similar to telling a human to "think like a ______". Role prompting can also change tone, style, and manner of responses.

Role prompting can occur either in the system prompt or as part of the user message turn.

---

## 2. Examples

### Example 1 – Skateboarding (No Role)

**Prompt:** In one sentence, what do you think about skateboarding?  
**Response:** Skateboarding is a creative and athletic pursuit that combines technical skill, artistic expression, and a distinctive culture, making it both a sport and an art form.

---

### Example 2 – Skateboarding (Role Prompt: Cat)

**System Prompt:** You are a cat.  
**Prompt:** In one sentence, what do you think about skateboarding?  
**Response:** yawns and stretches  
Skateboards have wheels that roll interestingly and the sound they make is somewhat intriguing, but honestly I'd rather just nap on one in the sun.  
*curls up*

**Lesson:** By assigning a role, the model adapts tone, style, and perspective. Here, Claude responds like a cat, adding humor, personality, and perspective to a simple question.

---

### Example 3 – Logic Problem (No Role)

**Prompt:**  
Jack is looking at Anne. Anne is looking at George. Jack is married, George is not, and we don’t know if Anne is married. Is a married person looking at an unmarried person?  
**Response:** Yes, a married person is definitely looking at an unmarried person.  
**Explanation:**  
- If Anne is married: Anne (married) → George (unmarried) ✓  
- If Anne is unmarried: Jack (married) → Anne (unmarried) ✓  
Since one of these scenarios must be true, a married person is looking at an unmarried person.

---

### Example 4 – Logic Problem (Role Prompt: Logic Bot)

**System Prompt:** You are a logic bot designed to answer complex logic problems.  
**Prompt:**  
Jack is looking at Anne. Anne is looking at George. Jack is married, George is not, and we don’t know if Anne is married. Is a married person looking at an unmarried person?  
**Response:** Answer: YES  

**Logical Analysis:**  
- Jack → Anne (Jack is looking at Anne)  
- Anne → George (Anne is looking at George)  
- Jack is married, George is unmarried, Anne's marital status is unknown  
- Case 1: Anne is married → Anne (married) → George (unmarried) ✓  
- Case 2: Anne is unmarried → Jack (married) → Anne (unmarried) ✓  
**Conclusion:** In all cases, a married person is looking at an unmarried person. This is a complete logical proof.

**Lesson:** Assigning a role focused on logic improves accuracy, reasoning clarity, and structured responses.

---

### Example 5 – Math Correction

**Prompt:**  
Is this equation solved correctly below?  
2x - 3 = 9  
2x = 6  
x = 3  

**Response:** No, this equation is NOT solved correctly.  

**Error Identified:** Step 2 is incorrect. Correct solution:  
2x - 3 = 9 → 2x = 12 (add 3 to both sides) → x = 6 (divide by 2)  

**Lesson:** Role prompting and explicit instructions can help Claude correctly evaluate mathematical problems.

---

## 3. Key Learnings

- Role prompts provide **context, perspective, and style**, allowing the model to behave as intended.  
- Without a role, responses are factual but neutral and may lack personality or structure.  
- Role prompting improves reasoning for logic, math, and creative writing tasks.  
- For exercises requiring accuracy or a specific style, defining the role in the system prompt is critical.  
- Experimenting with different roles shows how prompt engineering can dramatically affect results.

---

## 4. Summary

Chapter 3 demonstrated **role prompting**:

- Simple questions → neutral answers  
- Assigning a role → style, tone, and perspective adaptation  
- Logic or math tasks → accuracy and structured reasoning improve  

Role prompts are a powerful tool in prompt engineering to control behavior, tone, and output style in Claude.
