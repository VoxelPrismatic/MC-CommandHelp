# SET UP THE BOARD (do this in order)

```
/scoreboard objectives add WINS
/scoreboard objectives setdisplay sidebar WINS descending
/scoreboard players set TeamRED WINS 0
/scoreboard players set TeamBLUE WINS 0
/scoreboard objectives add CONSTANT
/scoreboard players set CONSTANT CONSTANT 1
```
   
# ADD TO SCORE
```
/scoreboard players operation TeamRED WINS += CONSTANT CONSTANT
———OR———
/scoreboard players operation TeamBLUE WINS += CONSTANT CONSTANT
```

# REMOVE FROM SCORE
```
/scoreboard players operation TeamRED WINS -= CONSTANT CONSTANT
———OR———
/scoreboard players operation TeamBLUE WINS -= CONSTANT CONSTANT
```

## NOTES
I recommend inputting all of "set up the board" into a series of chain command blocks

"TeamRED", "TeamBLUE", "CONSTANT" can be changed, although must reflect across all matches (eg when changing "TeamRED", it must reflect across all "TeamRED"s)

The `+= CONSTANT CONSTANT` **is necessary**, otherwise it won't work

`+=` means "add this amount"

`-=` means "subtract this amount"
