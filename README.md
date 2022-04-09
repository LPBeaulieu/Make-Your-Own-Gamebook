# Make Your Own Gamebook
This app lets you create your own gamebook, without the hassle of assigning the random section numbers yourself!

![Image RTF basic mode](https://github.com/LPBeaulieu/Make-Your-Own-Gamebook/blob/main/Make%20Your%20Own%20Gamebook%20Image.jpg)
<h3 align="center">Make Your Own Gamebook</h3>
<div align="center">
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/LPBeaulieu/TintypeText/blob/main/LICENSE)
  [![GitHub last commit](https://img.shields.io/github/last-commit/LPBeaulieu/TintypeText)](https://github.com/LPBeaulieu/TintypeText)
  [![GitHub issues](https://img.shields.io/github/issues/LPBeaulieu/TintypeText)](https://github.com/LPBeaulieu/TintypeText)
  
</div>

---

- <b>Make Your Own Gamebook</b> allows you to create your very own interactive gamebook, where readers choose how to engage with characters and events they encounter as the story unfolds. 
- All you need to do is keep tabs on your section names in the section title headers and references throughout the text, and the Python code takes care of all the nitty-gritty details of assigning the numbers and sorting your document for you! 
- The code even checks for spelling mistakes in the section titles and lets you know if you have duplicates. 
- Importantly, it verifies that the last section can be accessed from the first section without interruption (that is to say, it checks for contiguity) and lets you know the furthest section that it is able to reach in your unsorted original document. This helps you figure out where there are issues as you are writing your work. 
- Text documents or rich text format (RTF) documents may be used with the code, and you can even feed the code the RTF document from the TintypeText typewriter optical character recognition application (See the TintypeText github repository: https://github.com/LPBeaulieu/Typewriter-OCR-TintypeText)

## 📝 Table of Contents
- [Important Pointers](#Important_Pointers)
- [Getting Started and Usage](#getting_started)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## ⛓️ Important Pointers <a name = "Important_Pointers"></a>
- Every section within the document should bear a unique name, using a “** Section” opening tag and closing asterisks ( ** ), as exemplified by the following section title header: “** Section Exploration of the Caves **”.
- The same section titles, without the opening tags or asterisks, but preceded by “turn to” and followed by a period (for example: “turn to Exploration of the Caves.”) will be used throughout the section texts to refer to the the appropriate section title headers.
- It must be emphasized that the presence of <b>two consecutive asterisks before</b> (within the “** Section”  tag) <b>and after the section title header</b> is required in order to locate the section titles within the text. Furthermore, <b>a period is needed after a section title reference</b>, so as to indicate the end of the random index (so that “turn to 1” is not confused with “turn to 11”, for instance).
- All of the <b>section title headers</b> (for example: “** Section Exploration of the Caves ** ”), and <b>section title references</b> (for example: “turn to Exploration of the Caves.”), need to be <b>spelled the exact same way</b> to ensure correct random index substitutions.
- Also, you should <b>avoid putting any text before the first section or after the last section</b>, as this text would be lost after splitting the document into individual sections. You should instead write separate foreword and afterword documents that will not be submitted to the present code.
- It is all the more important to <b>check for typos and omitted asterisks in the first section opening tag</b> (“** Section”), as if the second section opening tag is correctly written, such mistakes in the first section would result in its exclusion from the list of sections.
- You should <b>avoid non-directional double quotes ( " )</b> when writing your “.txt” document on your computer, as these characters are omitted in the RTF file. Documents should be redacted in a word processor that uses directional quotes and be saved in “.txt” or “.rtf” format.

## 🏁 Getting Started and Usage<a name = "getting_started"></a>

Here is a link to an instructional video how to setup and use <b>Make Your Own Gamebook</b>:.

The paths included in the code are formatted for Unix (Linux) operating systems (OS), so the following instructions are for Linux OS environments.

<b>Step 1</b>- Create a virtual environment (called <i>env</i>) in your working folder:
```
python3 -m venv env
```

<b>Step 2</b>- Activate the <i>env</i> virtual environment <b>(you will need to do this step every time you use the Python code files)</b> 
in your working folder:
```
source env/bin/activate
```

<b>Step 3</b>- Install the required <b>SpellChecker</b> module (https://pypi.org/project/pyspellchecker/) to spellcheck the section titles:
```
pip install pyspellchecker
```

<b>Step 4</b>- You're now ready to use <b>Make Your Own Gamebook</b>! 

Be sure to check out the Youtube video (see link above) for instructions on how to use the Python code files. You can now easily create your very own gamebook in a few seconds, without all the hassle of assigning random section numbers yourself! 🎉📖 
  
## ✍️ Authors <a name = "author"></a>
- 👋 Hi, I’m Louis-Philippe!
- 👀 I’m interested in natural language processing (NLP) and anything to do with words, really! 📝
- 🌱 I’m currently reading about deep learning (and reviewing the underlying math involved in coding such applications 🧮😕)
- 📫 How to reach me: By e-mail! LPBeaulieu@gmail.com 💻


## 🎉 Acknowledgments <a name = "acknowledgments"></a>
- Hat tip to [@kylelobo](https://github.com/kylelobo) for the GitHub README template!

<!---
LPBeaulieu/LPBeaulieu is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
