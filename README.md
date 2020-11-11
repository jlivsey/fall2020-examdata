# Data for Fall 2020 Exam

You can load the data directly by sourcing the .R file

    library(devtools)
    source_url("https://raw.githubusercontent.com/jlivsey/fall2020-examdata/2c946058fa07972166f6a8aab3fad07cd895ea5b/data.R")

Or if this doesn't work you can load the .csv file and convert to a time series object

    library(RCurl)
    y <- getURL("https://raw.githubusercontent.com/jlivsey/fall2020-examdata/main/data.csv")
    z <- read.csv(text = y)
    x <- ts(z)
 
