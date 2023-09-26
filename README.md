<h1>NN Practices</h1>

This is a repository to hold some of my practice work while forllowing Andrej Karpathy's amazing Neural Networks zero to hero series :) Feel free to use anything here for your own learning!

<h2>individual stuff</h2>
The EZMNIST file is just a fun little practice I did in like an hour to recognize handwritten digits. (I only used google to find out how to load the dataset!). I feel like I now have a solid foundation and can pretty easily build up from here. Also GPU acceleration is really nice.

<h2>from the lessons</h2>
Some ai (MLP) generated names starting with 'bro':

```
brogyacha.
bro.
brochi.
broda.
brovalley.
brostianael.
brossan.
bron.
brovine.
brondina.
```
And some without context:
```
xybha.
fineluhah.
prynna.
musen.
nily.
shi.
kavlan.
aythouannes.
dafay.
kivina.
riniina.
aabis.
ayelee.
kinroy.
mavi.
haliigh.
reri.
aid.
raclynn.
inden.
```
<h2>things i've learned:</h2>

1) Matmul represents feedforward, where size[0] of the second tensor is the output of the layer before it and size[1] is the number of neurons.

2) You can do pretty much anything to make the output and call backward on the loss, it doesn't have to be a conventional neural net. You can do things like multiply and add random numbers and it will all be accounted for.

3) Vanishing gradients occurs when the activation function causes gradients to be zero, which are then propagated backward meaning some neurons don't learn. Batch normalization helps to mitigate this by scaling down the inputs to the activation before sending them through. Initializing parameters at lower values can also help to keep the loss from being too high and spiraling out of control.
