# Core Principles

```
Gemini 3 favors directness over persuasion and logic over verbosity.
```
- **Precise Instructions**: Be concise in your input prompts. Gemini 3 responds best to direct, clear instructions. State your goal clearly without fluff.
- **Consistency & Defined Parameters**: Maintain a uniform structure throughout your prompts (e.g., standardized XML tags) and explicitly define ambiguous terms.
- **Output Verbosity**: By default, Gemini 3 is less verbose and prefers providing direct, efficient answers. If you require a more conversational or "chatty" persona, you must explicitly ask for it.
- **Multimodal Coherence**: Text, images, audio, or video should all be treated as equal-class inputs. Instructions should reference specific modalities clearly to ensure the model synthesizes across them rather than analyzing them in isolation.
- **Constraint Placement**: Place behavioral constraints and role definitions in the System Instruction or at the very top of the prompt to ensure they anchor the model's reasoning process.
- **Long Context Structure**: When working with large contexts (books, codebases, long videos), place your specific instructions at the end of the prompt (after the data context).
- **Context Anchoring**: When transitioning from a large block of data to your query, explicitly bridge the gap. Use a framing phrase like "Based on the information above..." before your question.
