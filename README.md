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
