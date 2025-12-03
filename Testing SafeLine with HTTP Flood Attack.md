# ⭐ 1. Testing SafeLine with HTTP Flood Attack

# 🔸 What is HTTP Flood?

An HTTP Flood is a DDoS attack where the attacker sends a massive number of HTTP requests to overwhelm a server.

# 🔸 What you performed:

1. Configured DVWA (acting as the attacker machine) to generate rapid HTTP requests.

2. Adjusted flood parameters such as:

   => Number of hits

   =>Request method (GET/POST)

   =>Time duration

# 🔸 SafeLine Response:

1. SafeLine detected the abnormal request volume.

2. Blocked or throttled traffic based on the configured protection mode.

3. Generated visual attack logs showing:

   =>Request spikes

   =>Attacking IP

   =>Decision taken (block/allow)
