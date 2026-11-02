# TCDD-Subset

This subset is constructed from the full TCDD dataset, which contains three types of data: single-turn single-tool calls, single-turn multiple-tool calls, and multi-turn tool calls. We focus exclusively on multi-turn conversations.

We group conversations by the task associated with their final tool call and assign difficulty scores based on features such as contextual references, tool switching, and argument complexity. We then select approximately the top 10% of conversations within each task, retaining at least five conversations for tasks with fewer samples. Selection preserves complete conversations and does not use predictions from any model.

The resulting subset contains 128 multi-turn conversations spanning eight tasks, supporting evaluation of model performance in more challenging multi-turn tool-calling scenarios.
