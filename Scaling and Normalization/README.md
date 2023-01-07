

# Types of scaling

## Max absolute scaling

## Min-Max Scaling

In the Min-Max Scaling, there are two approaches we can follow, the automatic one, or the manual one:

# The manual approach

insteam of implementing the module, we can implement the mini-max scaling by hand following these fourmlas:


 (value - min) / (max - min)
 
 
 # The automatic approach
 
 we can install the module which named as mlxtend, by follwoing these commands: <br>
 

Thus, scaling is done by using a pre-built in module named mlxtend, we can install it as follows:

          !pip install mlxtend      

<img width="755" alt="image" src="https://user-images.githubusercontent.com/63984422/210859616-ecea77eb-d217-4652-bca6-bc6de87ed603.png">


By doing that, we can only call it upon the data and the specified column, and it will do the min-max scaling automataclly 
 

 We then can use this module to scale our data, choosing certain column as follows: 
 
 
                     # select the usd_goal_real column
                    original_data = pd.DataFrame(kickstarters_2017.usd_goal_real)

                    # scale the goals from 0 to 1
                    scaled_data = minmax_scaling(original_data, columns=['usd_goal_real'])
 
 
 
 
