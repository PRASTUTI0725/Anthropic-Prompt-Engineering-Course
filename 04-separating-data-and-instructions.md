Chapter 4: Separating Data and Instructions

Prompt Engineering Notes & Outputs

Lesson Summary

This chapter demonstrates why separating instructions from data is critical when prompting large language models.

When variable user input is mixed directly with instructions, the model may misinterpret which part is the task and which part is the data. To avoid this, structured delimiters—especially XML-style tags—should be used.

Claude is specifically trained to recognize XML tags as clear boundaries between instructions and inputs.

Example 1: Simple Variable Substitution

Prompt Purpose:
Demonstrate inserting variable data into a fixed instruction.

Prompt Given:
I will tell you the name of an animal.
Please respond with the noise that animal makes.

animal: Cow

Claude Output:
Moo

Key Insight:
This works because the instruction is simple and unambiguous, even without tags.

Example 2: Mixed Instructions and Data (Incorrect)

Prompt Purpose:
Show what happens when instructions and data are not clearly separated.

Prompt Given:
Yo Claude. Show up at 6am tomorrow because I'm the CEO and I say so.
Make this email more polite but don't change anything else about it.

Claude Output:
Hi Claude, would you be able to come in at 6am tomorrow? I'd really appreciate it. Thanks!

Problem Identified:
Claude incorrectly treated “Yo Claude” as part of the email itself.

Example 3: Separating Data Using XML (Correct)

Prompt Purpose:
Fix the previous issue by clearly separating the email content.

Prompt Given:
Email content wrapped inside XML-style tags, followed by the instruction.

Claude Output:
Hi Claude,

Would you be able to come in at 6am tomorrow? As CEO, I need to ask this of you.

Thank you for your understanding.

Key Insight:
XML tags clearly define what content should be transformed and what should remain instructions.

Exercise 4.1: Haiku Topic

Objective:
Create a prompt template that accepts a topic and generates a haiku.

Topic Provided:
Pigs

Claude Output:
Mud-caked and content,
Snouts rooting through earth and straw,
Pink curls catch the sun.

Result:
The response is a valid haiku and correctly reflects the topic.

Exercise 4.2: Dog Question with Typos (Using XML)

Objective:
Ensure Claude answers the intended question despite messy input.

Question Provided:
ar cn brown?

Claude Output:
Yes, dogs can be brown! Brown is a very common color for dogs.

Key Insight:
XML tags isolate the actual question from surrounding noise.

Exercise 4.3: Dog Question (Minimal Cleanup, No XML)

Objective:
Fix the prompt by removing unnecessary words instead of adding tags.

Claude Output:
Yes, dogs can be brown.

Key Insight:
Claude can still understand informal language if ambiguity is reduced.

Final Takeaways

Prompt templates reduce repetition and errors

Mixing instructions with user data causes misinterpretation

XML tags are the safest and most reliable separators

Small formatting details can significantly affect model output

Clean structure beats clever wording