# Llama 3.2-3B Instruct

This project demonstrates the use of the AI (Llama 3.2-3B) model for extracting metadata from academic articles.

## Project Structure

- `Llama_3_2_3B_Instruct.ipynb`: Jupyter notebook demonstrating the use of the Llama 3.2-3B model.

## Usage

1. Clone the repository:
    ```sh
    git clone https://github.com/recepdemrci/rpa-knowbot.git
    cd rpa-knowbot
    ```

2. Open the Jupyter notebook:
    ```sh
    jupyter notebook src/Llama_3_2_3B_Instruct.ipynb
    ```

3. Replace HUGGINGFACE_TOKEN with your token

4. Run the cells in the notebook to extract metadata from academic articles.

## Functions

### `pdf_to_text(filepath)`

Converts a PDF file to text.

**Parameters:**
- `filepath` (str): Path to the PDF file.

**Returns:**
- `str`: Extracted text from the PDF.

### `text_to_json(text)`

Converts text to JSON format.

**Parameters:**
- `text` (str): Text to be converted.

**Returns:**
- `dict`: JSON representation of the text.

### `set_prompts(texts)`

Sets prompts for the Llama model.

**Parameters:**
- `texts` (list): List of texts.

**Returns:**
- `list`: List of prompts.

### `generate_outputs(prompts, batch_size)`

Generates the metadata of PDF article using prompts.

**Parameters:**
- `prompts` (str): Prompt of the extracting pdf

**Returns**
-`str`: Generated outputs