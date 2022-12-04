# Text Classification with Neural Networks

In this notebook, machine learning models are implemented to predict the sentiment of movie reviews using the [IMDb movie reviews dataset](https://ai.stanford.edu/~amaas/data/sentiment/) through the `torchtext` package. Specifically, classifiers based on Convolutional Neural Networks (CNN's) and Recurrent Neural Networks (RNN's) are implemented. Both models attain approximately 82% test accuracy using the cross-entropy loss criterion. Both models are stored in `models.zip`.

Here are some predictions from the CNN model on the following example reviews.

> Prediction: 0, Actual: 0<br>
> Input: <UNK> isn't it ? <UNK> all the good work done by <UNK> and <UNK> , the movie never grew into something more than a horrible <UNK> movies copycat . <UNK> a couple of jokes , no absolutely no unpredictable twists , to be honest the only unpredictable moments are there because both director and editor made some stupid mistakes , it is a shame for them and a waste of time for us . <UNK> someone can tell me why on earth were they digging a hole inside that safe , who the hell is the <UNK> and how on earth did they know that the diamonds were in the particular cell , it could just make my day , but it seems that <UNK> asks us to take too much things in this one for granted , and do not raise our eyebrows when something looks <UNK> just another studio contract movie relax and <UNK> . 
> 
> Prediction: 1, Actual: 1<br>
> Input: <UNK> , <UNK> don't watch action movies because of the fact that they are usually all pretty similar . <UNK> movie did have many stereotypical action movie scenes , but the characters and the originality of the film's premise made it much easier to watch . <UNK> <UNK> <UNK> his normal acting approach , which was great to see . <UNK> <UNK> , of course , was beautiful and did great acting . <UNK> cast all together . <UNK> must see for people bored with the same old action movie . 
> 
> [TEST]   Loss: 0.4104    Accuracy: 82.66%

Here are some predictions from the RNN model on the following example reviews.

> Prediction: 0, Actual: 0<br>
> Input: <UNK> <UNK> had some great actors in it ! <UNK> they had forgotten how to act . <UNK> was hoping the movie would get better as it went along but the acting was so robotic it was doomed from the very start . <UNK> actually appeared that maybe the actors were reading from a script the whole time . <UNK> it was the <UNK> score or the <UNK> himself , but one thing is for sure the <UNK> artist needs to get another job  ! <UNK> <UNK> <UNK> was so thick you could see it <UNK> on the actors faces  ! <UNK> not recommend this movie to anyone , no wonder it never hit the <UNK> . <UNK> <UNK> <UNK> . / <UNK> <UNK> shame on you guys for not giving it your all . <UNK> <UNK> was great just needed a whole lot more . 
> 
> Prediction: 1, Actual: 1<br>
> Input: <UNK> tragically wonderful movie.. . brings us to a <UNK> that does not exist anymore . <UNK> <UNK> technical expertise , <UNK> have yet to see a ( hollywood ) movie that can match the authenticity of the atmosphere in this small town by the river near the <UNK> . <UNK> <UNK> <UNK> <UNK> <UNK> looked liked the last installment of the <UNK> of <UNK> <UNK> in trying to capture rural <UNK> <UNK> /><br <UNK> you like serene but intense story lines , this is a must see film . <UNK> will be a respite from hollow flashy films much like the last 1000 blockbusters you saw . <UNK> think this is one of <UNK> better stories.<br /><br <UNK> if it's a movie about <UNK> and brothels and the complicated rules that <UNK> life in such settings , it did not turn into a skin flick . <UNK> characters are full of depth and act with much intensity . 
> 
> [TEST]   Loss: 0.8557    Accuracy: 81.64%
