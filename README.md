# Choco Tutorials

Tutorials for Choco, a Constraint Programming library for Java. Designed for average developers, not scholars. A work-in-progress. An attempt to use as many code samples as possible, as little reading as possible.

## What is constraint programming?

I'll answer that question by asking a question of my own: How would you tell a computer how to paint a picture?

**Imperative Programming**: You define a step-by-step procedure.

    while (!picture.isComplete()) {
      brush.dipInto(nextPaint());
      brush.moveTo(nextCoords());
      brush.press(canvas);
      brush.moveTo(nextCoords());
      brush.lift();
      brush.rinse();
    }

**Functional Programming**: You come up with a simple pattern that is repeated at each level of granularity.

    function draw(Painting p) -> Painting
      if (size p) < 1
        then (paint p)
        else (quadrants draw p)

**Constraint Programming**: You define what you want the picture to look like, then outsource to Oompa-Loompas.

    numTrees < 10
    volumeOfWater < 20
    numDistinctColors = 5
    solve()

