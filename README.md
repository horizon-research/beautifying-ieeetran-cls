# Beautifying IEEEtran.cls
Making IEEEtran.cls a little less ugly.

The initial commit has the original IEEEtran.cls, which apparantly is version 1.7a (2007/03/05). So comparing against that commit would tell you what's been changed. Lines with a ```%LessUgly``` comment are where changes are. Briefly, here is a list of changes:

* Section/Subsection/Subsubsection titles are bolded.
* Subsection title numberings start with the section numbering. For instance, subsection **B** under Section **IV** would be **IV-B**. Originally, the section numbering is omitted.
* Subsubsection title numberings start with the section and subsection numberings. For instance, subsubsection **3** under subsection **B** and Section **IV** would be **IV-B.3)**. Originally, the subsection and section numberings are omitted.
* The hypen (-) after **Keywords** is replaced with an em-dash (---) for V1.6.
* An **Artifact** section is added. You can now add your artifact information using: ` \begin{Artifact} something-about-your-artifact \end{Artifact} `. This can be put right after the Keywords section.

A few disclaimers:
* Use at your discretion.
* It's created mainly for conferences in computer architecture/systems (e.g., ISCA/MICRO/ISPASS) that sometimes have to use the IEEEtran template. When using the IEEEtran template, these conferences usually choose the compsocconf class option (IEEE Computer Society conferencs, or CPS). So most of the "beautifying" edits are for that class.
