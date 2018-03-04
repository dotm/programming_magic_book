# Basic Spells

## Primitive Data Types (The basic atoms of the programming universe)

In the beginning, the programming universe (a.k.a. your RAM) was formless. It is filled with a vast ocean of memory bubble, but there’s no "thing" in it. Now you as the programmer stare over the surface called monitor to peek through to this universe from your terminal (command line), with your hands hovering above the keyboard that control everything in this universe. You as the programmer of this universe are the one who wield the power to create "things" out of this ocean.

There are 3 basic things you can create.

The first thing is Number. You can create 0, 42, 0.0001, 3.14, or -9 inside a memory bubble. You can even create 2.4e3 which turns into 2.4 &times; 10<sup>3</sup> which turns into 2.4 &times; 1000 which turns into 2400. Or you can create 2.4e-3 which turns into 4 &times; 10<sup>-3</sup> which turns into 4 &times; 0.001 which turns into 0.004. 

All the number above that can be created inside a bubble (0, 42, 0.0001, etc.) is called **Numeric Literal**.

The second thing you can create in this universe is word and character which in the programming universe is called String. You can create a single character string like "b". You can create a multi characters string like "7070". You can create a single word string like "hello". You can create a multi word string like "Hello World".

Anything inside double quotes creates a string inside a bubble and is called **String Literal**.

The last basic thing you can create is what is called Boolean. True or False. On or Off. You can create one electron inside a bubble to make it On. You can create an empty bubble to make it Off.

The **Boolean Literal** only have two variation: True and False.

These 3 things are called primitive data types. It is called primitive because it is the basic building block of the programming universe. Much like different kind of atoms are the primitive data types of the physical universe, these 3 things (Number, String, Boolean) are the primitive data types of the programming universe.

The way you create any of these things is by typing. You type 42 and then you type Enter, and boom, you just create the Number 42. You type ‘True’ and then you type Enter, and boom, you just create the Boolean True.

This is all quite interesting. But you see a problem. When you create something inside a bubble, it exists only for a moment. In the blink of an eye, that thing you just create disappears back into nothingness. Fortunately you have two basic spells to solve this problem: variable declaration and variable assignment.

---
Spells learned:

- Number creation
  - Incantation: Numeric literal
  - Effect: create a number inside a bubble
- String creation
  - Incantation: String literal
  - Effect: create a string inside a bubble
- Boolean creation
  - Incantation: Boolean literal
  - Effect: create a boolean inside a bubble

---

---
## Variable Declaration and Variable Assignment Spells

The variable declaration spell creates a bubble and turns it into a solid box. How does this spell turn bubbles into boxes? By giving name to the bubble.

In the programming universe, when you give a name to a bubble, it becomes solid and permanent. Just like a box. That named box is called a **variable**.
When you take the name back, the box turns back into a bubble, and the bubble pops in a flash, and anything that exists within that bubble disappears into nothingness.

Let's turn an empty bubble into a box by giving it the name `a`:
```var a```
Done. What you see above is the variable declaration spell in action. The spell turns a fleeting bubble into a solid, persistent box by naming it.

Now let's see the variable assignment spell in action:
```a = 7```
The variable assignment spell create a thing you want to create (Number, String, Boolean) **inside** that named box. By creating thing inside of a named box, it becomes permanent, at least until you take the box name that envelopes that thing.

The = here is not the equal sign. It is how the spell of variable assignment is typed. In the programming universe = is the invocation of the variable assignment spell. So what is "equal"? It is == or ===. And "unequal" is not ≠, but instead != or !==. It’s how the programming universe works. Get used to it. Don’t complain. ;)

You can do the variable declaration and variable assignment spells at the same time:
```var a = 7```
This creates a bubble, turns it into a box named `a`, and create inside that box the Number 7.

In some programming language you may omit the var. So `a = 7` both declare a variable and assign 7 to that variable.

So, why do we bother creating things inside these permanent boxes instead of inside bubbles? The answer is: so that we can do things with them. For example, you can use arithmetic operators with Number:
```
a = 7
a + 3
a / 2
a
```
In `a + 3`, the `a` part before the `+ 3` is actually the Variable Call Spell: you take a **copy** of anything inside a variable (which in the case above is 7).
And, do you remember what the `3` means? Yep, it is a Numeric Literal used for Number Creation Spell.
The above `a + 3` then means that after you call the variable `a`, you get the value 7. Then, you create a 3 inside a bubble. And then you add both values (7 and 3).

The Variable Call Spell copy anything inside a variable, and give the copy to you, which means that the variable `a` still contains the value 7 inside it. So, when you do `a / 2`, the `a` still 'evaluates' to 7 (the `a` variable still have the value 7, and you can still take the 7 out), and you can divide it by 2.
The last line above just cast the Variable Call spell on the variable box `a` and do nothing to the value 7 you get from the spell.

Anyway, why do we call the named box a variable? Because the thing inside it can vary:
```
a = 7
a = "A multi word string"
```
The first spell above creates the Number 7 inside the box `a`. The second spell above makes the Number 7 inside the box `a` disappears and create the String "A multi word string" inside that box.

There are spells that can make the box only filled once. It is the Constant Declaration Spell and Constant Assignment Spell: 
```const A = 7```
With this spell you can make a box that can only be filled once. Once you create a thing inside the box `A` (which in the above case is 7), you cannot make that thing disappears and create another thing inside that box (e.g. the string "DoReMi"). In other words, once you assign a thing to that box `A` (which in the above case is 7), you can’t assign other things to it.

The Constant Call Spell is the same as the Variable Call Spell:
`A + 3`
You just type the name of the constant `A`, and you'll get a copy of anything inside that constant box.

Now, knowing that variable (named box) is called variable because it can vary, and knowing that = is the invocation of the variable assignment spell (and not equality), you can make sense of this spell incantations:
```
a = 2
a = a + 1
```
The first spell creates the box `a` and creates the Number 2 within it.
The second spell takes whatever the thing inside the box `a` (in this case 2), add it with 1 (which result in 3 because 2+1 is 3), and use that result (the Number 3) to create the value 3 inside the box `a` (replacing the Number 2 with the Number 3).

Adding with one is so common in the programming universe that there is a special spell for it: the Increment Spell.
To use the increment spell, you take a variable that has a Number value within it, and do this incantation: `variable_name++`
```
a = 2
a++   #This is the same as doing a = a + 1
```

There is also the Decrement Spell `a--` which is the same as doing `a = a - 1`

---
Spells learned:

- Variable declaration
  - Incantation: `var variable_name`
  - Effect: turn a nameless, fleeting bubble into a solid, persistent box by naming it with variable_name.
- Variable assignment
  - Incantation: `variable_name = literal`
  - Effect: do a creation spell inside a box.
- Variable call
  - Incantation: `variable_name`
  - Effect: get a copy of the value that exist inside a box named variable_name (the box need to be created first using Declaration Spell).
- Constant declaration
  - Incantation: `const Constant_Name`
  - Effect: turn a nameless, fleeting bubble into a solid, persistent box that can only be filled once.
- Constant assignment
  - Incantation: `Constant_Name = literal`
  - Effect: do a creation spell inside a box.
- Constant call
  - Incantation: `Constant_Name`
  - Effect: get a copy of the value that exist inside a box named Constant_Name (the box need to be created first using Declaration Spell).
- Increment
  - Incantation: `variable_with_number_value++`
  - Effect: add one to a box containing a number value
- Decrement
  - Incantation: `variable_with_number_value--`
  - Effect: subtract one from a box containing a number value
- Operator (Yes… Operators are spells too. You’ll learn more about them in the next section)

---

---
