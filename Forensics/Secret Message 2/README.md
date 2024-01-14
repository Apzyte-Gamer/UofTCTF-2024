Secret Message 2
=

The super secret organization changed their flag again. Can you work your magic again?

Hint: The flag characters contain `abcdefghijklmnopqrstuvwxyz_`

Author: SteakEnthusiast

[redacted.png](./redacted.png)

Solution
=

By opening the image, I noticed that this time, the text was blurred. So, I went on looking for Unredacters, until I came upon an electron app made by BishopFox named [unredacter](https://github.com/BishopFox/unredacter). 

I quickly downloaded the source code and opened it up in VS Code.

Then according to the hint, I went src/preload.ts and changed `const guessable_characters = 'abcdefghijklmnopqrstuvwxyz ';` to `const guessable_characters = 'abcdefghijklmnopqrstuvwxyz_';`

Now, it was time to crop the image for the guessing. I opened up GiMP and zoomed to the blurred part and cut out that section where no pixel was left. I even managed to catch the top pixels that were almost blended with the background. The final image looked like this:

![Final Image](./secret.png)

I now executed the program and after 5-10 mins, I got the best guess as `pokemon_catching_ezz`.
I then formatted it into the format and got the flag!

`uoftctf{pokemon_catching_ezz}`
