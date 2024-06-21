### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/pritamparab/minimum-planes.git
    ```
2. Navigate to the project directory "minimum-planes"
3. Open "minimum-planes-problem.html" file on the browser.

## Code Initialization

  - `planes` keeps track of the number of planes hired.
  - `currentEnd` is the farthest airport we can reach with the current plane.
  - `farthest` is the farthest airport we can reach overall up to the current point.

## Code logic

  - Update `farthest` to the maximum distance reachable from the current airport.
  - When we reach `currentEnd`, it means we need to hire a new plane because we have exhausted the current plane's fuel.
  - If `currentEnd` is greater than or equal to the last airport index, break the loop.
  - If after hiring a new plane, we can't move further, return `-1`.
  - If we exit the loop and haven't reached the last airport, return `-1`.
