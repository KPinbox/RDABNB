---
layout: post
order: "11"
group: "Host"
group_id: 2
subgroup: "Messages"
subgroup_id: 20
title: "Respond To Message"
description: "Respond to a message in a message thread (whether as a host or guest)."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "POST"
endpoint_url: "https://api.airbnb.com/v2/messages"

complete_curl_request: "curl -X POST -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary '{\"message\":\"Thanks!  I'd love to host you. -Nima\",\"thread_id\":\"185143454\"}' --compressed https://api.airbnb.com/v2/messages?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Currency for listings" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "3m0ky1cmj6jm4x3sjm3sx8osf", description: "Airbnb auth token (from auth-ing with login endpoints)" },
	{ key: "Content-Type", value: "application/json; charset=UTF-8", description: "Content type" }
]

body: "{\"message\":\"Thanks!  I'd love to host you. -Nima\",\"thread_id\":\"185143454\"}"

---
{% include JB/setup %}
