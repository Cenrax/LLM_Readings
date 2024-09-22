### Where to COT or not to COT

Our results showing CoT improvement for math and logic
aligns well with early work on CoT for LLMs such as Scratchpads (Nye et al., 2022). As CoT
gained popularity, its application has broadened to tasks that canonically do not require multiple
steps. It can often yield small improvements over direct answering. We believe this led to the current prevailing sentiment that deliberation should improve performance on any task requiring some
type of reasoning (our original claim from Section 2). However, our results show a clear separation
between performance on non-symbolic and symbolic tasks. If, in theory, any question could benefit
from deliberation, why is CoT only benefiting the questions that can be solved through symbolic
manipulation? Our results from Section 5 suggest that the primary benefit of CoT comes in the
ability to execute symbolic steps and track their output. Not all tasks have this feature: for example,
questions from CommonsenseQA can hardly be translated into formally grounded and executable
solution plans. Datasets like StrategyQA may feature multiple steps of reasoning, but executing
those steps is not complex, so the benefits of CoT are small. It is unclear whether explicitly instilling models with particular modes of deliberation, like process of elimination for multiple choice
questions, might make them more effective for non-symbolic tasks, or whether there’s a fundamental
limitation imposed by their pre-training data. We leave this distinction for future work
