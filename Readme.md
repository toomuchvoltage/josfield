# Abstract
So I argued with [Jos Stam](https://en.wikipedia.org/wiki/Jos_Stam) about whether I'm smart or not and I convinced him I'm smart.
Along the way I found an alternative to [Jeff Tupper's self-referential formula](https://en.wikipedia.org/wiki/Tupper%27s_self-referential_formula) that is both more awesome and more flexible.

# Background
Some crazy day on March I was talking to Jos about wishing to maybe some day go and do a masters... but only on topics I'm interested in (e.g. real-time rendering or simulation.)

And along the way Jos seemed to suggest that he was uncertain whether I was smart or not... because he was under the impression I had somehow schmoosed my way into Autodesk. Which is entirely untrue, I got interviewed by 5 people in a 4 hour period and most folks on that panel had already dug up my engine and knew what I was about. In fact, decision makers not on that panel had also looked into my work as well and were quite impressed.

Hell, I had even showed Jos my work... but as I've learned, generally getting Jos to remember stuff or to stick to things is next to impossible.

So me and Jos got into a bit of an argument over his suspicions. Because I felt a bit insulted and ignored. Then I asked him if he knew about the [Superformula](https://en.wikipedia.org/wiki/Superformula). And to my surprise, he hadn't heard of it in his life.

And thus started our email chain...

# On the way to discovery...

Initially I sent him the superformula link and he got back and introduced me to his old pal Jeff Tupper.

![email1](http://toomuchvoltage.com/josfield/img/jos1.png)

I saw the formula and I thought... hey this looks neat. And what an interesting guy. Moreso, my brain went to work and I said to my self, `"hey I used to come up with neat crap like this back in high school... I'm pretty sure I can impress him"`

So one night and many espressos later, I came up with what I called the `Jos Field`. To be honest coming up with this stuff is rather trivial. But it's neat and a nice exercise on the brain. So I got back to him with:

![email2](http://toomuchvoltage.com/josfield/img/jos2.png)

For those interested here's the derivation:

[derivation](http://toomuchvoltage.com/josfield/pdf/josfield_derivation.pdf)

As mentioned in the email this alternative has some interesting properties:

* Unlike Tupper's self-referential formula, this is defined on R^2. Tupper's formula is only defined within a certain x and y.
* Tupper's formula is an inequality that results in **true** and **false**. Those are then taken as **dots** and **holes**. This is a continous function that can simply just be evaluated everywhere.
* You can define your own image, including the formula itself. Just modify the resolution by changing **20** and **7** and put your bits on the **k table** and interpret it as a big integer.
* You can even have sharp peaks by using anything between 0-9 on your **k table**. The implementation here only supports 0's and 1's because it's easier to optimize for that.

Some concessions from Jos ;):

![email3](http://toomuchvoltage.com/josfield/img/jos3.png)

But I kept busting his ****s. I even did the gradient field:

![email4](http://toomuchvoltage.com/josfield/img/jos4.png)

And if that wasn't enough, I even did a ray-marching 3D version of it.

![email5](http://toomuchvoltage.com/josfield/img/jos5.png)

# `src` or it didn't happen...

Check out the source code in the `src` folder. If you're impatient... just look at the `png`s in there.
The `width` and `height` attributes on the `<canvas>` element in the HTML file define the image size. Reduce them if you're impatient and/or things take too long. You can set `Do3D` to `false` in the JavaScript to see the 2D image.

Enjoy!

# Conclusions... ?

∎ I'm smart! ;)