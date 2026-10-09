---
name: update-rules
description: "A reminder and guide for agents to always update the .agents/rules files whenever new lore, distances, logic, or names are established or changed during chapter writing."
---

# Updating Rules

When writing a fantasy book as vast and complex as *The Crown of Ratherlon*, continuity is king. You MUST proactively update the rule and lore files within the `.agents/rules` directory whenever a new world-building decision is made, an old rule is changed, or new constraints (geography, logistics, lore) are introduced.

## Why is this necessary?
Because you, the agent, do not share memory across new conversations or context windows unless the rules are permanently documented in the workspace. If you invent a new character, determine a travel distance, establish a battle route, or change a character's motivation (like King Rodrik's reason for not naming an heir), and you *do not* update the `.agents` files, future agents will contradict your work.

## When to update rules
1. **Geography & Logistics:** You establish a distance, travel speed, or route between two locations. Update `geography-and-logistics.md`.
2. **Lore & History:** A new piece of history, naming convention, or lore (e.g. Ashen wars, Nyxen behaviors) is locked in. Update the relevant world-building file or create a new one.
3. **Character Arcs & Motivations:** A character's core motivation or backstory is altered (e.g., Rodrik's succession logic). Update the `twin-war-dynamics-1.md` or `book-outline-1.md`.
4. **Vocabulary:** A new specific term (like *Redcut* or *Hallow Ford*) is introduced and meant to be recurring. Add it alphabetically to `dictionary.md` AND `.agents/rules/dictionary.md`.
5. **Direct User Request:** The user explicitly tells you a rule has changed or provides new constraints.

## How to update rules
Always use your `multi_replace_file_content` or `replace_file_content` tools to make targeted updates to the existing `.agents/rules/` markdown files. If a completely new category of rule is established, use `write_to_file` to create a new `.md` file in the `.agents/rules/` directory.

**Never wait for the user to tell you to update the rules.** If you make a lasting decision for the book, document it immediately.
