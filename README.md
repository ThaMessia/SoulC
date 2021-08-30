# SoulC
Sooo, I was seeing how a Brainfuck interpreter was made and I saw it was tastefully easy.
I thought I could create a new esoteric programming language similar to brainfuck and I did it.

![SoulC](https://user-images.githubusercontent.com/68974876/130805678-5868d748-4d36-4f00-8261-95478d273c9c.png)

As said before, SoulC is similar to Brainfuck but with some differences. 
Don't know Brainfuck but you still want to program in SoulC? It's okay, I prepared a documentation of the language with 
some examples to make it easier to understand (it's an esoteric programming language :D)

# Documentation:

Let's see some basics of the language
```yml
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
.p
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
.p
xxxxxxxxxx
.
```
This program prints "Hi" and then, escape code of newline.
Every 'x' represents a letter (or just a character if you want to make it simple) in ASCII, therefore it means that 
to **memorize** a letter, you must type how many 'x' for how many characters in ASCII that letter will be.

Example: 
```yml
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```
This will **memorize** an 'a' because there are 97 'x' and 'a' in ASCII is 97.


To understand what ".p" means, we can divide it in two parts: '.' and 'p'. '.' is very easy to understand, it just prints output.

Why did I talk about memorizing all this time? Because every character in the .soulc file is all in an array.
If I want to print multiple characters I have to advance in the array. 
Now that we have this concept clean in our mind, let's move on.

'p' stays for **pointeradvance**, it means that by writing 'p' in our program after the output ('.')
we can advance in the array, allowing ourselves to print more characters. 

But what if we want to go back into the array? We can just use 'q'.

Let's move on!

```yml
,[.,]
```

Ok, this can be particular to understand. ',' is input and these square brackets means counts as control structures.
If you noticed that this code takes input and then prints out the input given in a loop, then you are right.

For people who still don't understand how that code works, let's take it easy.
All of this code takes place in **one element of the big array**, 
that means that we can use the input given as a variable to print.

The control structure here counts as a loop, so it's obvious it will repeat itself forever since no instructions are given.

# Summary
If you learnt all of this, then you fully understood the basics of SoulC, and you can say you learnt an esoteric programming language.

I can say just one thing now: **Enjoy the language!**
