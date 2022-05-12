# I  MISTAKENLY DELETED A STATE MACHINE ON A CLIENT TEST .. OH CRAP

<img src="image/albert-einstein.jpg">

I intended to delete the log on the step machine console but mistakenly deleted a state machine on the client test. Shoot... 

I tried to rerun the existing pipeline, but it doesn’t work because it no longer exists.

I tried to modify the state machine definition and redeploy, but it is still erroring state machine no longer exists, so it can’t update new changes.

I told my manager, and they fixed it, but I did not ask how they did it.

That led me to write this repo and feed my curiosity. And finally, I can fix this, and here is what I did.

1. Change the name of a state machine, push to a master branch, and wait until Cloud Formation creates a brand new state machine.
2. Rename that same state machine, push to a master branch, and redeploy it.
3. That’s it. You got your same state machine before.

## “Anyone who has never made a mistake has never tried anything new.”
## ― Albert Einstein

