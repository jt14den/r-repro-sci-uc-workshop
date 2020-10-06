# Episode data types 
## download and read file in
download.file("https://raw.githubusercontent.com/swcarpentry/r-novice-gapminder/gh-pages/_episodes_rmd/data/gapminder_data.csv", destfile = "data/gapminder_data.csv")
gapminder <- read.csv("data/gapminder_data.csv")

## read in file from web
gapminder <- read.csv("https://raw.githubusercontent.com/swcarpentry/r-novice-gapminder/gh-pages/_episodes_rmd/data/gapminder_data.csv")

str(gapminder) #str stands for structure 
# what is this
View(gapminder) #to look at it in a tab 

## Data types 

typeof(gapminder$year)
typeof(gapminder$lifeExp)
typeof(3.14)
typeof(TRUE)  # logical 
typeof('bannana')
class(gapminder)
typeof(gapminder$continent)
typeof(gapminder$country) #character

## Vectors 
## TODO  - dunno what to do here yet

## Data structures = realistic example 
str(gapminder)
summary(gapminder$country)
# What happened here? 
?summary
summary(gapminder$country) # tell us lenght of character vector 
#but we want a diff summary, we'd lke to count up the occurances of our country 
#to do this we need to convert the country vector to a factor
#what's a factor? categorical variable, e.g. colors, breeds of dogs 
factor(gapminder$country)
#note at the end, we can see 142 levels (or categories)
#let's add this to our summary; how? 
summary(factor(gapminder$country))

typeof(gapminder$year)

typeof(gapminder$country)
str(gapminder$country)
str(factor(gapminder$country))
length(gapminder)
typeof(gapminder)
# what's a list?? a data structure 
nrow(gapminder)
ncol(gapminder)
dim(gapminder)
colnames(gapminder)
head(gapminder)


## Subsetting DFs
### bracket notation - if we use a single bracket with number, it will return
### single column as a dataframe
head(gapminder[3])

### however if we use [[3]] it'll return the column as a vector 
head(gapminder[[3]])
head(gapminder[["lifeExp"]])
# $ dollar sign can pull out a column by name 
head(gapminder$year)
# we can pull out by rows and columns by using two arguments in []
gapminder[1:3,] #row 1-3 and all columns
gapminder[3,] #   
gapminder[3:10, 1:3]

# let's subset gapminder and only include data from 87
gapminder[gapminder$year == 1987, ]
# how about population greater than 15,000,000
gapminder[gapminder$pop >= 15000000,]







