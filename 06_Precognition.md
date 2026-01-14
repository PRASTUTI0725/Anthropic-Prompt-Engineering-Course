Chapter 6: Precognition (Thinking Step by Step)
Lesson Examples
Example 1 – Basic movie review sentiment

Prompt:

Is this movie review sentiment positive or negative?

This movie blew my mind with its freshness and originality. In totally unrelated news, I have been living under a rock since the year 1900.


Claude's Response:

Negative.

This review is sarcastic. The reviewer is sarcastically claiming the movie is fresh and original, then immediately undercuts that claim by saying they've been "living under a rock since 1900" - implying that anyone with even minimal exposure to modern media would recognize the movie as derivative and unoriginal. The sarcasm reveals the reviewer actually found the movie stale and lacking in originality.

Example 2 – Movie review sentiment with step-by-step thinking

Prompt:

Is this review sentiment positive or negative? First, write the best arguments for each side in <positive> and <negative> XML tags, then answer.

This movie blew my mind with its freshness and originality. In totally unrelated news, I have been living under a rock since 1900.


Claude's Response:

<positive> The first sentence explicitly praises the movie, stating it "blew my mind" and calling it "fresh" and "original." These are clearly positive descriptors that express strong appreciation for the film. </positive> 
<negative> The second sentence is sarcastic and undercuts the first statement. By claiming to have been "living under a rock since 1900," the reviewer is sarcastically implying that only someone completely out of touch with cinema would find this movie fresh or original. The phrase "in totally unrelated news" signals the sarcasm - it's actually very related, suggesting the movie is derivative and unoriginal, and only someone with zero cultural context would think otherwise. </negative>
Answer: Negative

This is a sarcastic negative review. The reviewer uses irony to criticize the movie - the praise in the first sentence is immediately revealed as insincere by the sarcastic second sentence, which implies the movie is actually stale and unoriginal.

Example 3 – Movie review sentiment, negative first then positive

Prompt:

Is this review sentiment negative or positive? First write the best arguments for each side in <negative> and <positive> XML tags, then answer.

This movie blew my mind with its freshness and originality. Unrelatedly, I have been living under a rock since 1900.


Claude's Response:

<negative> The second sentence is sarcastic and undermines the first. By claiming to have been "living under a rock since 1900," the reviewer sarcastically implies that only someone completely disconnected from cinema history would find this movie fresh or original. The word "Unrelatedly" signals irony - it's actually very related. This suggests the movie is derivative and unoriginal, and the opening praise is insincere mockery. </negative> 
<positive> The first sentence contains explicit praise: "blew my mind," "freshness," and "originality" are all positive terms expressing genuine appreciation. The second sentence, while unusual, could be read as self-deprecating humor - the reviewer acknowledging their own limited movie-watching experience rather than criticizing the film. They might be saying "I don't watch many movies, so this seemed amazing to me," which doesn't necessarily make their positive reaction invalid or sarcastic. </positive>
Answer: Negative

This is a sarcastic negative review. The sarcasm is clear from the juxtaposition of the two sentences - the reviewer is using irony to suggest the movie is actually stale and unoriginal, and only someone with no exposure to cinema would think otherwise.

Example 4 – Famous movie starring an actor born in 1956 (simple)

Prompt:

Name a famous movie starring an actor who was born in the year 1956.


Claude's Response:

Pulp Fiction (1994), starring Tom Hanks.

Tom Hanks was born on July 9, 1956, and has starred in many famous films including Forrest Gump, Saving Private Ryan, Cast Away, and The Green Mile.

Example 5 – Famous movie starring an actor born in 1956 (step-by-step thinking)

Prompt:

Name a famous movie starring an actor who was born in the year 1956. First brainstorm about some actors and their birth years in <brainstorm> tags, then give your answer.


Claude's Response:

<brainstorm> Let me think about actors born in 1956: 
- Tom Hanks - born July 9, 1956 
- Mel Gibson - born January 3, 1956 
- Carrie Fisher - born October 21, 1956 
- Bryan Cranston - born March 7, 1956 
- Nathan Lane - born February 3, 1956

Tom Hanks has been in many famous movies: Forrest Gump, Saving Private Ryan, Cast Away, Philadelphia, The Green Mile, Toy Story series, Apollo 13, Big, Sleepless in Seattle, etc.

Mel Gibson starred in: Braveheart, Lethal Weapon series, Mad Max series, The Patriot, Signs, etc.

Carrie Fisher is most famous for Star Wars as Princess Leia. </brainstorm>

Forrest Gump (1994), starring Tom Hanks, who was born in 1956. This is one of the most famous and beloved films of the 1990s, winning multiple Academy Awards including Best Picture and Best Actor for Hanks.

Exercise 6.1 – Classifying Emails

Prompt Template:

Please classify this email and ONLY return the classification (letter and category): {email}


Emails & Claude's Responses:

Email:

Hi -- My Mixmaster4000 is producing a strange noise when I operate it. It also smells a bit smoky and plasticky, like burning electronics. I need a replacement.


Response:

B. Broken or defective item


Email:

Can I use my Mixmaster 4000 to mix paint, or is it only meant for mixing food?


Response:

A. Pre-sale question


Email:

I HAVE BEEN WAITING 4 MONTHS FOR MY MONTHLY CHARGES TO END AFTER CANCELLING!! WTF IS GOING ON???


Response:

C. Billing question


Email:

How did I get here I am not good with computer. Halp.


Response:

D. Other (please explain)

Exercise 6.2 – Email Classification Formatting (XML Output)

Prompt Template:

Please classify this email and wrap JUST the letter of the classification in <answer></answer> tags: {email}


Emails & Expected Responses:

Email:

Hi -- My Mixmaster4000 is producing a strange noise when I operate it. It also smells a bit smoky and plasticky, like burning electronics. I need a replacement.


Response:

<answer>B</answer>


Email:

Can I use my Mixmaster 4000 to mix paint, or is it only meant for mixing food?


Response:

<answer>A</answer>


Email:

I HAVE BEEN WAITING 4 MONTHS FOR MY MONTHLY CHARGES TO END AFTER CANCELLING!! WTF IS GOING ON???


Response:

<answer>C</answer>


Email:

How did I get here I am not good with computer. Halp.


Response:

<answer>D</answer>