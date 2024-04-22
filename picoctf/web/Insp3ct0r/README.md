# Insp3ct0r
Points: 50
## Category
Web Exploitation
## Problem Statement
> Kishor Balan tipped us off that the following code may need inspection: `https://jupiter.challenges.picoctf.org/problem/9670/` ([link](https://jupiter.challenges.picoctf.org/problem/9670/)) or http://jupiter.challenges.picoctf.org:9670
## Hints
> How do you inspect web code on a browser?
> There's 3 parts
## Solution
Once we open the link, we are greeted with a seemingly basic website. The title of the problem suggests to view the source code on browser and found the first part of flag.
```html
...
</p>
<!-- Html is neat. Anyways have 1/3 of the flag: picoCTF{tru3_d3 -->
    </div>
...
```
Then, we checked `mycss.css` file and found second part of the flag
```html
...
/* You need CSS to make pretty pages. Here's part 2/3 of the flag: t3ct1ve_0r_ju5t */
```
Lastly, after inspecting another file `myjs.js` we found last part of the flag
```html
...
/* Javascript sure is neat. Anyways part 3/3 of the flag: _lucky?2e7b23e3} */
```
And we combined the three parts of the flag
## Flag
`picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?2e7b23e3}`