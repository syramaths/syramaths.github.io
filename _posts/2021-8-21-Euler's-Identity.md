---
layout: post
title: Euler's Identity
---

This equation connects some of the fundamental constants in mathematics in an amazingly simple way. Here, I will show how this forumla can be derived.

Let's say we have a complex number z, where z = a + bi.

This number z can be written in terms of sin and cos, z = r(cosθ + isinθ), where r is the modulus of z, and θ is the argument of z.

Then, we can find the Maclaurin series of sin(x) and cos(x):

sin(x) = x - (x^3)/(3!) + (x^5)/(5!) - (x^7)/(7!) + ...
cos(x) = 1 - (x^2)/(2!) + (x^4)/(4!) - (x^6)/(6!) + ...

So, isin(x) = i(x - (x^3)/(3!) + (x^5)/(5!) - (x^7)/(7!) + ...)

Therefore, z = r((1 - (θ^2)/(2!) + (θ^4)/(4!) - (θ^6)/(6!) + ...) + i(θ - (θ^3)/(3!) + (θ^5)/(5!) - (θ^7)/(7!) + ...))

And, with a bit of re-arranging:

z = r(1 + iθ - (θ^2)/(2!) - i(θ^3)/(3!)) + (θ^4)/(4!) + i(θ^5)/(5!) - (θ^6)/(6!) - i(θ^7)/(7!) + ...)
  = r(1 + iθ + (iθ)^2/(2!) + (iθ)^3/(3!) + (iθ)^4/(4!) + (iθ)^5/(5!) + (iθ)^6/(6!) + (iθ)^7/(7!) + ...)
  
This looks suspiciously like the Maclaurin series for e^x:
  
e^x = 1 + x + (x^2)/(2!) + (x^3)/(3!) + (x^4)/(4!) + (x^5)/(5!) + (x^6)/(6!) + (x^7)/(7!) + ...
  
Now, if we replace x with iθ, we get:

e^(iθ) = 1 + iθ + (iθ)^2/(2!) + (iθ)^3/(3!) + (iθ)^4/(4!) + (iθ)^5/(5!) + (iθ)^6/(6!) + (iθ)^7/(7!) + ...

Therefore, we can write z in terms of the exponential function:

z = re^(iθ)


Now that we have this, all we need to do is substitute in some values for r and θ, and we will get Euler's identity!

let r = 1, θ = π

z = e^(iπ) 
  = cos(π) + isin(π)
  = -1 + i * 0
  = -1
  
And there it is:

e^(iπ) = -1

Or, equivalently:

e^(iπ) + 1 = 0


Beautiful!
