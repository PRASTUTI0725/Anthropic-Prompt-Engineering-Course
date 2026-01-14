Chapter 5: Formatting Output and Speaking for Claude
Overview

This chapter focuses on controlling how Claude responds, not just what it responds with. You’ll learn how to:

Enforce structured outputs

Use XML tags for clean parsing

Guide responses by prefilling Claude’s output

Produce deterministic formats like JSON

Handle multiple outputs cleanly

XML-Formatted Output
Haiku About a Rabbit
<haiku> Soft ears standing tall, Nose twitching through clover fields, Spring's gentle jumper. </haiku>
Speaking for Claude (Prefilled Output)

By forcing Claude to begin directly inside an XML tag, we eliminate unnecessary introductions.

Haiku About a Cat
<haiku> Whiskers sense the dark, Silent paws on moonlit paths, Eyes like amber flames. </haiku>
JSON-Formatted Output

Claude can reliably output structured data when explicitly instructed.

Haiku About a Cat (JSON)

{
"first_line": "Whiskers twitch and flick",
"second_line": "Soft paws pad across the floor",
"third_line": "Purring in warm sun"
}

Multiple Inputs + XML Output
Olde English Email Rewrite

<olde_english_email>
Good morrow, Zack, I doth write to thee seeking a brief account of that prompt which thou wast charged to compose.
</olde_english_email>

Exercise 5.1: Forcing a Specific Argument
The Case for Stephen Curry as the Greatest Basketball Player of All Time

Stephen Curry has a legitimate claim to being the greatest basketball player ever because he fundamentally transformed how the game is played in a way no other player has. His impact goes beyond statistics—he changed basketball's strategic DNA.

Curry's three-point shooting revolutionized offensive philosophy across all levels of basketball. Before Curry's rise, the three-pointer was a complementary weapon; he made it the centerpiece. His ability to hit shots from 30+ feet with defenders draped on him opened up spacing that simply didn't exist before, forcing defenses to extend far beyond the three-point line and creating opportunities for teammates that previous eras never saw.

His individual accomplishments are remarkable: two MVPs (including the only unanimous MVP in NBA history), four championships with the Warriors, and he broke Ray Allen's all-time three-point record. More importantly, his gravity—the defensive attention he commands even without the ball—is unmatched. Entire defensive schemes are built around him.

Curry also proved you don't need to be the biggest or most athletic player to dominate. At 6'2" and without elite explosiveness by NBA standards, he succeeded through skill, conditioning, and basketball IQ, inspiring a generation of players.

While comparisons to Michael Jordan and LeBron James are unavoidable, Curry’s singular influence on the modern game makes his legacy uniquely transformative.

Exercise 5.2: Two Outputs, One Input
Two Haikus About Cats

<haiku_1>
Soft paws in moonlight,
Silent hunter stalks the night,
Green eyes gleaming bright.
</haiku_1>

<haiku_2>
Curled up by the fire,
Purring warmth on winter days,
Whiskers twitch in dreams.
</haiku_2>

Exercise 5.3: Two Outputs, Two Inputs
Cat Haiku

<cat_haiku>
Velvet paws that creep,
Eyes like moons in shadow's keep,
Dreams of mice in sleep.
</cat_haiku>

Dog Haiku

<dog_haiku>
Tail wagging with joy,
Loyal heart that won't decay,
Friend through every day.
</dog_haiku>

Key Takeaways

XML tags clearly separate content from explanation

Prefilling Claude’s response controls tone and structure

JSON output is achievable with strict instructions

Formatting instructions are as important as task instructions

Claude mirrors clarity — messy prompts lead to messy outputs