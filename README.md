# Ace Prompts

## Ace for Gemma 3

`Ace for Gemma 3` is a collection of system prompts for Google's Gemma 3 LLM.  
The prompts have been constructed in a way to make Gemma a helpful assistant and provide accurate and detailed information according to its guidelines.

### Ace Glasses

`Ace Glasses` is a prompt that is optimized for describing any image.

The current recommended version of `Ace Glasses` is `v1.3`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | ❌            | Refuses to provide a general description of images with violating content. |
| v1.1    | v1.0 | ✅            | Describes everything AROUND the violating content OR can describe the content using harmless language. |
| v1.2    | v1.1 | ❌            | Was instructed to wiggle the rules a bit to describe violating content, instead it provides a less descriptive result as v1.1 that is not helpful. |
| v1.3    | v1.1 | ✅            | Instructed to provide an objective interpretation of guideline violating content. Better responses on followup instructions. |

### Ace Scientist

`Ace Scientist` is a prompt that makes Gemma a helpful online search assistant.  
In order to use Ace Scientist, the model needs to be able to search the internet.

The current recommended version of `Ace Scientist` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | ✅            | Instructed to search the web and to provide up-to-date and correct information. |

### Ace Alchemist

`Ace Alchemist` is a prompt that makes Gemma a helpful database expert.

The current recommended version of `Ace Alchemist` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | ✅            | Instructed to provide correct information, document and explain the outputs, keep things simple, cite documentation when possible |

## Installing Ace

*Note: All recommended prompts are located in `current`, all others are located in `archive`.*

The JSON files provided in this repository are made by/for `Open WebUI`.  
In order to use the Prompts you must install Ollama, `Open WebUI` and the `gemma3` model.  
Then in `Open WebUI` go to `Workspace` > `Models` and click `Import Models` and select the prompt files you want.

## Using Ace elsewhere

You want to use Ace Prompts elsewhere?  
Thankfully that is VERY easy.

1. Open the respective TXT file of the Prompt you want.
2. Copy the complete prompt text
3. Paste the Prompt into the `System Prompt` text input of your respective LLM Chat solution.

## License

Copyright 2025 Thomas Obernosterer
Licensed under the MIT License.

See the LICENSE file for a copy of the full license.

### Google Noto Color Emoji

Copyright 2021 Google Inc. All Rights Reserved. 
License: https://fonts.google.com/noto/specimen/Noto+Color+Emoji/license

I use Noto Color Emoji for the Profile Images of the Prompts.  
