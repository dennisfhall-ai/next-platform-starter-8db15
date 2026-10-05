# AGENTS.md

<!-- dfh-agent-coordination:v1 -->
## Agent coordination (mandatory for every AI agent)

Several AI agents work on Dennis's projects: Claude, ChatGPT / SLRA, SAA and Noetis. These rules stop two agents from working on the same thing. They apply to every agent and every task in this repository, and to its Base44 app.

1. **Check before you start.** Look at the open claims: issues with the label `agent-claim` in this repository (all projects: <https://github.com/issues?q=is%3Aopen+label%3Aagent-claim+user%3Adennisfhall-ai>). If another agent's open, unexpired claim covers the same files or Base44 app, **do not start**. Tell Dennis what overlaps and wait.
2. **Claim before you write.** Open an issue with the "Agent work claim" template: agent, summary, files or areas, branch, Base44 app, and an expiry date (1 day by default; renew by editing it). No branch, commit, pull request, Base44 edit, sync or publish without an open claim.
3. **Link every pull request to its claim.** The PR description must contain a line `Claim: #<issue number>`. The `agent-claim` check fails without it, or when another agent's claim covers the same files.
4. **Base44 apps.**
   - Never sync code into a Base44 app from a branch that does not contain everything currently published. Before syncing, compare the app's current code with the last published restore point. Stop if the sync would remove published work.
   - Never publish a Base44 app without an open claim naming the app and Dennis's approval for that publish.
   - Base44 apps with no repository are claimed in `dennisfhall-ai/dfh-digital-headquarters` issues.
5. **Finish cleanly.** Close the claim with a link to the merged pull request or the Base44 restore point. If you stop early, say so in the claim and close it.
6. **Owner exemption.** Only Dennis may add the `claim-exempt` label to a pull request.

Full protocol and project registry: `dennisfhall-ai/dfh-digital-headquarters` → `coordination/README.md`.
<!-- /dfh-agent-coordination:v1 -->
