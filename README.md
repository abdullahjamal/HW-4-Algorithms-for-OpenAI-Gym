# HW-4-Algorithms-for-OpenAI-Gym

# 1 - Implemented a explicit policy for mountain car env
     First I move the car to the left and then check if the velocity is between 0.012 and 0.015. If velocity is between this range, I move  the car to the right. I tried with both original reward and modified reward and the plots can be found in plot folder. Looks like,        with modified reward, the car reaches the flag for more episodes. Looking at the enviroement, the reason behind this policy is basic physics. If we move the car to the left and then release it from some point, there is an ample chance it will touch the flag.
    

# 2 - Implemented a explicity policy of cart-pole env
     For this environemt, I check the angle of the pole. If it is greater than 0, I move it to the right, otherwise I assign it the left action. To solve the problem, we should get the reward of 195 averaged over the episodes. Here the average reward is 43 and the maximum reward is 72. The idea behind the policy is to stable the cart-pole. If the angle is greater than zero, it has to move to the right to be in stable position. With more sophisticated approaches, one would get solve the problem by getting an average reward of 195 over number of episodes.

# 3 - Implemented a cross entropy method for mountain car env.
     I tried cross entropy method with both original reward and modified reward. I tried with one hidden layer and two hidden layer and   with different parameters, but looks like the reward doesn't change.

# 4 - Overview of algorithms studied in class
     You can find the brief details in 04_algorithms_methods_overview.md file
