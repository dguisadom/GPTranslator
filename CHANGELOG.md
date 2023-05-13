#GPTranslate changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [0.8.0-alpha] - 2023-05-13

### Changed

- Chat completion prompt changed to reduce tokens usage maintaining same results.
- context.txt example changed to add more examples about how to get more hints to the model in order to inprove translations.
- Now header values are related to config variables
- Requirements.txt add new required libs

### Added

- After translation, the script ask to confirm translations that have sensibly diferent size from the original text.
- config.json file to maintain global configuration object

### Fixed

- Fixed version number to adheres to Semantic Versioning
 

## [0.7.0-alpha] - 2023-05-12

### Added

- Command-Line Interface: GPTranslate is now equipped with a command-line interface, allowing users to run the tool directly from the console. This makes it easy to integrate GPTranslate into scripts and automated workflows.

- JSON Input: The tool now supports reading JSON files as input. It can recursively traverse the JSON structure and translate all string values. GPTranslate can handle JSON objects, arrays, and primitive types efficiently.

- Target Language Support: GPTranslate now supports translation into multiple target languages. Users can specify the target language using the ISO 639-1 language code. GPTranslate covers all ISO 639-1 language codes, providing flexibility for translation needs.

- Contextual Translation: To ensure accurate translations, GPTranslate now supports contextual translation. Users can provide a description of the technical context, including language type, technical terminology, language context, and even forced translations or the meaning of specific acronyms. This contextual information helps improve the accuracy of the translations.
Prompt Injection Protection: GPTranslate now incorporates prompt injection protection to maintain the integrity of input and output data. This security feature safeguards against any malicious or unintended modifications during the translation process.

- OpenAI API connection: Conected to open AI chat completion API to get the text translations