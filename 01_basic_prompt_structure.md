# Chapter 1 – Basic Prompt Structure

## 1. Prompts I Tested
In this chapter, I explored how the model responds to simple, clear prompts and how modifying instructions can improve output control. The following types of prompts were tested:

- Simple conversational questions  
- Factual questions  
- Instruction-based prompts  
- Constraint-based prompts  
- Role-based prompts (system prompt simulation)

---

## 2. Bad Prompt → Improved Prompt Examples

### Example 1 – Counting to Three
**Bad Prompt:**  
Count to three.  

**Response:**  
One, two, three.  

**Improved Prompt:**  
Count to three. Output only the numbers, each on a new line. Do not add any extra text.  

**Response:**  
1  
2  
3  

**Lesson:** Adding explicit constraints ensures cleaner, predictable output and removes unnecessary text.

---

### Example 2 – System Prompt (Role-Based)
**System Role Prompt:**  
You are a 3-year-old child. You speak in a playful, simple way, sometimes giggling, and stretching words. Question: How big is the sky?  

**Response:**  
Ooooh! The sky is soooo big! It's like... it goes up up up and never stops! giggles  
It's bigger than my house and bigger than the park and bigger than EVERYTHING!  
Sometimes I try to touch it but it's toooo far away. And it has clouds that look like bunnies and the sun is up there too and it's really really bright!  
Mama says the sky goes on forever and ever and everrrrr! That's SO big! spins around looking up  

**Lesson:** System prompts provide context and control over tone and style. By specifying a role, the model adapts its language and personality accordingly.

---

### Example 3 – Simple Factual Questions
**Prompt:**  
Hi Claude, how are you?  

**Response:**  
Hi! I'm doing well, thanks for asking. I'm here and ready to help with whatever you need - whether that's answering questions, working through problems, having a conversation, or anything else. What's on your mind today?  

**Prompt:**  
Can you tell me the color of the ocean?  

**Response:**  
The ocean typically appears blue, though its color can vary quite a bit depending on several factors.  
The blue color comes mainly from water absorbing colors in the red part of the light spectrum and reflecting blue wavelengths back to our eyes. Deeper, clearer ocean water tends to be a rich, dark blue.  
But you'll see lots of variation - coastal waters might look turquoise or greenish due to sediments, algae, and shallow depths. In some places the ocean can appear gray under overcast skies, or take on golden or reddish hues during sunrise and sunset. Areas with lots of phytoplankton might look greener, while tropical waters over white sand can be that gorgeous bright turquoise.  
Is there a particular aspect of ocean color you're curious about?  

**Prompt:**  
What year was Celine Dion born in?  

**Response:**  
Celine Dion was born in 1968. She was born on March 30, 1968, in Charlemagne, Quebec, Canada.  

**Lesson:** Clear, factual prompts produce accurate answers. No additional instructions or roles are required for straightforward information.

---

## 3. Key Learnings

- Models follow instructions literally; vagueness leads to assumptions.  
- Explicit constraints improve output clarity and control.  
- Role or system prompts strongly influence tone, style, and personality.  
- Simple questions produce predictable outputs, but prompt phrasing still matters.  
- Experimenting with prompts reveals how small wording changes can drastically change results.  

---

**Summary:**  
Chapter 1 demonstrated that controlling output is about **clarity, constraints, and context**. System prompts allow manipulation of tone and personality, while improved instruction phrasing ensures accurate, clean, and predictable outputs. These principles form the foundation of effective prompt engineering.
