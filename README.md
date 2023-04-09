# My_JupitorNoteBook

# Import necessary libraries
import nbformat
from nbformat import v4

# Create the notebook object
nb = v4.new_notebook()

# Create the cells
cell1 = v4.new_markdown_cell("# My Jupyter Notebook")
cell2 = v4.new_markdown_cell("*Riya Maria Roy*\nBCA")
cell3 = v4.new_markdown_cell("*I am interested in data science because it allows me to explore, analyze and derive insights from large datasets, and make data-driven decisions.*")
cell4 = v4.new_markdown_cell("### What does the code do?")
cell5 = v4.new_code_cell("Sum = 1 + 1\nprint(Sum)")

# Add the cells to the notebook
nb.cells.append(cell1)
nb.cells.append(cell2)
nb.cells.append(cell3)
nb.cells.append(cell4)
nb.cells.append(cell5)

# Save the notebook
with open("My Jupyter Notebook.ipynb", "w", encoding="utf-8") as f:
    nbformat.write(nb, f, version=4)
