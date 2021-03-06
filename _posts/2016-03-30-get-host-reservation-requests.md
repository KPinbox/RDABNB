---
layout: post
order: "12"
group: "Host"
group_id: 2
subgroup: "Messages"
subgroup_id: 20
title: "Get Reservation Requests"
description: "Returns information about all the listing reservation requests new, preapproved or declined."
method: "GET"
endpoint_url: "https://api.airbnb.com/v1/reservations/relationship"

complete_curl_request: "curl -X GET -H \"X-Airbnb-OAuth-Token: 9nwld6we4td9vkwj160teb49a\" -H \"Content-Type: application/x-www-form-urlencoded; charset=UTF-8\" --compressed https://api.airbnb.com/v1/reservations/relationship?client_id=3092nxybyb0otqw18e8nh5nty&locale=en-US&currency=USD&thread_id=188111261"

category: "endpoint"
tags: []

default_required_url_parameters: [
	{ key: "client_id", value: "3092nxybyb0otqw18e8nh5nty", description: "API Key" }
]

required_url_parameters: [
	{ key: "thread_id", value: "188111261", description: "The message thread associated with this reservation. (See \"Get Host Messages\")" }
]

optional_url_parameters: [
	{ key: "locale", value: "en-US", description: "Desired lagnuage" },
	{ key: "currency", value: "USD", description: "Desired currency" }
]

required_header_parameters: [
	{ key: "X-Airbnb-OAuth-Token", value: "9nwld6we4td9vkwj160teb49a", description: "Airbnb auth token (from auth-ing with login endpoints)" }
]

default_required_header_parameters: [
	{ key: "Content-Type", value: "application/x-www-form-urlencoded; charset=UTF-8", description: "Content type" }
]

---
{% include JB/setup %}
