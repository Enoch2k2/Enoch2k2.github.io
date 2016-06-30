---
layout: post
title:  "Argument Variables and How They Are Used"
date:   2016-06-30 18:14:48 -0400
---


What are argument variables? We know that variables are used to store integers, strings, and booleans. However, when we define methods, we have argument variables inside the parenthesis. There are two stages I like to think of a method. The defined stage, where you define your method and the call stage, when you use your method. Most of the time when you have a method in the defined stage, you will have information you want to use when it's called. For instance...
    
```
def add_two_nums(num_one, num_two)
  num_one + num_two
end
```

What you see is, this method has two argument variables, num_one and num_two. What exactly does num_one and num_two do? The answer is clear, when you define the method, you already have the intentions of adding two numbers together. When you make it dynamic and want to use that method to take in any two numbers, you use two argument variables. So when you run your method (method call) you get back the result (return value). So in this case...
    
```
add_two_nums(1, 2)
```

What you see here is, I just use the name of the method `add_two_nums` to initiate the method call, then i add the two numbers to the argument `(1, 2)`. So when it calls that method the argument variables `num_one = 1`, and `num_two = 2`. The positioning of the numbers does matter in the method call. Since `num_one` is the first argument variable when we defined `add_two_nums` then the first argument we put into the method definition will be equal to the first argument inside the method call, hence `num_one = 1`. Then same for the second position in the method definition will be equal to the second position in the method call. Which makes your methods dynamic.

So behind the scenes when that method is called, you can think of your method definition doing this.

```
def add_two_nums(num_one = 1, num_two = 2) # here 1 and 2 is being passed in through the method call
  1 + 2            # 1 and 2 are added and then returned
end
```

Which of course gives us 3 returned.

So argument variables are very helpful to use to make methods dynamic. As a new developer, you should take your time to understand the concepts of argument variables and why methods should be dynamic. Best of luck and go forth young, inspiring, beautiful minded tech nerds and change the world with code!
