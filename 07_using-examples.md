# Chapter 7 – Using Examples (Few-Shot Prompting)

## 1. Prompts I Tested
In this chapter, I explored how providing examples inside prompts (few-shot prompting) influences tone, formatting, and classification accuracy. The focus was on guiding the model by showing desired behavior instead of only describing instructions.

The following prompt types were tested:

- Conversational tone control using examples  
- Output formatting using prior examples  
- Information extraction using example patterns  
- Classification tasks with labeled examples  

---

## 2. Few-Shot Prompting Examples

### Example 1 – Tone Control Using Conversation Examples

**Prompt:**  
Please complete the conversation by writing the next line, speaking as "A".  
Q: Is the tooth fairy real?  
A: Of course, sweetie. Wrap up your tooth and put it under your pillow tonight. There might be something waiting for you in the morning.  
Q: Will Santa bring me presents on Christmas?

**Response:**  
A: Yes, if you've been good this year! Santa checks his list and brings presents to children who've been kind and helpful. Make sure to leave out some cookies and milk for him on Christmas Eve.

**Lesson:**  
Providing a prior example establishes tone, audience, and style automatically. The model continues the pattern without needing extra instructions about friendliness or wording.

---

### Example 2 – Information Extraction Using Formatting Examples

**Prompt:**  
Extract the names and professions from the text below.  
Follow the SAME format as the examples.

Silvermist Hollow, a charming village, was home to an extraordinary group of individuals.  
Among them was Dr. Liam Patel, a neurosurgeon who revolutionized surgical techniques at the regional medical center.  
Olivia Chen was an innovative architect who transformed the village's landscape with her sustainable and breathtaking designs.  
The local theater was graced by the enchanting symphonies of Ethan Kovacs, a professionally-trained musician and composer.  
Isabella Torres, a self-taught chef with a passion for locally sourced ingredients, created a culinary sensation with her farm-to-table restaurant.

1. Dr. Liam Patel [NEUROSURGEON]  
2. Olivia Chen [ARCHITECT]  
3. Ethan Kovacs [MUSICIAN AND COMPOSER]  
4. Isabella Torres [CHEF]

At the heart of the town, Chef Oliver Hamilton has transformed the culinary scene with his farm-to-table restaurant, Green Plate.  
Just down the street, head librarian Elizabeth Chen runs the Riverside Grove Library.  
Renowned artist Isabella Torres painted murals across town.  
Former Olympic swimmer Marcus Jenkins now coaches the local swim team.

**Response:**  
Chef Oliver Hamilton [CHEF]  
Elizabeth Chen [LIBRARIAN]  
Isabella Torres [ARTIST]  
Marcus Jenkins [SWIM COACH]

**Lesson:**  
By showing correctly formatted examples before new input, the model infers the structure and applies it consistently without additional formatting rules.

---

### Example 3 – Classification Using Labeled Examples

**Prompt:**  
Classify each email into one of the following categories.  
Only output the letter at the END.

(A) Pre-sale question  
(B) Broken or defective item  
(C) Billing question  
(D) Other (please explain)

Examples:  
Email: My blender arrived cracked and smells like burning plastic.  
Answer: This is a broken product. B  

Email: Why am I still being charged after cancelling my subscription?  
Answer: This is a billing issue. C  

Email: Can your product be used for mixing paint?  
Answer: This is a pre-sale question. A  

Now classify this email:  
Email: prateekbhardwaj618@gmail.com  
Answer:

**Response:**  
This doesn't appear to be an email — it's just an email address with no message content. Without an actual question or issue described, it cannot be classified into the given categories.

D - This is just an email address with no actual email content to classify.

**Lesson:**  
Few-shot examples teach both reasoning style and output format. The model correctly identifies missing context and still follows the instruction to end with the category letter.

---

## 3. Key Learnings

- Examples are often more effective than long instructions  
- Few-shot prompting strongly controls tone and structure  
- Formatting consistency can be enforced through examples alone  
- Classification accuracy improves when labeled samples are provided  
- The model generalizes patterns even with minimal guidance  

---

**Summary:**  
Chapter 7 demonstrated that few-shot prompting is a powerful technique for shaping behavior, enforcing formatting, and improving classification reliability. By showing the model what “good output” looks like, prompt complexity can be reduced while output quality increases significantly.
