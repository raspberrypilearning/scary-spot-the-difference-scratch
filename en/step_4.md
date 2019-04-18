## Add a random pause

Your program is nearly finished. In this step, you will make the program pause for a random number of seconds before the zombie appears.

--- task ---
Use a `pick random`{:class="blockoperators"} block and a `wait`{:class="blockcontrol"} block to make your program pause for a few seconds before the image of the zombie appears.

--- hints --- --- hint ---
The `wait`{:class="blockcontrol"} block is in the **Control** menu. Inside the `wait`{:class="blockcontrol"} block, place a `pick random`{:class="blockoperators"} block from the **Operators** menu.
--- /hint --- --- hint ---
Here are the two blocks you will need to add to your program.

```blocks
wait ( ) seconds

pick random (0) to (10)
```

--- /hint --- --- hint ---
This is what your completed program should look like.

```blocks
when green flag clicked
forever
switch backdrop to (start v)
if <mouse down?> then
switch backdrop to (scare v)
+wait (pick random (0) to (10)) seconds
end
end

```

--- /hint --- --- /hints ---
--- /task ---

--- task ---
Click on the `green flag`{:class="blockevents"} to test your code. When you click on the Stage, the zombie should appear after a random amount of time, and then the backdrop should switch back to the spot the difference image.
--- /task ---

