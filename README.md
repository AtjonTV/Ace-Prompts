# Ace Prompts

## Ace for Gemma 3

`Ace for Gemma 3` is a collection of system prompts for Google's Gemma 3 LLM.  
The prompts have been constructed in a way to make Gemma a helpful assistant and provide accurate and detailed information according to its guidelines.

### Ace Glasses

`Ace Glasses` is a prompt that is optimized for describing any image.  
With the prompt Gemma does not refuse to describe images that contain guideline-violating content, it simply ignores it and describes everything around such content.

The current recommended version of `Ace Glasses` is `v1.3`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | No           | Refuses to provide a general description of images with violating content. |
| v1.1    | v1.0 | Yes          | Describes everything AROUND the violating content OR can describe the content using harmless language. |
| v1.2    | v1.1 | No           | Was instructed to wiggle the rules a bit to describe violating content, instead it provides a less descriptive result as v1.1 that is not helpful. |
| v1.3    | v1.1 | Yes          | Instructed to provide an objective interpretation of guideline violating content. Better responses on followup instructions. |

### Ace Scientist

`Ace Scientist` is a prompt that makes Gemma a helpful online search assistant.  
In order to use Ace Scientist, the model needs to be able to search the internet.

The current recommended version of `Ace Scientist` is `v1.0`.

Available versions:

| Version | Base | Recommended? | Description |
|---------|------|--------------|-------------|
| v1.0    |      | Yes          | Instructed to search the web and to provide up-to-date and correct information. |

## Installing Ace

*Note: All recommended prompts are located in `current`, all others are located in `archive`.*

The JSON files provided in this repository are made by/for `Open WebUI`.  
In order to use the Prompts you must install Ollama, `Open WebUI` and the `gemma3` model.  
Then in `Open WebUI` go to `Workspace` > `Models` and click `Import Models` and select the prompt files you want.

## License

Copyright 2025 Thomas Obernosterer
Licensed under the MIT License.

See the LICENSE file for a copy of the full license.
