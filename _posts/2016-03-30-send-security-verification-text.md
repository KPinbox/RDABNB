---
layout: post
order: "21"
group: "Host"
group_id: 2
subgroup: "Verification"
subgroup_id: 22
title: "Request Verification Text"
description: "Text security code to selected phone number for account verification."
warning: "<strong>NOTE:</strong> This is a logged-in endpoint and requires an <strong>access_token</strong>. See <a href=\"#login-by-email\">Login Endpoints.</a>"
method: "POST"
endpoint_url: "https://api.airbnb.com/v2/security_checks"

complete_curl_request: "curl -X POST -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/json; charset=UTF-8\" --data-binary '{\"data\":{\"phone_number_id\":27231699,\"verification_method\":1},\"strategy\":\"phone_verification\",\"activity_type\":\"mobile\"}' --compressed https://api.airbnb.com/v2/security_checks?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD"

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

body: '{"data":{"phone_number_id":27231699,"verification_method":1},"strategy":"phone_verification","activity_type":"mobile"}'

---
{% include JB/setup %}
