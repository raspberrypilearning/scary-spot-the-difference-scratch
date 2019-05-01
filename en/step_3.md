## Detect mouse clicks

Soon, you can ask a friend to try out your new Spot the Difference game. They will have to click on as many differences as they can find.

But they won't know that after their first click, a timer will start, and then the zombie will appear!

--- task ---
To detect mouse events, like a click, your program has to always be listening for the event. To set this up, you can use a `forever`{:class="blockcontrol"} loop.
Add a `when flag clicked`{:class="blockevents"} block and a `forever`{:class="blockcontrol"} loop to the code for the Stage.

```blocks3
when green flag clicked
forever
end
```
--- /task ---

--- task ---
Your code will change the backdrop, so make sure that the `start`{:class="blocklooks"} backdrop is displayed at the beginning of the game.

```blocks3
when green flag clicked
forever
+switch backdrop to (start v)
end
```
--- /task ---

--- task ---
Now, you need to use an `if`{:class="blockcontrol"} block to detect if `mouse down?`{:class="blocksensing"}. If it is, then you can `switch backdrop to scare`{:class="blocklooks"}.

--- hints --- --- hint ---
You can find the `if`{:class="blockcontrol"} block in the **Control** menu and the `mouse down?`{:class="blocksensing"} block in the **Looks** menu.
--- /hint --- --- hint ---
Here are the blocks you will need to add to your program.

```blocks3
switch backdrop to (scare v)

if < > then
end

mouse down?
```

--- /hint --- --- hint ---
Here is what your script should look like.

```blocks3
when green flag clicked
forever
switch backdrop to (start v)
+if <mouse down?> then
switch backdrop to (scare v)
end
end

```

--- /hint --- --- /hints ---
--- /task ---

--- task ---
Click on the `green flag`{:class="blockevents"} to run the program. When you click on the backdrop, the image of the zombie should appear briefly.
--- /task ---
