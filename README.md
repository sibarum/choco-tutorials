# Choco Tutorials

Tutorials for Choco, a Constraint Programming library for Java. Designed for average developers, not scholars. A work-in-progress. An attempt to use as many code samples as possible, as little reading as possible.

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

    numTrees < 10
    volumeOfWater < 20
    numDistinctColors = 5
    solve()

