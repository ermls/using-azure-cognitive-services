# using-azure-cognitive-services
Showing how to set up and consume cognitive services

This is demo code from Microsoft Learn’s “Extract Insights from text with the Language service” training module. I am describing what the code does and entering in some data
as described in the module’s exercise.

In practice, I would use Power Platform to call the service through connectors or Power Automate flows. If I were using Python, I would use the same commands and a similar
format to create my own solutions, just modified for my project and the resource being used.

The procedure is similar for each cognitive solution when building each AI solution. These services provisioned, trained if needed, and consumed through API calls.

1. Here I create a general cognitive service resource and show the keys and endpoint. Alternatively, I can create a specific language resource which would work similarly.

![Cog Serv Portal 1](https://user-images.githubusercontent.com/83891373/188251575-70a434a2-fffd-4840-a7f5-a8e44e4ee3fd.jpg)

![Cog Serv Portal 2](https://user-images.githubusercontent.com/83891373/188251578-8a6073e8-c888-4375-87a3-38ffa53f6db8.jpg)

![Cog Serv Portal 3](https://user-images.githubusercontent.com/83891373/188251582-3e3652ab-05fc-41b4-90a9-75081390b02f.jpg)

2. Here I set the endpoint and key variables in the .env file for Python code I will use to initialize and consume the resource.

![Python Env Code](https://user-images.githubusercontent.com/83891373/188251596-d9f6870a-bf28-482a-8f29-9a84c447013f.jpg)

3. Here I import the .env variables from the previous step and use them to initialize a text analytics client from the cognitive service resource.

![Python Initialize Code](https://user-images.githubusercontent.com/83891373/188251600-e7a85ffe-f199-48e4-9dc1-eb5c09ba06dd.jpg)

4. This is a sample of the text files that will be fed into the text analytics client methods.

![Python Text Input](https://user-images.githubusercontent.com/83891373/188251606-d34c45ed-4238-4341-998c-041d662769a3.jpg)

5. Here I call the text analytics client through an API to perform specific tasks. They are called using Python methods with the sample text files as arguments. The rest of
the code formats and prints the results.

![Python Consume Code 1](https://user-images.githubusercontent.com/83891373/188251609-fb262b22-793d-4ae3-ae5b-81d2271952d4.jpg)

![Pythone Consume Code 2](https://user-images.githubusercontent.com/83891373/188251610-2ece9a94-24ae-4c78-ad1c-9c59c1e33277.jpg)

6. This shows me opening up the Powershell integrated terminal and running the python code.

![Python Run](https://user-images.githubusercontent.com/83891373/188251617-2a9221a4-a6e3-4f8d-8f1a-5f4ef9b0d83d.jpg)

7. This shows the text analytics results from the cognitive resource being printed to the screen. 

![Python Results](https://user-images.githubusercontent.com/83891373/188251622-2072e230-f1ec-4477-a732-68a497a86f94.jpg)
