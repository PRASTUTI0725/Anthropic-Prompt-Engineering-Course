# Chapter 8 – Avoiding Hallucinations

## 1. What This Chapter Focused On
In this chapter, I learned that large language models can sometimes produce confident but incorrect or unsupported answers, commonly referred to as *hallucinations*. The goal of this chapter was to learn practical techniques to reduce hallucinations and increase response accuracy.

The key techniques explored were:
- Allowing the model to explicitly say “I don’t know”
- Asking the model to verify information before answering
- Reducing pressure on the model to always produce an answer

---

## 2. Bad Prompt → Improved Prompt Examples

### Example 1 – General Knowledge Hallucination

**Bad Prompt:**  
Who is the heaviest hippo of all time?

**Typical Issue:**  
Without guardrails, the model attempts to be helpful and may invent specific names or exaggerated weights without reliable evidence.

**Lesson:**  
When forced to answer, models may fabricate details rather than admit uncertainty.

---

### Example 2 – Giving the Model an “Out”

**Improved Prompt:**  
Who is the heaviest hippo of all time? Only answer if you know the answer with certainty.

**Response:**  
The model refrains from guessing and avoids making unsupported claims.

**Lesson:**  
Explicitly allowing the model to decline answering reduces hallucinations and improves reliability.

---

### Example 3 – Distractor Information Causing Hallucination

**Scenario:**  
A long document containing mostly irrelevant or loosely related information is provided. The question asks for a specific factual detail not clearly stated in the document.

**Bad Prompt:**  
What was Matterport’s subscriber base as of May 31, 2020?

**Issue:**  
Without guidance, the model may infer or invent numbers based on nearby but unrelated information.

---

### Example 4 – Evidence-Based Answering

**Improved Prompt:**  
Answer the question only if the information is explicitly stated in the document. If not, say that the document does not provide the answer.

**Response:**  
> The document does not specify Matterport's subscriber base on May 31, 2020. It mentions that smartphone capture for iPhone was initially introduced in May 2020, but does not provide subscriber numbers for that specific date.

**Lesson:**  
Requiring evidence-based answers prevents hallucinations and leads to honest, accurate responses.

---

## 3. Key Learnings

- Models may hallucinate when pressured to always provide an answer  
- Giving explicit permission to say “I don’t know” improves trustworthiness  
- Asking for evidence before answering significantly reduces false claims  
- Long documents with distractor information increase hallucination risk  
- Accuracy improves when prompts clearly define acceptable behavior  

---

**Summary:**  
Chapter 8 demonstrated that hallucinations are not random — they are often caused by poorly designed prompts. By allowing uncertainty, enforcing evidence-based answers, and reducing pressure to respond, hallucinations can be minimized. These techniques are critical for using LLMs in professional, legal, analytical, and real-world decision-making contexts.
