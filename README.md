# Statistics
This repository contains scripts to run various statistical models include GLMs, 
GLMMs, and model averaging. Scripts are simplified with explanations and links 
to reference texts where relevant.

Currently, we have:

1. Hierarchical models or Mixed Models (GLMMs)

# How to access
Scripts are saved in the /scripts folder, and relevant datasets to run the examples 
are in the /data folder. If you download the entire repository and then open the 
Rproj file, all scripts should run (i.e. R will know where to look for the 
datasets). You just need to open the relevant script and begin. 

If you do not want to download the entire repository, find the required script 
in the /scripts folder and the matching dataset in the /data folder. The dataset should
be named with the same name as the script.

# How to add an analysis
If you would like to share an analysis, it is best to clone the respository, add
your files to the relevant folders, then merge back to github. 

You will need to prepare a script and a dataset to upload. It is recommended to 
simplify the dataset if possible to keep the file sizes small and so that it's 
easy for someone to understand the analysis. Make sure to:
1. Name your dataset the same as your script
2. Annotate your code well, including a description at the beginning
3. Include your name and date at the top of your script file
4. Add your analysis to the list above
5. Add relevant keywords to repository (click cog next to "About")

If you are adding an RMarkdown file with the html output, please add this to the
YAML header before you render so that all html outputs are saved in the same 
folder:

knit: (function(inputFile, encoding) {
  rmarkdown::render(inputFile, encoding = encoding, output_dir = "../docs") })
