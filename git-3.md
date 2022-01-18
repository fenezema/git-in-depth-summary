# (Section 4) Git - That One Friend/Foe You Interact with Everyday

## Danger Zones
This section will only taking main takeaways from previous sections. In short, try to avoid these destructive commands:
1. `git checkout -- <file>`
2. `git reset --hard <n HEAD>`

While on remote repo, **DO NOT** do `git push` to remote if we do one of these command:
1. `reset`
2. `rebase`
3. `amend`

It will highly interupt other works and maybe messed those up very bad, and you'll be appointed as that manacing developer that should be avoided.