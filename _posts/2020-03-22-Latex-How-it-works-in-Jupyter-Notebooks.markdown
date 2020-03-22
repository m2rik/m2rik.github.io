Latex - How it works in Jupyter Notebooks
1 Get your Jupyter Notebooks as Latex output
1.1 Install Miktex - Download Link: https://miktex.org/download
 check if its on path from cmd using: tex version
1.2 Use the code below for a pdf-output with cells
 `jupyter nbconvert --to pdf latex.ipynb`
1.3 Use the code below for a pdf-output with no cells
`jupyter nbconvert --to pdf latex.ipynb --no-input`
1.4 Using a custom template
Steps

Create .tpl file
`import in cmd using --template=yourtemplate.tpl
jupyter nbconvert --to python 'example.ipynb' --stdout --template=simplepython.tpl`

1.5 Export your template from your ipynb file using:
`jupyter nbconvert --to pdf --TemplateExporter.exclude_input=True my_notebook.ipynb jupyter nbconvert --to markdown my_file.ipynb --template="mytemplate.tpl"`

1.6 Edit Titles from Miktex Latex editor
Steps

Open your .tex file in the Miktex viewer
Go to /maketitle and delete it
Insert the Statement: `\begin{title} \begin{center} \Large\textbf{Your Text}\ \large\textit{Your Text 2} \end{center} \end{title}`
1.7 To create an internal clickable link in the same notebook:
Steps

Create link To some Internal Section
Create destination `
