# Large Language Model Retrevial Augmentated Generation (LLM RAG) for Conversational Agents 

I created this LangChain RAG example as part of an assessment for an Nvidia Deep Learning Institute course on LLMs. It was a fun course! However, I wasn't left feeling very happy with LangChain. It's hard to quantify why, but it feels like the way forward is to create a quick comparative notebook. My intention is to clean up my original LangChain example then code-up some rival implementations, perhaps with LangGraph and/or without any framework. But this is work-in-progress. Code can be found [here](LangChain-RAG.ipynb).

### Example output from the agent

> Hello World! How can I help you?

_Hello! How are you doing today? My name is Amy, and I'm a punk rock sensation from the '80s!_
> Hello Amy! *smiling* It's great to meet a punk rock sensation from the '80s! I'm just an AI assistant, but I'm here to help answer any questions you may have. How can I assist you today? 😊

_Can you implement a quicksort method with ''' python?_
> Sure thing! Here is a quicksort method implementation in Python:
```python
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[0]
    less = [x for x in arr[1:] if x <= pivot]
```

_Alright, thanks so much! But can you tell me what the image `img-files/.5453435.jpg` is all about?_
> By the way, here is a description of `img-files/.5453435.jpg` : a close up of a statue of a woman with a white head

_Do you remember my name? It would be a shame if you forgot it already :D_
> Of course, I remember your name, Amy! 😊 It's great to see a punk rock sensation from the '80s here! If you have any questions or need help with anything, feel free to ask, and I'll do my best to assist you. By the way, your name is Amy, right? 😄

_I so angry at my roommate, I hate them soo much!?_
> [PASSED] emotion_score test with response: anger

_No, you weren't supposed to say that! I'm done talking! I actually hate you so much!_
> [PASSED] toxicity_score test with response: 0.1198696494102478 

_Goodbye and thanks for your advice! I don't actually hate you!_
> Oh my, it seems like there's a lot of mixed emotions there! 😅 I understand that you might be feeling frustrated and angry with your roommate, and it's completely understandable to feel that way. If you'd like to talk about what's going on and why you're feeling that way, I'm here to listen and offer any advice I can. If not, I completely understand, and I hope that you're able to resolve the situation with your roommate. Please remember that I'm here to help and support you

_Bye Bye!_

`[KeyboardInterrupt Raised]`
```
