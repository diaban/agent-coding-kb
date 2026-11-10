# Open questions

## From the second synthesis

1. **What should be measured?** Shares of AI code count lines. What measure would capture value delivered and the cost of verification?
2. **Who is accountable?** When nobody has read the code, who answers for an incident: the team, the agent's vendor, the author of the specification?
3. **How is skill kept?** What practices preserve the human ability to take over if people no longer write code? See [ironies of automation](concepts/ironies-of-automation.md).
4. **Do the tests verify anything?** Do tests written by agents, for code written by agents, detect the errors that matter? See [Goodhart's law](concepts/goodharts-law.md).
5. **Can an agent language be born without training data?** Or will it take the form of an intermediate representation under existing languages? See [cold start](languages/cold-start.md).
6. **Will text remain the pivot format?** Or will structured representations take over, with text as a mere view?
7. **Who will choose the language of agents?** If training data decides, does the choice belong only to the companies that train models?
8. **What language for a harness?** Throwaway code, tool protocols, or a mix of both?

## Added while building this base

9. **How far does the compiler analogy hold?** Can per-output verification replace the tool-level correctness that made assembly unread? See [compilers](precedents/compilers.md).
10. **Does a precise specification become a programming language again?** See [scenario 2](scenarios/02-spec-as-language.md).
11. **What would make adoption go backwards?** Which incident rate or cost would lead teams to restore systematic review? See [scenario 4](scenarios/04-backlash.md).
12. **Is the lock-in loop measurable?** Is the share of a few languages in generated code actually rising?
13. **What happens to existing code?** Both syntheses reason about new code. Most code in production was written by humans and has to be maintained.
