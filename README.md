# Project 02 Proposal: <your project title>

**Team members:** Joseph Callaway 

See the [Project 02 instructions](https://data385.github.io/project/proj02_wholegame.html) for what goes in each section. Bullet points are great. Put any images in an `img/` folder.

## 1. Problem statement

_Who has the problem, what decision or need it involves, why it matters, and what you expect to find._

The problem is crime but how do people avoid being victims and are there other factors that make someone more likely to be a victim. Ultimately it matters because cities can be dangerous places odds are people do not want to be on the receiving end of any foul play. My expectations are age, sex, location and offense type and maybe time of year might be revealing in the answering of this question.

## 2. Research question

_A clear association between a response and at least one predictor variable._

What factors such as age,sex, area, corrolate with likely-hood of being a victim of crimes in Los Angeles and are there any particular crimes that correlate more with one of these factors?

## 3. Data acquisition

_In 1-2 sentences, describe the data you intend to collect and how you will get it._


### a. Confirm viability

_Scraping: summarize the "Before You Scrape" checklist. Downloading: citation, link to the documentation, and how the data were originally collected. Collecting it yourself: how you are collecting it and where you are storing it._


### b. Variables of interest

_If you do not have the data yet, list the variables you plan to collect and the exact question text. Include 1) the variable name, 2) data type 3) description. Use bullet points._

3.Data has bee sourced from data.gov sourced from these particular pages: https://catalog.data.gov/dataset/crime-data-from-2020-to-present?from_hint=eyJxIjoibG9zIGFuZ2VsZXMgY3JpbWUifQ%3D%3D
https://catalog.data.gov/dataset/crimes-one-year-prior-to-present
https://catalog.data.gov/dataset/nypd-arrest-data-year-to-date?from_hint=eyJxIjoiY3JpbWUgIiwic29ydCI6InJlbGV2YW5jZSIsIm9yZ190eXBlIjoiQ2l0eSBHb3Zlcm5tZW50Iiwib3JnX3NsdWciOiJueWMtbnkifQ%3D%3D
The sites robots.txt poses no issue with downloading this set. The variables I believe to be of interest are Area Name, Vict Age and Sex, Premise Desc, Status Desc, and DATE OCC.

## 4. Data example

_Scraping: a URL and an annotated screenshot. Downloading: a link to your rendered `data_management.pdf` with `glimpse()`. Collecting: a screenshot of one example row._
linking to a Quarto Document Render to show the Glimpses of currently collected data
see[here]("Proposal.pdf")

## 5. EDA

_The techniques and functions you plan to use to import, wrangle, visualize, and explore the data, and why each is needed._

In terms of techniques I will use, I am anticipating using ymd() with the current set of data I have and potentially parse_number() depending on subsequent sets I shall acquire. Wrangling functions like filter(), select(), arrange(), mutate() and count() I can almost guarantee shall be a used in one way or another. If not all then most. Recode, I I could see case_when statement to modify the data to my specifications. Factors I could maybe see myself using if I wanted to label severity of crimes but I don't see myself using those as much. Join, assuming the datasets are sufficient on their own I don't see myself using these as much. Reshape is a simliar story as well. Functions are something I could potentially see myself using as well. ggplot is a given as well as it's visualizations of distribution will prove useful.

## 6. Modeling

_The models you plan to use, your response and predictor variables, and why the models fit your research question._

Some of the variables I am using are going to be factorial but variables such as age and date might be compatible with a linear model as those shall actively show change over time. date might be tricky because I can imagine peaks and valleys IF season does have a factor. Explanatory variables include sex,age, premise description, location and response variable is a row on the dataset.

## 7. Communicate

_How you plan to present your results (website, poster, or short slide presentation)._

I intend to communicate results via a website, it will allow the results of each individual city to show assuming there are significant differences and leave other pages for comparison open


## 8. LLM disclaimer

_Whether and how you will use AI tools: the specific tool, its use, and your data protection methods. If you won't use any, say so._

I hope to not use LLMs (Coding agents are counter productive to me learning Rstudio so they are a massive no) but if I cannot find a solution to a given problem it shall be my last result to find an issue to a problem as a browser search serves the same function for me. If I am going to, I shall try and make an effort to mark any instances of LLM's.