# serverless-step-function

I tended to delete log on step machine console, but mistaken delete a state machine on client test. Shoot... 

I tried to rerun existing pipeline, it doesn't work because that state machine no longer exist.

I tried to modified state machine defination, redeploy, it is still erorring state machine no longer exist.

And, Finally, I am able to fix this, and here what I did.

1. Change name of a state machine, push to master, and wait until cloud formation create a brand new state machine.
2. Rename that state machine, push to master, and redeploy it.
3. That's it. You got your exact same state machine before.

"Failure is the key to success; each mistake teaches us something."

