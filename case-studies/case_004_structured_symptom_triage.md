# Case Study: Structured Symptom Triage Before Answering

## Context

The trigger was simple:

“I have a problem.”

However, instead of asking clarifying questions,  
AI systems tend to immediately produce answers.

This behavior becomes especially problematic in real-world scenarios  
where context is incomplete or hidden.

## Example

A home network setup involving a Sony TV and a Bose smart speaker  
was causing unexpected behavior.

This combination is known to be problematic among experienced users,  
due to conflicting audio routing and control behaviors between devices.

Without structured reasoning, the AI repeatedly produced generic explanations  
based on common patterns.

None of them addressed the actual setup.

The situation continued for nearly three days,  
with multiple attempts leading to no resolution.

Using a structured symptom-based approach:

- The process started with clarification instead of answers  
- The specific device combination was identified  
- Possible causes were narrowed based on actual context  

## Problem

- No clarification before answering  
- Missing critical context  
- High risk of incorrect assumptions  
- Repeated irrelevant or generic responses  

## Typical Failure

Without structured control:

- AI answers immediately without understanding the situation  
- Assumptions are made based on incomplete information  
- Generic troubleshooting paths are repeated  
- The user is forced into trial-and-error cycles  

## Approach

A structured symptom triage approach was applied:

- prioritizing observation before explanation  
- delaying answers until sufficient context was gathered  
- explicitly separating known, unknown, and assumed elements  

## Intervention

At the point where the AI attempted to generate immediate answers,  
the process was intentionally redirected.

- Forced clarification before any explanation  
- Prevented answering without sufficient context  
- Identified key constraints (device combination, environment)  
- Narrowed the problem space based on verified information  

## Outcome

- Root cause candidates significantly narrowed (from many to a few plausible causes)  
- Irrelevant troubleshooting paths eliminated  
- Time lost due to repeated trial-and-error reduced  
- Problem understanding stabilized  

## Insight

The problem was not incorrect answers.

It was answering before understanding the problem.

Not better answers,  
but delaying answers until context is clear  
changed the outcome.

## Impact

- Reduced frustration in problem-solving  
- Prevented unnecessary trial-and-error cycles  
- Enabled structured troubleshooting in complex environments  

## Note

This approach is available as a free release:

→ https://github.com/continuity-model/branching-reference-model/releases/tag/symptom-stable-v1.2

It was achieved using a standard AI model  
without any special setup, tuning, or external tools.

Only the **structure of problem understanding** was changed.
