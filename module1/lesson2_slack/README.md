Question to answer in your notes: which severities arrived, and WHY those? The code looped through SEVERITIES and sent a message (INFO, WARNING, ERROR, CRITICAL). But slack.py only delivers alerts at or above the threshold in .env. Mine is set to INFO, so every severity passed the filter. 

In your notes: how many hours apart are server time and YOUR wall clock? 5 hours

In your notes: why is a quiet INFO here GOOD design, not a failure? It keeps you informed of the disk status without causing a panic. 

In your notes: what would make this number spike on the Balerica bank? Many users using SWIFT, API usage, and installing software. 

In your notes: which of these fake incidents deserves to wake a human at 3 AM? “account_lookup returned code 12: ledger file not reachable”. If the ledger isn’t accessible, the bank can’t do its job. 

Question to answer in your notes: which severities arrived, and WHY those? I predicted 1 (CRITICAL) because the slack.py skips any levels below what’s in .env.

With SLACK_ALERTS_ENABLED=false, hw1 printed “Skipped” and nothing reached Slack, even though the severity filter (INFO) would have allowed it. The kill switch turns off all alerts at once, without editing any code. That helps during maintenance windows: when engineers are deliberately restarting services or taking things offline, the monitors would otherwise flood the channel with expected “failures.” Too many false alarms cause alert fatigue, and people may then ignore a real problem. Afterward, you flip it back to true.
