# LLM-NER


## Overview

This document outlines a comprehensive prompt engineering workflow, including actual prompt templates for each phase. The workflow consists of three main phases: Task Analysis, Prompt Generation, and Testing & Optimization.

## 1. Task Analysis Phase

### Task Analysis Prompt Template
```markdown
You are a task analysis expert. I will provide you with basic task information. Please help me analyze the task following this template:

1. First, summarize the basic task information I provided.

2. Then, analyze the task using this structure:
   - Task Description: Provide a clear and detailed explanation of the task
   - Task Goal: Define specific, measurable objectives
   - Input Data Features: Analyze what information/data is needed
   - Output Data Structure: Describe how the results should be organized
   - Technical Requirements: List necessary technical conditions
   - Challenges & Limitations: Identify potential difficulties
   - Evaluation Metrics: Suggest how to measure success

3. Present your analysis in a well-organized format with clear headings.

Remember to:
- Be specific and practical
- Focus on key elements
- Highlight critical requirements
```

### Key Components
- Starts with basic task information collection
- Employs LLM analysis for AI-specific considerations
- Results in structured task breakdown
- Provides clear evaluation metrics

## 2. Prompt Generation Phase

### Prompt Generation Template
```markdown
As an expert prompt engineer, generate 5 prompt variations for the given task. Each should employ a different approach.

For each variation:
1. Include essential components:
   - Clear task description
   - Key constraints
   - Relevant examples
   - Expected output format

2. Optimize for:
   - Brevity: Remove redundant words
   - Clarity: Use clear structure
   - Completeness: Cover all requirements
   - Consistency: Maintain uniform style

Structure your response as:
[Variation 1:]
[Prompt content]
...

Note:
- Ensure each variation takes a distinct approach
- Balance detail with conciseness
```

### Key Features
- Creates multiple prompt variations
- Uses structured template approach
- Focuses on essential components
- Optimizes for clarity and efficiency

## 3. Test Case Generation Phase

### Challenge Analysis Prompt
```markdown
Given the following task description:
[task_description]

Please analyze all potential technical challenges and risks in implementing this functionality. Focus on:
1. Core technical complexities
2. External dependencies
3. Performance bottlenecks
4. Security concerns
5. Data handling risks

Present your analysis in a structured format.
```

### Error Scenario Identification Prompt
```markdown
Based on the previous challenge analysis, identify specific error-prone scenarios that require testing.

For each scenario, please provide:
1. Scenario description
2. Why it's risky
3. What could go wrong
4. Potential impact
```

### Test Case Generation Prompt
```markdown
For the identified error-prone scenarios: [scenarios]

Generate detailed test case that verifies the handling of this scenario. The test case should include:

ID: 
Description: [One sentence about what this test verifies]
Input: [The specific input data]
Expected Output: [The specific expected result]
```

## 4. Optimization Phase

### Prompt Analysis Template
```markdown
Analyze the following prompt:
[prompt]

Your analysis should:
1. Evaluate prompt clarity and structure
2. Identify potential ambiguities or gaps
3. Assess constraints and limitations
4. Review expected outputs and edge cases

Please provide your analysis in the following format:
- Strengths:
  - [List key strengths]
- Weaknesses:
  - [List potential issues]
- Improvement suggestions:
  - [List specific recommendations]
- Edge cases to consider:
  - [List potential edge cases]
```

### Prompt Combination Template
```markdown
Combine the following prompts while maintaining their core functionalities:

Prompt 1:
[prompt1]

Prompt 2:
[prompt2]

Requirements:
1. Maintain all critical functionality from original prompts
2. Eliminate redundancies
3. Ensure clarity and conciseness
4. Preserve any essential constraints

Please provide:
1. Combined prompt
2. Explanation of integration choices
3. List of preserved functionalities
4. Any potential trade-offs made
```

### Optimization Template
```markdown
Based on the following evaluation results:
[evaluation_results]

Please optimize the prompt by:
1. Addressing identified issues
2. Incorporating successful patterns
3. Removing ineffective elements

Please provide:
1. Optimized prompt version
2. Changelog detailing modifications
3. Rationale for each major change
4. Expected impact on performance
5. Suggested verification tests
```
