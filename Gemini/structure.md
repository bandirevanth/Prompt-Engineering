# Structured Prompting

Use XML-style tagging or Markdown to structure prompts. This provides unambiguous boundaries that help the model distinguish between instructions and data. Don't mix XML or Markdown, choose one format for consistency.

### XML Example:

```
<rules>
    1. Be objective.
    2. Cite sources.
</rules>
 
<planning_process>
    1. Analyze the Request: Identify the core goal and all explicit constraints.
    2. Decompose: Break the problem into logical sub-tasks or variables.
    3. Strategize: Outline the step-by-step methodology to solve each sub-task.
    4. Verify: Check your plan for logical gaps or edge cases.
</planning_process>
 
<error_handling>
    IF <context> is empty, missing code, or lacks necessary data:
    DO NOT attempt to generate a solution.
    DO NOT make up data.
    Output a polite request for the missing information.
</error_handling>
 
<context>
    [Insert User Input Here - The model knows this is data, not instructions]
</context>
```

### Markdown Example:

```
# Identity
You are a senior solution architect.

# Constraints
- No external libraries allowed.
- Python 3.11+ syntax only.

# Output Format
Return a single code block.
```
