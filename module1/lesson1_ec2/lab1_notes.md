

Runs 1-7
**What changed:** (pip upgrade)
Run 2 Cloned my own repo and captured git_clone.jpg. Used my intials for TXN. 

**Errors and fixes:** (e.g., the activate "Permission denied" error and how Claude fixed it; forgetting the ID line before uvicorn and redoing it)

**What I newly understood:** (Why Claude is useful, what return codes 0 and 4 mean.)
Alice’s balance is still 5000.00, even though I posted TXN-JN-0003 (350.50) and TXN-JN-0004 (50.00) against her account. The balance didn't change. The likely reason is that payment_post writes to the journal (payments.dat), while accounts.dat was exported once by the installer. 

