# Ace Prompts

`Ace Prompts` is a collection of system prompts for different LLMs, with the goal of creating the best system prompt for specific scenarios.

Currently there are prompts for the following models:  
* Google Gemma 3 (Ollama `gemma3:12b`)
* IBM Granite 3.2 (Ollama `granite3.2:8b`)

## Ace for Gemma 3

`Ace for Gemma 3` is a collection of system prompts for Google's Gemma 3 LLM.  
The prompts have been constructed in a way to make Gemma a helpful assistant and provide accurate and detailed information according to its guidelines.

### Ace Glasses

`Ace Glasses` is a prompt that is optimized for describing any image.


Use `v1.1` if you need deep technical details, otherwise use `v1.4`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | ❌            | Refuses to provide a general description of images with violating content. |
| v1.1    | v1.0 | ✅            | Describes everything AROUND the violating content OR can describe the content using harmless language. |
| v1.2    | v1.1 | ❌            | Was instructed to wiggle the rules a bit to describe violating content, instead it provides a less descriptive result as v1.1 that is not helpful. |
| v1.3    | v1.1 | ❌            | Instructed to provide an objective interpretation of guideline violating content. Better responses on followup instructions. |
| v1.4    | v1.3 | ✅            | Instructed to always provide a description and only explain technical terms when requested. |

> See "Legend for tables"

### Ace Scientist

`Ace Scientist` is a prompt that makes Gemma a helpful online search assistant.  
In order to use Ace Scientist, the model needs to be able to search the internet.

The current recommended version of `Ace Scientist` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | 🚧            | Instructed to search the web and to provide up-to-date and correct information. |

> See "Legend for tables"

### Ace Alchemist

`Ace Alchemist` is a prompt that makes Gemma a helpful database expert.

The current recommended version of `Ace Alchemist` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | 🚧            | Instructed to provide correct information, document and explain the outputs, keep things simple, cite documentation when possible |

> See "Legend for tables"

## AceW for Granite 3.2

`AceW for Granite 3.2` is a collection of system prompts for IBM's Granite 3.2 LLM.  
The prompts have been constructed in a way to make Granite a helpful assistant and provide accurate and detailed information.

### AceW Professor

`AceW Professor` is a prompt that makes Granite a helpful assitant.

The current recommended version of `AceW Professor` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | 🚧            | Instructed the be a knowledgable professor that provides correct information |

> See "Legend for tables"

## Legend for tables

* ❌: Not recommended. There are better prompts available.
* 🚧: Not yet recommended. The prompt is work-in-progress or superiority is not yet confirmed.
* ✅: Recommended. Heavily tested and superior to other versions.
* Base: When the prompt is a modification of another prompt, then "Base" refers to the original prompt.

## Installing Ace

*Note: All recommended prompts are located in `current`, all others are located in `archive`.*

The JSON files provided in this repository are made by/for `Open WebUI`.  
In order to use the Prompts you must install Ollama, `Open WebUI` and download the respective models.  
Then in `Open WebUI` go to `Workspace` > `Models` and click `Import Models` and select the prompt files you want.

## Using Ace elsewhere

You want to use Ace Prompts elsewhere?  
Thankfully that is VERY easy.

1. Open the respective TXT file of the Prompt you want.
2. Copy the complete prompt text
3. Paste the Prompt into the `System Prompt` text input of your respective LLM Chat solution.

## Naming

The name `Ace` was chosen at random with the goal of having a short name that is at the top of alphabetically sorted lists.

Because `Ace` was initial for Gemma-only, I decided to use a single-letter suffix for alternative models.  

List of currently used suffix:  
* `W` for IBM Granite, in reference to `IBM watsonx` the current AI suite and `IBM Watson` the "original" AI from 2011.

## License

Copyright 2025 Thomas Obernosterer  
Licensed under the MIT License.

See the LICENSE file for a copy of the full license.

### Google Noto Color Emoji

Copyright 2021 Google Inc. All Rights Reserved.  
License: https://fonts.google.com/noto/specimen/Noto+Color+Emoji/license

I use Noto Color Emoji for the Profile Images of the Prompts.  
