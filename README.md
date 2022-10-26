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
 

  
  
  
  
  
  
 