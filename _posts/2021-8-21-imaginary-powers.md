---
layout: post
title: Imaginary Powers
---

In this short post, I will show you how you can find i^i.

Whilst I don't know how to deal with "i to the power of something imaginary" in a very nice way, I do know how to deal with "e to the power of something imaginary". So, I will write i^i in terms of e:

i^i = e^(ln(i^i))

Hmm, looks like we can do something with this logarithm:

e^(ln(i^i)) = e^(i ln(i))

Aha! This is starting to look a lot like a number in the form e^(iθ), which we do know how to find, using e^(iθ) = cosθ + i sinθ. But what exactly is ln(i)?

Let's say ln(i) is equal to some number x. This means that:

e^x = i

Looking at e^(iθ) = cosθ + i sinθ, we can see that for e^(iθ) to equal i, cosθ must equal 0, and sinθ must equal 1. This happens when θ = π/2 radians.

Therefore, we now know that x (or ln(i)) must be iπ/2. 

And there it is! 

i^i = e^(i ln(i))

 = e^(i * iπ/2)
 
 = e^(-π/2)
