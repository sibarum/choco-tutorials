# Choco Tutorials

Tutorials for Choco, a Constraint Programming library for Java. Designed for average developers, not scholars.

## What is constraint programming?

I'll answer that question by asking a question of my own: How would you tell a computer how to paint a picture?

**Imperative Programming**:

    while (!picture.isComplete()) {
      brush.dipInto(nextPaint());
      brush.moveTo(nextCoords());
      brush.press(canvas);
      brush.moveTo(nextCoords());
      brush.lift();
      brush.rinse();
    }

**Functional Programming**:

    function draw(Painting p) -> Painting
      if (size p) < 1
        then (paint p)
        else (quadrants draw p)

**Constraint Programming**:

    solver.post(numTrees < 10)
    solver.post(volumeOfWater < 20)
    solver.post(numDistinctColors = 5)
    solver.solve()

