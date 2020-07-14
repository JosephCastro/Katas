# Angel Problem


There's an Angel that exists in a map with M and N size and can move
randomly across that map.

For example, he's in a X,Y point and can move to J,K point.

Also there's a Devil, that can remove a point (X,Y) of the map randomly, so the Angel
can't land in that point anymore. (Also can't remove the point used by the Angel in the same moment).

The Devil wants to catch the Angel.

## First scenario
You need to simulate this scenario following the next rules:

1. The map es about 16x16
2. The Angel starts in the middle of the map
3. In every step, the Angel moves randomly to any position enabled.
4. In every step, the Devil removes randomly, one position from the map.
5. If the Angel can't move to the position, then doesn't move until the next step.
6. If the Devil can't remove one position, can try one more time until he gets one.
7. There's a total of 150 steps (movements)
8. The Devil wins if the Angel can't move for 5 times (continually).
9. The Angel wins if complete all the steps

