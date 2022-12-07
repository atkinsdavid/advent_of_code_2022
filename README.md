# From https://adventofcode.com/2022

<details>
    <summary>
        ##Day 01
    </summary>
    <ul>
        <li>split input on line breaks</li>
        <li>inside loop:</li>
            <ul>
                <li>multiplied value to ensure it was numeric</li>
                <li>used counters to track current index position in array of totals, and reset if we hit a 0 value</li>
                <li>add value to running total inside loop</li>
                <li>add running total to current index position</li>
            </ul>
        <li>sort the array of totals, get the last one for pt 1</li>
        <li>add together the values from the last 3 index positions</li>
    <ul>
</details>

<details>
    <summary>
        ##Day 02
    </summary>
        <ul>
            <li>split input on line breaks</li>
            <li>set number values for each possible sting (only 9 combos, seemed quickest)</li>
            <li>loop through input, add total of each line to total variable</li>
            <li>added second loop to recalculate string values based on instructions for pt2</li>
        </ul>
</details>

<details>
    <summary>
        ##Day 03
    </summary>
        <ul>
            <li>Added array of alphabet characters (didn't want to figure out how to generate the array)</li>
            <li>split input on line breaks</li>
            <li>pt1</li>
                <ul>
                    <li>loop through each pack</li>
                        <ul>
                            <li>loop through letters in first half of pack string</li>
                                <ul>
                                    <li>loop through letters in second half to compare letter from first half</li>
                                    <li>break after we find the match</li>
                                </ul>
                            <li>break after we find the match</li>
                        </ul>
                    <li>loop throguh alpha array to find matching character</li>
                    <li>add character's index position + 1 to the sum</li>
                </ul>
            <li>pt2</li>
                <ul>
                    <li>loop through each pack</li>
                        <ul>
                            <li>if it's the last in the group (counter = 2), reset the counter and move on</li>
                            <li>if it's the second in the group, add one to the counter and move on</li>
                            <li>if it's the first in the group</li>
                                <ul>
                                    <li>add one to the counter</li>
                                    <li>identify the rest of the packs in the group</li>
                                    <li>loop through each letter in the first pack</li>
                                        <ul>
                                            <li>break out of the loop if we've already found our letter</li>
                                            <li>loop through the letters in the second pack</li>
                                            <li>if this letter matches the letter from the first pack</li>
                                                <ul>
                                                    <li>loop through letters in the last pack</li>
                                                    <li>if this letter matches the letter from the previous 2 packs</li>
                                                        <ul>
                                                            <li>save our found letter</li>
                                                            <li>break out of this loop</li>
                                                        </ul>
                                                    </ul>
                                            <li>break after we've found our letter    </li>
                                        </ul>
                                    <li>loop throguh alpha array to find matching character</li>
                                    <li>add character's index position + 1 to the sum</li>
                                </ul>
                        </ul>
                </ul>
        </ul>
</details>

<details>
    <summary>
        ##Day 04
    </summary>
        <ul>
            <li></li>
        </ul>
</details>


<!--New Day template

<details>
    <summary>
        ##Day __
    </summary>
        <ul>
            <li></li>
        </ul>
</details>

-->