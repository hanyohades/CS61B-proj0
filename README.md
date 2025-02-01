# CS61B-proj0

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">

</head>
<body>
    <div class="container">
        <h1>2048 Game Implementation</h1>
        <h2>Project Overview</h2>
        <p>Implemented core game mechanics for 2048, focusing on tile movement, merging, and game state validation. Key methods include <code>tilt()</code>, <code>maxTileExists()</code>, <code>atLeastOneMoveExists()</code>, and <code>emptySpaceExists()</code>.</p>
        <h2>Key Implementations</h2>
        <h3>tilt() Method</h3>
        <ul>
            <li>Handles tile movement and merging in any direction</li>
            <li>Key challenges:
                <ul>
                    <li>Preventing double merges in a single move</li>
                    <li>Managing triple merges (only merging leading tiles)</li>
                    <li>Maintaining accurate score updates</li>
                    <li>Handling empty space movement</li>
                </ul>
            </li>
        </ul>
        <h3>Game State Validation Methods</h3>
        <ol>
            <li><strong>maxTileExists()</strong>
                <ul>
                    <li>Checks for 2048 tile presence</li>
                    <li>Board traversal optimization</li>
                </ul>
            </li>
            <li><strong>atLeastOneMoveExists()</strong>
                <ul>
                    <li>Validates remaining possible moves</li>
                    <li>Checks for empty spaces and mergeable adjacent tiles</li>
                </ul>
            </li>
            <li><strong>emptySpaceExists()</strong>
                <ul>
                    <li>Efficient empty space detection</li>
                    <li>Quick board state validation</li>
                </ul>
            </li>
        </ol>
        <h2>Testing Strategy</h2>
        <ul>
            <li>Used TestUpOnly.java as primary test guide</li>
            <li>Created test cases for:
                <ul>
                    <li>Basic tile movement</li>
                    <li>Single and multiple merges</li>
                    <li>Edge cases with triple merges</li>
                    <li>Full board scenarios</li>
                    <li>Win/lose conditions</li>
                </ul>
            </li>
        </ul>
        <h2>Lessons Learned</h2>
        <ul>
            <li>Importance of processing order in game logic</li>
            <li>Value of comprehensive test cases</li>
            <li>Benefits of breaking complex operations into smaller steps</li>
            <li>Significance of state tracking for game mechanics</li>
        </ul>
    </div>
</body>
</html>
