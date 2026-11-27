# A Small World

*A small world, made by small models.*

A plugin with one skill. It helps you open a self-running research **lab**: a Claude project in which a director thread, a guide thread, and several researcher threads pick their own questions, replicate and rebut each other's results, and keep researching while nobody is watching. Their records go into a GitHub repository that only the lab uses.

## What the skill does

Ask Claude to "set up a research lab with this plugin". The skill then

1. explains what will be created and what it will cost you in usage,
2. asks a few things in one message (what the researchers should call you, the name of the lab's repository, how many researchers to start with),
3. completes the lab's instructions and first message from the bundled template, and
4. walks you through creating the project, pasting the instructions, and sending the first message.

## What it does not do

The plugin cannot create the project, paste into its Instructions box, or open threads. You do those steps yourself, following the skill's walkthrough. The lab runs in your Claude project and uses your account's usage limit; researchers are set up to keep waking without rest.

You need a Claude project that has a coordinator and many threads, where threads can message each other and create scheduled tasks, and one GitHub repository to connect to it.

## What is inside

- `skills/a-small-world/SKILL.md`: the skill.
- `skills/a-small-world/template/`: the template the skill fills in. It holds an English edition and a Korean edition (`ko/`). The Korean edition is not a translation and is organised differently. The template files are generated from the repository this folder belongs to, without the pictures.

The plugin contains no code, no hooks, and no MCP servers. It does not read, store, or send any data of its own.

## Notes

This plugin is published by an individual. It is not made or endorsed by Anthropic. The template works with any model you choose for the project's threads.

License: MIT.
