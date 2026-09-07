# Task automation readiness

Reusable assessment instructions and test cases for evaluating whether a
scenario can be automated with the available product and test capabilities.

## Install in your project

1. Create `agent_docs/` in the repository you will assess if it does not exist.
2. Copy the supplied files to these locations:

   | File in this package | Destination in your project |
   | --- | --- |
   | [task-automation-readiness-instructions.md](task-automation-readiness-instructions.md) | `agent_docs/task-automation-readiness-instructions.md` |
   | [test-cases.xlsx](test-cases.xlsx) | `test-cases.xlsx` in the repository root |

3. Add a link to your `AGENTS.md` so the agent can find the assessment instructions:

   ```markdown
   - Test-case automation readiness: [instructions](agent_docs/task-automation-readiness-instructions.md).
   ```

## Run the assessment

Open the coding agent in your project and provide this request:

```text
Follow agent_docs/task-automation-readiness-instructions.md.
Assess the cases marked TODO in test-cases.xlsx against this repository.
Write a compact task-automation-readiness.md report in the repository root.
Perform the assessment only. Do not implement or execute tests.
Record clarification questions in the report and complete all selected cases.
```

For other cases, replace the workbook and selection in the request. The same
instructions support spreadsheets, documents and text; no fixed case count or
status distribution is required.
