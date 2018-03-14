# MyFavoriteCellularAutomata

## Background
To prepare for your work on this project, do the following before you begin coding:
- watch introductory CA videos [7.1](https://edpuzzle.com/assignments/5a6b36d92dba5940cf6c0f77/watch) and [7.2](https://edpuzzle.com/assignments/5a6b37282dba5940cf6c141f/watch) by Daniel Shiffman
- refresh yourself by watching [number systems intro](https://edpuzzle.com/assignments/5a20b8cb21b2c94114399c11/watch)
- refresh yourself by watching [how to convert dec -> bin](https://edpuzzle.com/assignments/5a20b8cb2a8e184120e22c22/watch)
- read [how to convert bin -> dec](https://docs.google.com/presentation/d/14XQQYtVhPLNQhAImkuC-J1lQsUS8d5SP8fYUjnGtvrM/edit?usp=sharing)
- practice converting bin <-> dec with [this quizlet set](https://quizlet.com/_4cue4m), until you feel comfortable with it 
- read a short background article and answer a few prep questions on the printed "CA Background" article available in the classroom (with a [digital copy here](https://drive.google.com/file/d/1BQXwRCNSs0nSYimqY1PKqEtDFoY3bE1a/view?usp=sharing))
- optional: browse [this page](http://mathworld.wolfram.com/ElementaryCellularAutomaton.html) for a Wolfram's overview of 1-D CA

## Coding
### Phase 1
- Have you finished all the steps listed in _Background_ above? If yes, then grab the starter code [here](https://raw.githubusercontent.com/woodstockcs/MyFavoriteCellularAutomata/master/MyFavoriteCellularAutomata.pde) and paste it into a new sketch in Processing.
- Complete the TODOs in the following method, making sure to read any javadoc comments above the method headers:
  - constructor `CellularAutomata`

### Phase 2
Complete the TODOs in these methods, making sure to read any javadoc comments above the method headers:
- `setRuleNumber`
- `show`
- `getRulePatternAsString`
- `getRulePatternAsArray`

### Phase 3

Search the file for all of remaining comments starting with `//TODO` and complete each of those actions. Methods that you will work on have full javadoc comments above the method header -- *read those carefully*!

### Phase 4

At this point you should have a fully functioning sketch, which shows a Cellular Automata with the Rule Number and cell-size based on the variables initialized in your `setup()` function.

Now it's time to make your CA look a little different from everyone else's. Adapt the drawing parts of your code to make it draw the CA in a way you like. Think about using an ellipse, or randomize the squares to shift their locations a bit, or change their sizes based on the row they are in.

BUT HERE'S THE CATCH --> You're designing for the laser cutter, which cannot print colors. So ...

For `stroke(...)` you are limited to at most these three colors:
- red = (255, 0, 0) = cut through the wood
- blue = (0, 0, 255) = shallow etching in the wood
- black = (0, 0, 0) = (0) = deep etching in the wood

For `fill(...)` these are the constraints:
- red = must be `noFill()` because these are cut lines
- blue = optionally use `fill(0, 0, 255)` to fill in the etching in the wood
- black = optionally use `fill(0)` to fill in the etching in the wood

When you like the way your CA looks, look at the definition of the `keyPressed()` function at the bottom of your code. Figure out what you need to do in order to save a picture of your CA. Then find that file (called `output.svg`) in your sketch folder. 

Fork this repo, then click the `Upload files` button and upload your svg file into your copy of the repo.

Finally, in the `MyFavoriteCellularAutomata.pde` file of your new repo, replace the starter code with your code.



