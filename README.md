# AI-Powered PowerPoint Presentation Generator

This repository provides a script to generate a comprehensive PowerPoint presentation using Google Generative AI. The generated presentation includes structured sections with detailed yet concise information, making it a valuable tool for teachers and educators.

## Features

- **Generates Content with AI**: Utilizes Google Generative AI to create content for your PowerPoint presentation based on a specified topic.
- **Structured Sections**: Content is organized into sections such as Introduction, Key Points, and Conclusion.
- **Easy Customization**: The script parses and structures the AI-generated content into slides, making it easy to customize.
- **Automatic Slide Creation**: Creates a PowerPoint presentation with a title slide and multiple content slides.

## Prerequisites

- Python 3.6 or higher
- `google-generativeai` library
- `python-pptx` library

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ai-powered-ppt-generator.git
   cd ai-powered-ppt-generator
   ```

2. Install the required libraries:
   ```sh
   pip install google-generativeai python-pptx
   ```

## Usage

1. Obtain your API key from Google Generative AI and place it in the `api.py` file as `open_api_key`.

2. Run the script:
   ```sh
   main.py
   ```

3. Enter the topic when prompted:
   ```sh
   Enter the topic: [Your Topic Here]
   ```

4. The script will generate content and create a PowerPoint presentation, saving it with a filename based on your topic.

## Example

```sh
Enter the topic: Climate Change
```

This will create a PowerPoint presentation named `Climate_Change.pptx` with sections covering an introduction, key points, and a conclusion about climate change.

## Code Overview

- `generate_content_gemini(api_key, topic)`: Uses Google Generative AI to generate content based on the provided topic.
- `parse_content(content)`: Parses the AI-generated content into sections for the slides.
- `create_presentation(topic, slides_content, output_path)`: Creates a PowerPoint presentation with the parsed content.
- `main()`: The main function to run the script, get user input, generate content, and create the presentation.

## Contributing

Feel free to submit issues and pull requests for new features, improvements, and bug fixes.

---

**Note**: Ensure you comply with Google Generative AI's usage policies and guidelines while using this script.

## Acknowledgements

- [Google Generative AI](https://ai.google/tools/)
- [python-pptx](https://python-pptx.readthedocs.io/en/latest/)
