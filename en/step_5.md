## Add a scream

In this step, you will make the zombie scream when the image appears.

--- task ---
Add a `play sound until done`{:class="blocksound"} block after the zombie image appears, and set it to the *scream* sound.

--- hints --- --- hint ---
You can find the `play sound until done`{:class="blocksound"} block in the **Sounds** menu.
--- /hint --- --- hint ---
Here is the block you will need to add.

```blocks
play sound (scream v) until done
```

--- /hint --- --- hint ---
Here is the completed program.

```blocks
when green flag clicked
forever
switch backdrop to (start v)
if <mouse down?> then
switch backdrop to (scare v)
wait (pick random (0) to (10)) seconds
+play sound (scream v) until done
end
end
```
--- /hint --- --- /hints ---
--- /task ---

--- task ---
Click on the `green flag`{:class="blockevents"} to test your program. When you click on the stage, after a random pause, the zombie should appear and a scream sound should play.
--- /task ---

Prank your friends by asking them to play your Spot the Difference game. Tell them they have to click on all the differences they find in the image, and then watch them jump in fear when the zombie appears!
