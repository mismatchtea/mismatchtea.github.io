---
layout: post
title: "rectangles investigation"
date: 2014-02-21 15:13:30
description: "a rich investigation with links between number, geometry and algebra"
categories: [investigations]
tags: [investigation]
banner: 2014/0221-banner.svg
---

This post gives details of an investigation I was introduced to by a colleague whilst I was an NQT. It's a beautiful problem which links many aspects of maths. I use it to illustrate how closely related number, algebra and geometry are to one another. It takes between one and two lessons, depending on how far into the investigation you want to go.

## "this lesson is just counting"
I tell students that the fundamental skill they will need is to count. We start by counting the number of rectangles in the picture [above][banner]. This leads on to the issues of recording which rectangles have been counted and also ensuring all rectangles have been counted. Having discussed methods for counting the rectangles, we look at something a little more structured like the [How Many Triangles][transum] starter from Starter of The Day. This encourages students to take a systematic approach to counting the various shapes which will be useful for the remainder of the investigation.

## size three problem
The main investigation starts by considering the following diagram, which I call a size 3 rectangle:

[![size3][size3]][size3]

The instructions are vague; how many rectangles can you find in the following diagram? I can never remember the solution to this, but I do know what type of number to look for. After students have given their solutions I ask them to give a convincing written method for their solution. After this I find it important to model to the class a systematic method for recording the results.

## size four problem
Once students are confident with how many rectangles there are in a size 3 rectangle, I ask them to predict how many there would be in a size 4 rectangle:

[![size4][size4]][size4]

Students come up with some wonderful predictions, my favourite being double the number of rectangles there are in a size 3. I ask them then to draw the size 4 diagram and convince me of their solution.

## size n
By now students should realise that the task is time consuming and it is worth generalising the result. This is where the real maths starts. I begin by asking for predictions for size 5 and size 6 rectangles which is a nice piece of afl. Ultimately I want the students to realise that starting with the size 3 rectangle isn't the most natural place to start, so we find how many rectangles there are in a size 1 and size 2 rectangle and tabulate the results.

## number and algebra
By now they should start to recognise which type of numbers each size of rectangle produces - square numbers. The problem is that not all of the square numbers are used, so how do they find which square number is the desired one for a size n rectangle? On further investigation they should notice that each result in the table is the square of each term in the sequence of triangle numbers, leading to the algebraic form

$$R_n = \left(\frac{n(n+1)}{2}\right)^2$$

## multiple dimensions
Lastly, we consider extending the problem by looking at multiple dimensions. Whilst many students are keen to look at three dimensions, I remind them of the fact that starting with a size 3 rectangle wasn't to our advantage - so we first look at one dimension:

[![lines][lines]][lines]

Using the notation $$R_{n,1}$$ to represent the number of "lines" in a size $$n$$ line gives the formula:

$$R_{n,1} = \frac{n(n+1)}{2}$$

I looked at the 3D version with a colleague of mine. After an hour of playing with multi-link cubes and tabulating results we were happy that the following result holds true in 3D:

$$R_{n,3} = \left(\frac{n(n+1)}{2}\right)^3$$

## proof
I have spent a lot of time working on this investigation since I was introduced to it over four years ago. I imagine that the following result holds for $$d$$ dimensions, but I have not been able to prove it yet. 

$$R_{n,d} = \left(\frac{n(n+1)}{2}\right)^d$$

where $$n$$ is the size of the "rectangle" in $$d$$ dimensions.

The best we could come up with in the maths department was a geometric proof that showed the results hold for $$d=1$$ to $$d=3$$. I would like to find an inductive proof for it.

[banner]: {{site.postAssets}}/2014/0221-banner.svg
[size3]: {{site.postAssets}}/2014/0221-size3.svg
[size4]: {{site.postAssets}}/2014/0221-size4.svg
[lines]: {{site.postAssets}}/2014/0221-lines.svg
[transum]: http://www.transum.org/software/SW/Starter_of_the_day/starter_September23.asp?ver=stu
