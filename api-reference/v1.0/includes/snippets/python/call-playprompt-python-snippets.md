---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = PlayPromptPostRequestBody(
	client_context = "d45324c1-fcb5-430a-902c-f20af696537c",
	prompts = [
		MediaPrompt(
			odata_type = "#microsoft.graph.mediaPrompt",
			media_info = MediaInfo(
				odata_type = "#microsoft.graph.mediaInfo",
				uri = "https://cdn.contoso.com/beep.wav",
				resource_id = "1D6DE2D4-CD51-4309-8DAA-70768651088E",
			),
		),
	]
)

result = await graph_client.communications.calls.by_call_id('call-id').play_prompt.post(body = request_body)


```