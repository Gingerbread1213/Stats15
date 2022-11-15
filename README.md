git add .
git commit -m " "
git push

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"




tydiverse()
  Select()
    contains()
   (when the col name contains the word)

   starts_with()
   (when the col name starts with the word)

    end_with()
    (when the col name end with the word)

   last_col
   (grab last col)
    
  
  
    select(-x)
    (take the col x out)

    select(new_name = old_name)
    (rename the col when selecting the col)
   
   
dplyr()
  anti_join()
  (Filter out that table A doesn't has item similar to table B)
  
  bind_rows()
  (combine two table by rows)

  count()
  (# of each items in the col)

  filter()
  (filter out the specific value we want from the col
  (to filter out multiple items, we use "data %in% c("x","y","z")")
  )

  full_join()
  (Keep all)

  left_join()
  (Keep first, replace second)

  group_by()
  (organize the data by groups)

  inner_join()
  (Join the like term)

  is.na(x)
  (find out if there is NA in col x)

  rename(new_name = old_name)
  (rename)

  right_join()
  (Keep second, replace first)

  replace_na(x)
  (Replace all na with x)

  semi_join()
  (Filter out that table A has item similar to table B)

  transmute()
  (mutate a col when select some col and will drop another col)

  year()
  (figure out the exact year from a [date] type)



Statistic
  abs()
  [absolute value]

  dbinom(x,y,z)
  [x = # of success, y = # of trial, z = probability of success, probability mass function]

  mean()
  
  median()
  

  punif(n, min = n, max = n)
  [calculate the probability event occur less than n , uniform]
  
  pbinom(x,y,z, lower.tail = TRUE)
  [x = # of success, y = # of trial, z = probability of success, cumulative distribution function]
     
 
  pnorm(n , mean = x, sd = y, lower.tail = TRUE )
  [n = probability of success, cumulative normal distribution function]

  qnorm(p, mean = x, sd = y, lower.tail = TRUE)
  [n = probability of success, calculate the exact value of the sample]
  quantile()
    probs = c(x)
    [give it in percentage form]
    probs = seq(0,1,0.2)
    [seq(from, end, step)]
  
  quantile(x,0.25) - 1.5*(quantile(x,0.75)-quantile(x,0.25))
  quantile(x,0.75) + 1.5*(quantile(x,0.75)-quantile(x,0.25))
  [state that the value is a outlier]

  runif(n, min = n, max = n)
  [take n samples, between n to n]
  
  rbinom(x,y,z)
  [x = trial, y = number of "coin", z = probability of success, random binomial simulation]

  replicate(n, X)
  [repeat the process X, n times]
  
  sample_n(int)
  [take int amount of sample from the population]
    replace = TRUE
    [take sample with replacement]
  
  set.seed(int)
  [to take the same sample every single time]

  sum((total - mean(total))^2)/x
  var()
  [variance]
  
  sqrt(var())
  sd()
  [std]
 

ggplot()

  geom_bar()
    position = "stack"
    
  geom_col()
    
  geom_point()
    position_jitterdodge(jitter.width = , dodge.width =, alpha = )
    [set the width of the overlap, alpha means transparency]
  
  geom_line()
  
  geom_histogram()
    (please note that there will only be X appeal in the aes() )
    ..x..
    (".." notation shows the relative frequency1)
    
  theme()
    legend.position = "none"
      [close the legend]
    axis.ticks = element_blank()
      [element blank = none or FALSE,
       which means to remove the ticks]
    axis.title = element_text()
      [set title]
    axis.text = element_text()
      [set text]
    linetype = ""
      [set linetype]
    
  geom_segment(aes(xend = 30, yend = country), size = 2) 
    (draw the graph by segment)
    
  geom_text(aes(label = round(lifeExp,1)), color = "white", size = 1.5) 
    (put labels on the graph, round() will set the point shape of the graph)
    
  scale_x_continuous("", expand = c(0,0), limits = c(30,90), position = "top") 
    (set the window of x)
    
  scale_color_gradientn(colors = palette) 
    (set the color of the scale)
    
  labs(title = "Highest and lowest life expectancies, 2007", caption = "Source: gapminder" )
    (label the title and caption of the graph)
  
  annotate(
    "curve",
    x = x_start, y = y_start,
    xend = x_end, yend = y_end,
    arrow = arrow(length = unit(0.2, "cm"), type = "closed"),
    color = "grey40"
  )
    (annotate the graph by putting caption)
  
  geom_vline()
    (draw a vertical line on the graph)
    
    
summary data 
   str()
   
   lm( y~x, data = "")
   [find the linear regression of the data]
   
   summary()
   
   df[[x]][y]
   (select x row the y col)
    df <- gapminder[[y]][x]
    (store a single variable)

    ef <- gapminder[x,y]
    (store the data into a data frame)
   
   
   
broom()
   nest(-x)
   [turn data into one row per variable, -x means nest all except x]
   
   tidy()
   [similar to summary]
   
   unnest()
   [doing opposite of nest]
  
  
purrr()
  map(x, ~ .)
  [applies an operation to each item in a list, x is the column imported, thing behind ~ are the operations]









SQL starts from here:
##############################################################################################################

  
SELECT x AS y FROM z
  [select column x, name it as y, from dataset z]


COUNT(x)
  x = *
    [tells you how many records are in a table]
  x = col name
    [tells you how many records will contain this col name]











  
 