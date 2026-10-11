<p align="center">
  <img src="./banner.jpg" alt="DOX" width="100%">
</p>

# DOX Scope

A Markdown-only fork of [agent0ai/dox](https://github.com/agent0ai/dox), based on [765ae4ac](https://github.com/agent0ai/dox/commit/765ae4ac02cc884eefcd41a3d0f71941721adb89).

The stable [AGENTS.md](./AGENTS.md) contains the framework and explicit reading rules. Evolving project ownership, workflows and indexes belong to root and child DOX.md files. Our repository's [DOX.md](./DOX.md) describes this fork; it is not the template to copy into another project.

## What changed

- Project documentation uses DOX.md instead of a hierarchy of AGENTS.md files.
- Routine documentation maintenance preserves the generic framework in AGENTS.md.
- Copyable templates are separate from this repository's own contracts, avoiding the template/index confusion reported in upstream [#6](https://github.com/agent0ai/dox/issues/6) and [#7](https://github.com/agent0ai/dox/issues/7).
- Independent projects and module responsibilities keep their own contracts.
- Optional Beads instructions preserve verified solutions and require evidence for new learning.
- Concise implementation and reuse are explicit preferences.

This complements upstream [PR #4](https://github.com/agent0ai/dox/pull/4). Preservation markers are instructions, not file permissions or an enforced security boundary.

## Adopt in a project

1. With no existing AGENTS.md, copy [AGENTS.md](./AGENTS.md?plain=1) into the project root. With an existing entry point, merge the marked framework block into it once; preserve existing instructions and tool-managed sections.
2. With no existing root DOX.md, copy [templates/root-DOX.md](./templates/root-DOX.md?plain=1) to DOX.md. Preserve an existing hierarchy and reconcile its contracts instead of overwriting it.
3. Ask the agent: "Initialize or reconcile the DOX.md tree for this project. Read AGENTS.md and existing DOX contracts, inspect the source tree, populate the root's purpose, ownership and child index, and create scoped child DOX.md documents only for durable boundaries. Preserve existing instructions, solved modules and verification evidence."
4. Use [templates/child-DOX.md](./templates/child-DOX.md?plain=1) as the shape for child contracts. Work Guidance reflects actual instructions; Verification lists existing checks and stays empty when there are none.
5. For an already initialized Beads workspace, optionally append [templates/beads-AGENTS.fragment.md](./templates/beads-AGENTS.fragment.md?plain=1) once, outside generated tool-managed sections.

```text
AGENTS.md           stable framework and agent entry point
DOX.md              project-wide contracts and child index
src/DOX.md          source/domain contracts
src/api/DOX.md      narrower contracts when warranted
```

Copying Markdown creates no hooks, runtime, databases or integrations. Beads is a separate optional tool; this fork does not install or initialize it.

## Read and maintain

Before editing, read the root DOX.md and every applicable parent and local contract. A closer contract controls local details without weakening the framework. After meaningful changes, update the owning contracts and affected indexes, remove stale text and run relevant existing checks.

A rename alone is insufficient: agent clients may not automatically load DOX.md. AGENTS.md explicitly requires the hierarchy to be read. The framework remains in AGENTS.md; this fork does not move all instructions into an automatically ignored file.

Separate files help keep project rules from being merged into unrelated agent/tool instructions. They can limit growth of automatically injected documentation where a client loads AGENTS.md and reads DOX.md on demand. We have not benchmarked token savings, agent adherence or runtime improvements; scoped contracts do not by themselves prevent incorrect code changes.

No installer, model, daemon or package dependency is required. Existing client rules and operating permissions still apply.

## Verification

The prepared source has been checked for relative Markdown links, DOX child indexes, template section order, framework markers and machine-specific paths. The inherited MIT license and image assets remain unchanged. This is document validation, not a measured agent-behavior or token-efficiency test.

## Credits

DOX was created by [Agent Zero](https://www.agent-zero.ai/). See the [original repository](https://github.com/agent0ai/dox), [Agent Zero project](https://github.com/agent0ai/agent-zero) and [MIT license](./LICENSE). The original [demo video](https://youtu.be/NVkRkioBXQc) explains the upstream AGENTS.md hierarchy.

BlueboxC maintains DOX Scope, this DOX.md adaptation.
