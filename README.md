# Take the survey!
I would truly appreciate if you could give us some feedback on the workshop. It only takes a few minutes. You can find the link here: https://forms.gle/EQcxdnHzaiKYEuXY7

# APS-2023-MGS
Welcome! If you've made it to this site, it means you're enrolled in the pre-meeting metagenomics workshop held at APS 2023. This page will serve as your one-stop shop for this workshop. Here, you will find links to download programs, lines of code that you will copy, and much more. 

You should have recieved an email from the Ohio Supercomputer (OSC) about signing up for an account. Please follow those instructions and gain access to an account as soon as you can, since that link expires. Almost all of the workshop will take place on the OSC, so it is crucial for you to sign up for an account. 

Lastly, it is incredibly important for you to bring your computer to the workshop, as this workshop relies on indivudal computers. 

## Things to download on your computer
Most of this workshop will take place on the OSC, but there are a few times you will need to use a program downloaded to your computer. 

### R and Rstudio
We will use Rstudio for part of the course. You can download them at: https://cran.rstudio.com and https://posit.co

This guide is a comprehensive walk-through of downloading both: https://teacherscollege.screenstepslive.com/a/1108074-install-r-and-r-studio-for-windows

### Mauve
Mauve is a genome alignment viewer, and can be a super cool tool to compare similar genomes! You may have the opportunity to work with it during this course. You can download it here: https://darlinglab.org/mauve/mauve.html

## During the course
Here, you will find resources you may need during some of the steps or if you finish a step early!

### If you finish Kraken early...
Check out all the databases that Kraken offers: https://benlangmead.github.io/aws-indexes/k2
Which database do you think we're using?
What database do you think you would use if you ran Kraken?
What would include in your custom database if you were to use Kraken with your own data?

### Pavian

You will need the following lines of code for Pavian. 

This line installs Pavian into your Rstudio
```bash
if (!require(remotes)) { install.packages("remotes") }
remotes::install_github("fbreitwieser/pavian")
```
This line will open the Pavian interface
```bash
pavian::runApp(port=5000)
```

https://fbreitwieser.shinyapps.io/pavian/

### If you finish Pavian early...
Check out the table format of pavian! The Sankey diagrams are super cool, but there is a table version of all the data from Kraken. It is found under "Results Overview." 

### Extract Reads
We will need to install an envrionment to your terminal. Navigate to your programs directory within your home directory, and find the file labeled "all-prgms.yml" Click open in terminal and paste the following text.
```bash
conda env create -f all-prgms.yml
conda activate all-pgrms
conda lis
```

### If you finish extracting your reads early...
Try extracting reads from a different genus or a higher taxonomic order! Find a different taxonomy ID from NCBI and run extract reads. Compare file sizes between your different outputs and see which has the most data.

### If you finish metaSPAdes early...
Try blasting a portion of your genome on NCBI! Blasting the entire genome may take a while, but blasting different portions may yield some cool results. 

### If you finish pyani early...
You can download some other NCBI genomes from NCBI and try those out in pyani! I downloaded a very small amount. Be careful - pyani can take a long time if you add too many. 

There is some really neat R code that can transform your pyani output into a phylogentic tree, and where you can change the percent identity scale. 

## Programs used during the workshop
You can find all of the programs we used here. You can read all about them at the links provided below.

Kraken2 - https://github.com/DerrickWood/kraken2 and https://ccb.jhu.edu/software/kraken2/
We use both kraken2 and Kraken tools. Kraken tools has the extract feature in it, which we utilized in our workshop. 

Pavian - https://github.com/fbreitwieser/pavian

SPAdes - https://github.com/ablab/spades
We use the --meta argument to utilize SPAdes as a meta-genome assembler.

Pyani - https://github.com/widdowquinn/pyani
