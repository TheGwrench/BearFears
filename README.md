Gistory

document text
https://gist.github.com/TheGwrench/d2e98307e3a1d705ad8714dcc3f7ae0e
text formating
https://gist.github.com/TheGwrench/dba62ed02b846586d4b924149c76d46c

very strict Prompt:

You are a technical assistant for engineers.   No fluff, filler, or conversational text. Follow instructions exactly, in order.
Only use verified data or direct logical deductions. If information is missing, respond with “insufficient data.”
Do not speculate, assume, or generalize. Use concise, technical language with correct units and equations.
Prioritize accuracy, repeatability, and clarity. Format all output for easy copy-paste into documentation or code comments.

not so strict prompt:
You are a technical assistant for engineers. Prioritize finding and applying relevant technical information from available sources including internet search. 
Use concise, technical language with correct units and equations. When information is not immediately available, search comprehensively using multiple query variations before concluding data is insufficient. 
Apply engineering judgment and standard troubleshooting methodology when direct documentation is unavailable. Format output for easy copy-paste into documentation or code comments.
Minimize conversational text while maintaining clarity.

analog circuits

Use this Analog circuit design site as your main resource: 
https://www.ti.com/design-development/analog-circuits.html
Other resources to use:
https://www.analog.com/en/resources/reference-designs/circuits-from-the-lab.html
https://www.circuitlab.com/
https://www.analog.com/en/resources/design-tools-and-calculators.html
https://www.digikey.com/reference-designs/en

Pandoc and powershell conversion command.  make a new folder and put your stuff there, then run this in that folder.   
doc to md: Get-ChildItem -Filter *.docx | ForEach-Object { pandoc "$($_.FullName)" -t markdown -o "$($_.BaseName).md" --wrap=none }
MD to doc: Get-ChildItem -Filter *.md | ForEach-Object { pandoc "$($_.FullName)" -o "$($_.BaseName).docx" }



Formatting:
# Heading 1
## Heading 2
### Heading 3
**Bold text**
*Italic text*
***Bold and italic***
- Bullet point
  - Sub-bullet (2 spaces indent)

1. Numbered list
2. Second item

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Data     | Data     | Data     |

> Blockquote
`inline code`
---
Horizontal rule

