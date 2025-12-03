# ⭐ 1. Testing SafeLine with HTTP Flood Attack

# 🔸 What is HTTP Flood?

An HTTP Flood is a DDoS attack where the attacker sends a massive number of HTTP requests to overwhelm a server.

# 🔸 What you performed:

Configured DVWA (acting as the attacker machine) to generate rapid HTTP requests.

Adjusted flood parameters such as:

Number of hits

Request method (GET/POST)

Time duration

# 🔸 SafeLine Response:

SafeLine detected the abnormal request volume.

Blocked or throttled traffic based on the configured protection mode.

Generated visual attack logs showing:

Request spikes

Attacking IP

Decision taken (block/allow)
