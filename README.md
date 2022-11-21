## Submission Instructions

Once you've finished the take home assignment, please zip your code in a .zip and email it to us. Please include any relevant instructions in this README for how to run the app.

Also, make sure to check the boxes in the rubric below before you submit the assignment

## Rubric

Your task is to build a product analytics “session streaming” tool that allows product managers (PMs) to watch realtime user sessions. Instead of screensharing (which sends video data and is tedious for users), this tool should work by sending DOM updates. We’ll call our tool StreamDOM

### Simplifications

- Assume that **sessions last for a maximum of 3 minutes**. For example, in the tetris demo we only care about the first 3 minutes of the Tetris game!
- This tool obviously **doesn’t need to be production-ready**, but you should at least be aware of any issues you may encounter in more real-world scenarios
- Don’t worry about improving the UI of the stream past the `rrweb` functionality of `record` and `replay` - there will be some limitations of DOM-based screensharing, but this is completely fine for this challenge.
- You should be able to DIY the design (don’t worry too much about it)

### Required Functionality

- [ ] The product manager should be able to see the **list of all currently active sessions** (just showing session id’s is fine)
- [ ] The product manager should be able to **watch any active session in real-time**
- [ ] Since this is realtime streaming, latency is important! Consider using websockets

      Latency of event E = Time E observed by PM - Time of E in user session
- [ ] **(Bonus)** Measure the latency and display it for the product manager to see while watching sessions. For example, display ‘X ms delayed’ while PM is watching the session

# nooks-streamdom-challenge
