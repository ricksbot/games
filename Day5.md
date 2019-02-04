# Day 5

## Business

Hello from Kansas State University Game Development Club,

Kansas State will be hosting our 5th annual Game Jam this upcoming February 8th-10th and we are looking for students from other universities who would be interested in coming to participate. Students participate for free and will have fun, food, and a great learning experience. Sign ups for our game jam and information can be found at: gdc.cs.ksu.edu! If you would be able to pass the information on to students or relevant clubs, we would love to see students from as many universities as are able to come! If you or any students have questions, please let me know! 

Thank you,

Nathan McClain

Junior | Computer Science
President of Hack K-State | Engineering Ambassador
Kansas State University
816.213.7180

## Prepare

**Not official advice**

One day you actually might make money from your game (ads or in-game purchases). You'll need to decide if making games is your hobby or if it has become a hobby (this has tax implications).

A business requires startup costs (filing fees, etc.), but allows you to better handle taxes (deduction, etc.) Hobbies don't require any filing fees, but you are required to pay income taxes on the earnings and deductions are harder.

As if this writing, here's the most recent guidance from the IRS: [Business or Hobby?](https://www.irs.gov/faqs/small-business-self-employed-other-business/income-expenses/income-expenses)

## Code

### Update on code

[Starter Code](https://github.com/CS2510/code/blob/master/day5/starter.html)

## Drawing Models in a World with a Camera

### Hierarchy
Everything is in a hierarchy.

Parents have children.

To "parent" a child to another object, the child can be (scaled and rotated) then translated.

Children can be parents of other children. You can do this infinitely.

## Save and Restore to have multiple children

Before the transform code to add a child, you call save() so you can parent other children. When you are down with one child's transforms, call restore() to add another child. You can do this recursively.

[Code from the end of class](https://github.com/CS2510/code/blob/master/day5/endOfClass.html).

Here is the same code with [additional comments and some standardized syntax](https://github.com/CS2510/code/blob/master/day5/endOfClassPolished.html). Start here if you want to build on the code.









