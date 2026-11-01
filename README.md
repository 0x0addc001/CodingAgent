# CodingAgent

**Agent-as-a-Service for software engineering.**

CodingAgent turns issues into reviewed, tested, multi-file changes inside a controlled execution environment.

面向软件工程的 Agent：在受控执行环境中把 Issue 转化为经过审查和测试的多文件代码修改。

## Agent loop

| Stage | Responsibility |
|---|---|
| Data | Repositories, issues, tests, CI logs, code history |
| Models | Code LLM, repository retriever, planning model |
| Training | SFT, rejection fine-tuning, execution-feedback RL |
| Inference | Code completion, planning, patch generation |
| Harness | Sandbox, shell, test runner, Git and review tools |
| Eval | Tests, acceptance, regressions, review quality |

## Initial scope

- Build a repository-aware context packer.
- Require executable verification before proposing completion.
- Preserve user changes and keep every edit reviewable.

## Roadmap

- [ ] Sandboxed execution runtime
- [ ] Repository retrieval baseline
- [ ] Test-driven patch loop
- [ ] Multi-agent review workflow
- [ ] Benchmark integration

## Engineering principles

- Tests are the executable specification.
- Minimize diffs and avoid unrelated rewrites.
- Never hide failed commands or skipped validation.

