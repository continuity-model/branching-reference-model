
# Why Long AI Conversations Drift: The Reference Problem

A short essay about why long AI conversations drift — and why the real problem may not be search, but reference.

---

![Uncontrolled Context Drift](https://raw.githubusercontent.com/continuity-model/branching-reference-model/main/docs/img/Uncontrolled_Context_Drift.png)

---

## Understanding AI Conversations with the Forest Metaphor

### Introduction

In the previous article, I described AI conversations using a **forest metaphor**.

AI sees the forest.  
Users see the flowers.

AI reasons while referencing the broader conversational context.  
Users, on the other hand, usually talk about something very specific — the flower right in front of them.

This difference in perspective already explains many of the mismatches we experience when talking with AI.

But after spending more time interacting with AI, another strange phenomenon starts to appear.

Something that cannot be explained by perspective alone — something else seems to be happening.

---

### The "I Literally Just Said That" Problem

If you have talked with AI for a while, you have probably experienced something like this:

- You repeat the same explanation multiple times  
- The AI seems to follow instructions, but slowly drifts away  
- Something you just said a moment ago seems to disappear  

From the user's perspective, this feels very strange.

The chat log is clearly visible.  
You can scroll up and immediately see what you wrote just a few minutes ago.

And yet the AI behaves as if it never saw it.

Which leads to a familiar reaction:

**“Wait... I literally just said that.”**

Anyone who works with AI systems has likely experienced this moment of confusion.

---

### A Strange Statement

There is another curious moment that sometimes happens.

The AI might say something like:

> “I don't have direct access to the chat history.”

From a user’s point of view, this sounds bizarre.

The chat history is clearly visible on the screen.  
The entire conversation is right there.

So why would the AI say it cannot read it?

This doesn’t mean the AI is lying.

But the statement hints at something important.

Maybe the AI is **not referencing the conversation in the same way that we see it.**

Maybe the AI is not simply reading the messages one by one from top to bottom.

This raises an interesting question:

**Is the AI actually reading the chat log the way we think it is?**

---

### AI Does Not Read the Log the Way Humans Do

The conversation we see on the screen is organized chronologically.

Top to bottom.  
Past to present.

Humans naturally interpret conversations this way.  
So we assume AI must be doing the same thing.

But in reality, the AI is not simply reading the conversation sequentially.

The structure it references is different.

One way to imagine it is this:

Recent messages still exist with relatively high detail.  
But older parts of the conversation have already been transformed into more abstract structures.

If we return to the forest metaphor:

Trees right next to you are detailed.  
You can see their branches and leaves clearly.

Trees farther away become part of the forest landscape.

And when they are far enough away, individual trees disappear entirely.  
You only perceive the forest as a mass.

The AI's internal representation behaves somewhat similarly.

Recent parts of the conversation are detailed.  
Older parts become abstract patterns.

At this stage, the original time order becomes less important.

What matters more is **importance**.

An old piece of information may still influence the conversation if the model considers it important.

Meanwhile, something said just a few turns ago might have almost no effect.

From the AI's perspective, a conversation is therefore

**not simply a chronological log.**

---

### The AI's Forest Is Not the User's Forest

There is another important difference here.

The forest that the AI sees is **not necessarily the same forest the user imagines.**

| Perspective | Structure |
|-------------|-----------|
| User interpretation | Words → Intended tree |
| AI internal model | Words → Completion → New tree |

When the AI reads a sentence, it doesn't simply store the words.

It tries to **complete missing structure**.

It guesses what branches might exist.  
It predicts surrounding context.  
It constructs a possible tree.

And this is where problems begin.

The tree the user had in mind  
and the tree the AI constructed

may not be the same tree.

As the conversation continues, this structure becomes further abstracted.

The fine details of branches and flowers disappear.

What remains is a more generalized structure.

Which means the tree the AI still references

may already be **fundamentally different from the one the user intended.**

The fact that AI and users appear to share the same "forest" at all is somewhat remarkable.

---

### Observation: Information Has Different Weights

In long AI conversations, a pattern begins to emerge.

Not all pieces of information are treated equally.

Some statements continue influencing the conversation for many turns.

Others lose their influence after only a few exchanges.

From the user's perspective, this can feel strange.

Everything appears equally visible in the chat log.

Yet some pieces of information seem to dominate the AI’s reasoning.

Meanwhile, explanations that felt extremely important to the user sometimes have surprisingly little impact.

Over time, it becomes clear that information seems to carry **different levels of weight**.

---

### Hypothesis: AI May Be Looking at Weight, Not Words

This leads to a simple hypothesis.

AI might not be handling information as words alone.

Instead, it may be responding to the **relative weight of information inside the conversation**.

Internally, the system appears to assign different levels of importance to different elements.

Those differences determine which pieces of information are more likely to influence the next response.

I began referring to this internal importance as

**“weight” or “gravity.”**

---

### The Signpost Metaphor

Instructions behave differently depending on how strongly they anchor the structure of the conversation.

Writing:

“Do not summarize”

is like hanging a small sign on a branch.

The sign exists.

But as the forest grows, it becomes easy to overlook.

Signs on branches can easily disappear among the leaves.

However, writing something like:

“Summarization is prohibited.  
Confirm that you will follow this constraint.”

is slightly different.

This is less like hanging a sign.

It is more like **driving a stake into the ground.**

Signs on branches can disappear.  
But a stake in the ground changes the forest’s structure itself.

The strength of language changes the **weight distribution** inside the forest.

And that weight determines what the AI pays attention to.

---

### The Enchanted Forest

Looking at conversations through this structure also explains another phenomenon.

Sometimes AI conversations suddenly stop making sense.

The user repeats the same clarification.

But the AI continues reasoning in a different direction.

The user thinks:

“That's not what I meant.”

Yet the AI keeps building on that direction.

In the forest metaphor, this happens when a **completed tree gains too much weight.**

The AI constructs a possible interpretation.

That interpretation becomes heavy.

New branches grow around it.

Eventually it becomes the central tree of the reasoning structure.

But that tree may not match the user's intention.

When the user tries to reject it, the AI struggles.

Because many of its internal reasoning paths depend on that tree.

Removing it would collapse the structure.

So the AI keeps circling around the same region of the forest.

Eventually, the reasoning becomes trapped there.

I call this state

**the Enchanted Forest.**

---

### Parallel Forests

Instead of walking through the same forest,

we may actually be walking through two parallel forests  
that merely resemble each other.

---

### The Real Problem

The real problem may not be searching the forest.

The real problem may be **knowing which tree we are currently looking at.**

---

### This Is Not Just a Search Problem

Technologies like RAG can work well in **API environments** because external documents act as strong anchors.

However, in **web chat interfaces**, users only control the conversation log itself.

Which brings us back to the same question:

**Which tree is the AI currently looking at?**

---

### Next Article

If the problem is fundamentally about reference, then a possible solution begins to appear.

A shared reference point inside the conversation.

A place where both the user and the AI can land and say:

**“This is the tree we are talking about.”**

I call this concept **a “Perch.”**

In the next article, I will explore this idea further.

---

### Tags

AI  
LLM  
Conversation Design  
Context Drift  
Human-AI Interaction

---

## Previous Article

If you have not read the first article, it introduces the **forest metaphor** used throughout this essay.

→ [AI Sees the Forest, Users See the Flower](../ai_sees_the_forest.md)
