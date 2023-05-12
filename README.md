
# GPTranslate

GPTranslate is a command-line tool for translating JSON files, using the power of the OpenAI language model. The tool reads a JSON file, a target language, and a context description, and outputs a JSON file that has been translated into the target language.

## Features

- Command-Line Interface: GPTranslate is designed to be run from the console, making it easy to integrate into scripts and automated workflows.

- JSON Input: The tool reads a JSON file, recursively traversing the structure and translating all string values. It can handle JSON objects, arrays, and primitive types.

- Target Language: You can specify the target language for the translation using the ISO 639-1 code. GPTranslate supports all ISO 639-1 language codes.

- Contextual Translation: Along with the JSON file and target language, you can also provide a description of the technical context. This context can include the type of language, technical words, language context, and even forced translations or the meaning of specific acronyms. This helps ensure the accuracy of the translations.

- Prompt Injection Protection: GPTranslate is designed with protection against prompt injection, ensuring that the integrity of your input and output data is maintained.

In some languages, the translation of a word can change significantly depending on the context. For example, the word "load" could be translated differently in a logistics context compared to an electronics context. Thanks to the context prompt feature, you can instruct the model to take into account these differences in language.

## Usage

Run GPTranslate from the command-line, providing the path to the JSON file, the target language, and the path to a .txt file containing the context description:

    bash 
    python gptranslate.py --json_path path/to/file.json --target_language es --context_text_file path/to/context.txt

If you run GPTranslate without any arguments, it will prompt you to enter the necessary information:

    bash 
    python gptranslate.py

You will be asked to provide:

- the path of the JSON file.
- The target language (ISO 639-1 code).
- The path to a .txt file containing context text for the translation.

## Installation

To install the necessary dependencies, run:

bash pip install -r requirements.txt A

## Requirements

- Python 3.6 or higher
- requests
- openai

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.