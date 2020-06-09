#  This is a markdown file
# What is R-Markdown?
It is a script-based text-development platform for preparing high-quality papers and reports. This strong tool is effective for use on complicated documents that have various types of diagrams and tables. R-Markdown is a distribution of Markdown language for R. More information about Markdown can be found here.
Personally, I’ve found R-Markdown to be a powerful tool for creating tutorial documents that include figures, tables, blocks of code, and more. R-Markdown can also be very helpful for working on papers; you can have everything in the same place. For example, as you will see in this tutorial, you can generate your figures and tables within documents. Because it is script-based, R-Markdown is reproducible; you will always get the same text format and figure quality. Therefore, if you want to have a professional-looking CV or are working on a paper or report, I suggest giving R-Markdown a try. The tool might become your new best friend.

# install R Markdown
 # There are two steps to install R-Markdown:

# 1- Install R Markdown
```{r setup, include=FALSE}
install.packages("rmarkdown")
library(rmarkdown)
```
 
install.packages("rmarkdown")
library(rmarkdown)
# 2- You also need to install “tinytex”. You can use the following command to install and load “tinytex”

```{r setup, include=FALSE}
tinytex::install_tinytex()
library(tinytex)
```

# Create an R-Markdown Document
To create your first R-Markdown document, start by installing R-Markdown. Then, open the “File” menu, and click on “New File.” From the dropdown menu, select “R-Markdown.” Doing so will open an R-Markdown file in your RStudio. The file comes with very simple and informative instructions.

On a side note, I use RStudio, which is a popular and user-friendly integrated development environment (IDE) for R. You can find more information about it (here).

# Publish your document
The final format of your output document can be pdf, html, or word. To select your favorite output and generate your final document, click on “Knit,” which opens a dropdown menu. Select the output format—for example, pdf—and it will generate your document.

# Components of an R-Markdown Code
R-Markdown documents usually include meta-data, text, and code chunks. The following sections briefly describe the components, and more information can be found on R-Markdown’s website.

# Meta-Data
When generating documents, R-Markdown requires some initial information and instructions. These can include general data about the documents—for example, date, title, output format, and author’s name.

# Text
Text parts in R-Markdown follow the tradition of other document-markup languages such as LaTex (see here). However, R-Markdown is easier than LaTex. Basically, authors can use scripts to adjust document formatting. Many details can be listed about R-Markdown’s text-formatting commands, but I am not going to explain them in this short tutorial. These cheat sheets here and here provide enough information to get you started on writing an R-Markdown document. A few examples: #header creates headers, ‘[]()’ creates a hyperlink. You can use $ to insert equations (e.g. $y=ax^{2}+ bx +c$).

# Code Chunks
Different types of code chunks can be used in R-Markdown; the types depend on application of the code. You might want to show your code when you develop an instruction. You can also write a code solely for generating a figure, but you may not want to show the code itself. The following is a generated timeline figure of Michael Jackson’s life; you can see the code.

```{r setup, include=FALSE}
#You need to uncomment ``` lines
 
#```{r timeline}
 

 
library(timelineS)
timelineS(mj_life, main = "Life of steve",label.cex =   0.7)
 
#```
```
 
