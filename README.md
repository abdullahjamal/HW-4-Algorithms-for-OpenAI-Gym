# HW-4-Algorithms-for-OpenAI-Gym

# 1 - Implemented a explicit policy for mountain car env
     First I move the car to the left and then check if the velocity is between 0.012 and 0.015. If velocity is between this range, I move  the car to the right. I tried with both original reward and modified reward and the plots can be found in plot folder. Looks like,        with modified reward, the car reaches the flag for more episodes.
    

# 2 - Implemented a explicity policy of cart-pole env
     For this environemt, I check the angle of the pole. If it is greater than 0, I move it to the right, otherwise I assign it the left action.

# 3 - Implemented a cross entropy method for mountain car env.
     I tried cross entropy method with both original reward and modified reward. I tried with one hidden layer and two hidden layer and   with different parameters, but looks like the reward doesn't change.

# 4 - Overview of algorithms studied in class
     You can find the brief details in 04_algorithms_methods_overview.md file
