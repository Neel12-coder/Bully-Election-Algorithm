# Bully-Election-Algorithm

Algorithm:
1. If coordinator does not respond to it within a time interval T, then it is assumed that coordinator has failed.

2. Now process P sends election message to every process with high priority number.

3. It waits for responses, if no one responds for time interval T then process P elects itself as a coordinator.

4. Then it sends a message to all lower priority number processes that it is elected as their new coordinator.

5. However, if an answer is received within time T from any other process Q,

(I) Process P again waits for time interval T’ to receive another message from Q that it has been elected as coordinator.

(II) If Q doesn’t responds within time interval T’ then it is assumed to have failed and algorithm is restarted.

