# Heinze-Final-
My Sports group descriptive table from R code 
library(readr)
data <- read_delim("data.csv")
dim(data)
names(data)
summary(data)
#descriptive statistics table 
#age
mean(data$age)
sd(data$age)
min(data$age)
max(data$age)
#minutes
mean(data$mpg)
sd(data$mpg)
min(data$mpg)
max(data$mpg)
#linear regression
linear_model <- lm(mpg ~ age, data = data)
summary(linear_model)

linear_plot <- plot(data$age, data$mpg)
print(linear_plot)
