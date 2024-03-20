# Word Search Generator

This Python script generates a word search puzzle from a list of words. The puzzle is then exported to a PDF file.

## Requirements

- Python 3
- fpdf

## Usage

1. Replace the `filename` variable with the path to your input file containing the list of words.

```python
g = Generator("path_to_your_word_list.txt")
```

2. Call the export_to_pdf method with the desired title, lines, and grid_font for your PDF.

```g.export_to_pdf("desired_title", number_of_lines, grid_font_size)
```

3. Run the script.
```python main.py
```

This script performs the following steps:

1. Reads the list of words from the input file.
2. Generates a grid of a suitable size based on the length and number of words.
3. Randomly inserts each word into the grid in a horizontal, vertical, or diagonal orientation.
4. Fills the remaining spaces in the grid with random letters.
5. Exports the grid and the list of words to a PDF file.
The output is a PDF file with a word search puzzle that can be printed out and solved.
