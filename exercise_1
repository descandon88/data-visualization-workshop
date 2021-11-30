
library(ggplot2)
library(RColorBrewer)
library(forcats)

ff <- 'https://www.dropbox.com/s/k9q8ee65vnxngzb/indiana.csv?dl=1'
download.file(ff, destfile = 'indiana_data.csv')
indiana <- read.csv('indiana_data.csv')

str(indiana)

ggplot(data = indiana, aes(x=annual_inc,y=loan_amnt)) + 
  geom_point() + theme(aspect.ratio=1)

"ploting by adding color according to term variable"
ggplot(data = indiana, aes(x=annual_inc,y=loan_amnt, color=term)) + 
  geom_point() + theme(aspect.ratio=1)

"ploting by adding shape according to  term variable"
ggplot(data = indiana, aes(x=annual_inc,y=loan_amnt, shape=term)) + 
  geom_point() + theme(aspect.ratio=1)

"ploting by sizing according to dti variable"

ggplot(data = indiana, aes(x=annual_inc,y=loan_amnt, size=dti)) + 
  geom_point(alpha = 1 / 3) + theme(aspect.ratio=1)
