# devflows-e2e

End-to-end test consumer for [DevFlows](https://github.com/QuanTizEd8/DevFlows).

This repository calls DevFlows reusable workflows **cross-repo**, exactly like
a real external consumer, to catch failures that DevFlows' own same-repo test
suite structurally cannot observe: runtime script delivery, nested-workflow
permission validation, and token scoping from a caller's perspective.

It is maintained as part of the DevFlows project; it contains no product code.

| Workflow | Consumes | Trigger |
| --- | --- | --- |
| `e2e-pandoc` | `pandoc.yaml@main` | manual dispatch + weekly schedule |

More consumers are added as the DevFlows catalog grows.
