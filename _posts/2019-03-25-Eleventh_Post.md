---
layout: post
title: Week Eleven- Bugs!
---

The goal for this week is to debug a small function given to us.

To begin, I simply copied and ran the code given to us. This produced the following error:

![](https://i.imgur.com/Rfmp4Io.png)

Using this message, I went back to line 8 and 9 and look for an unexpected symbol. Before I do this, I need to understand what the statement is trying to do. After I have an understanding of what the program is trying to do, I began looking for a symbol that is out of place. I notice the ending curly brace before `return` is closing the action in the for loop before the return statement. I removed this curly brace, moved the return statement to a new line, and then quickly looked threw the code to see where the curly brace would need to be replaced. Since there was already one at the true end of the for loop, we don't need to add one there. However, there is not one that closes the entire code for the function, so I add the curly brace to the end of the entire function code.

Now, I try to rerun the program again with one of the small data sets preloaded into R called CO2! This time, the code is sourced into RStudio without error and we see a new variable called `turkey_multiple` added to our global environment. When we run the function using CO2 data as the input, we see a new error:

![](https://i.imgur.com/He6zxw3.png)

The reason we didn't see this error earlier, when we saw the first error, is because it wasn't given any input to test the function with. All R was doing was making sure that each function or loop or statement was written correctly.

The next error we get is about the function `tukey.outlier` not existing:

![](https://i.imgur.com/mRqGkTh.png)

When I review the code, this is correct. No function named `tukey.outlier` was ever defined. Perhaps, this was meant to be the function  `outlier` from the outliers package.

I install and load the outliers package and change `tukey.outlier` to `outlier`. Next, when we attempt to run the program, we get the following error:

![](https://i.imgur.com/9HCMlZK.png)

This is telling us that the proper input for the function output is not being provided. To fix this we chance the input to be a subset of x. Now we run the program again. This time it runs cmopletely and we get output with a warning message.

![](https://i.imgur.com/mFyN9Ki.png)

To find all errors, I kept running `debug(tunkey_multiple(week11))` and moving line by line through the code until a new error came up. We were successful in debugging the program! However, I'm not sure I have made the program do what was originally intended since it seems to not even use the first for loop. I am also not sure what information the output is telling us but it runs! The code for this assignment can be found [here](https://github.com/jessicalynnrose/Intro_to_R_Spring_2019/blob/master/week11.R).
