# Pair Thinking

*Trade the marker.*

Pair Thinking is an agent skill that turns an AI agent into a thinking
partner instead of a task runner. It works like two colleagues at a
whiteboard: the agent brings information, you bring strategy, insight, and
judgment, and you trade the marker as the topic moves.

## Why it exists

I'm a teacher with a master's degree in education and IT, and I approach
everything the way a teacher would. I'm also twice-exceptional (2e): gifted,
with a learning difference alongside it. I grew up asking "why" a lot and
often didn't get an answer.

Agents answer "why" without ever getting tired of it, so I can collaborate
with them without anyone getting annoyed with me. I ask a lot of questions:
Why did you do it that way? What does that mean? When I'm stuck, I ask for a
metaphor, then extend it myself to check that I've understood.

Left to their defaults, though, agents rush ahead on a guess, agree with you
when you're partly wrong, and either interrogate you or lecture you. Pair
Thinking puts proven teaching practices into the agent's instructions:
backward design, success criteria, scaffolding, and checks for understanding.

## What it does

- **Lets you choose the depth.** Simple questions get direct answers. For
  complex ones, the agent asks: "Would you like to talk this through, or do
  you want a quick answer?"
- **Starts from the goal.** In a talk-through, the agent first asks what's
  driving the question and what "done" looks like, then breaks the goal into
  bite-size pieces.
- **Trades the marker.** The agent asks for your strategy and insight,
  researches in the direction you set, summarizes what it found, and asks
  what you want clarified.
- **Checks understanding honestly.** When you extend one of its metaphors,
  it either confirms and builds on it, or corrects you inside the same
  metaphor. It doesn't just agree.
- **Stays brief.** Every turn gives you something useful, with at most one
  question.

## Example

> **User:** I'm seeing DHCP snooping enabled on our core and aggregation
> switches, not just the access switches. Will this cause problems?
>
> **Agent:** It doesn't have to, but it often does. Most problems come down to
> which ports are trusted between switches and how Option 82 is handled.
> Would you like to talk this through, or do you want a quick answer?
>
> **User:** Let's talk it through. It's all Juniper, and remote campuses
> occasionally don't get DHCP responses.
>
> **Agent:** Sounds like the immediate problem is DHCP failing at remote
> campuses. What would make this done for you: finding the cause, having a
> fix to apply, or deciding whether snooping should stay on the core and
> aggregation switches?

## Install

See [Install](../../README.md#install) in the repository README.

Agents load a skill when a request matches its description. To use Pair
Thinking in every conversation, add this line to your agent's instructions
file, such as `AGENTS.md` or `CLAUDE.md`:

```markdown
Follow the pair-thinking skill in every conversation.
```

## Getting the most out of it

The skill draws out your thinking, but these habits help:

- **Say what's driving you.** "I'm prepping for an interview" or "we're just
  brainstorming" changes the whole session.
- **Ask why.** Ask why it did something, or what a term means, as often as
  you need to.
- **Ask for a metaphor, then extend it.** Send your version back. If you're
  off, the agent should tell you where.
- **Choose your depth.** Say "quick answer" or "let's talk it through."
- **Push back.** If a turn feels slow, boring, or off-track, say so. The
  agent should adjust.

## Resources

The teaching practices behind the skill:

- **Backward design:** [Understanding by Design](https://cdn.vanderbilt.edu/vu-cft/resources/teaching_resources/theory/design.htm)
  (Vanderbilt Center for Teaching). Start from the desired result, then plan
  how to get there.
- **Teach-back:** [Use the Teach-Back Method](https://www.ahrq.gov/health-literacy/improve/precautions/tool5.html)
  (AHRQ). Check understanding by having people explain an idea in their own
  words, not by asking "Do you understand?"

On twice-exceptional (2e) learners:

- [Twice-Exceptional Kids: Both Gifted and Challenged](https://childmind.org/article/twice-exceptional-kids-both-gifted-and-challenged/)
  (Child Mind Institute)
- [Twice-Exceptional: Definition, Characteristics and Identification](https://www.davidsongifted.org/gifted-blog/twice-exceptional-definition-characteristics-identification/)
  (Davidson Institute)
- [Twice Exceptional (2E)](https://gtfamilytoolkit.tea.texas.gov/resources/twice-exceptional-2e)
  (Texas Education Agency)
