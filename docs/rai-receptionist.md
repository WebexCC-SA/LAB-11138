# AI Receptionist

AI Receptionist

AI Receptionist for Webex Calling is your always-available virtual front desk assistant. It automates routine tasks like answering calls, responding to simple questions, and transferring calls to queue. With AI Receptionist handling the basics, your staff can stay focused on high-value conversations that truly enhance customer satisfaction.

We are going to create an AI Receptionist to front face the calls from our callers. In our lab scenario, our AI Receptionist will answer the call and will help our callers with responding to simple questions and based on the intent, our AI receptionist can transfer the call to the Sales and Orders or the Returns and Support queue.

<p class="lab-step" markdown="1">24. Navigate to “Calling” in the left pane and then click “AI Receptionist” on the list.</p>

![Screenshot](./assets/image79.png)

<p class="lab-step" markdown="1">25. First, lets upload a Knowledge base doc for our AI Receptionist. The Knowledge Base doc is in the Workstation1 Desktop - please make sure you are choosing the right vertical Healthcare vs Retail doc for your knowledge base.</p>

<p class="lab-step" markdown="1">26. Click “Knowledge Base” and then click “Create knowledge base” option.</p>

![Screenshot](./assets/image80.png)

<p class="lab-step" markdown="1">27. Give the knowledge base a name and description of your choice. Or you can give the name as “Retail KB” and the description as “Retail Knowledge Base”. Click Create.</p>

![Screenshot](./assets/image165.png)

<p class="lab-step" markdown="1">28. Now click the “Retail KB” knowledge base.</p>

![Screenshot](./assets/image166.png)

<p class="lab-step" markdown="1">29. Click “Add”</p>

![Screenshot](./assets/image83.png)

<p class="lab-step" markdown="1">30. In this next screen, click “Choose a file” and choose the correct KB file from the desktop.</p>

![Screenshot](./assets/image84.png)

<p class="lab-step" markdown="1">31. Then click “Add” after you have chosen the file.</p>

![Screenshot](./assets/image85.png)

<p class="lab-step" markdown="1">32. The file will take few mins to process. We can continue building the AI Receptionist. Click the Back button on the top, next to “Knowledge Base” wording</p>

![Screenshot](./assets/image167.png)

<p class="lab-step" markdown="1">33. Click “AI Receptionists” on the top and click “Create AI receptionist”</p>

![Screenshot](./assets/image87.png)

<p class="lab-step" markdown="1">34. You will now see the “AI Receptionist” wizard. There are multiple steps/tabs that will assist us in building the AI Receptionist.</p>

<p class="lab-step" markdown="1">35. For the General Settings tab, use the following values and click Next.</p>

Location: dCloud-SJC

AI Receptionist Name: Retail AI Receptionist

Phone number: {{Choose a number from the drop-down}}

AI Engine: Webex AI Pro US 1.0

AI Receptionist Language: English (United States)

AI Receptionist Voice: {{Any of your choice}}

Direct line caller ID Name: {{Choose the Display name}}

![Screenshot](./assets/image168.png)

<p class="lab-step" markdown="1">36. In this page of “Receptionist guidelines” – we can setup the AI Receptionist Goal, the AI Transparency message and the Welcome message.</p>

AI Receptionist Goal - we can instruct the AI Receptionist how to work or respond with the caller. All the guardrails and the instructions can be mentioned in this field – we can get as granular as we want and give it very specific instructions.

Transparency message – We can type in the message that the AI Receptionist must read out to the caller indicating the call is answered by an AI. You can alter the message if needed.

Welcome message – The Welcome message that is said by the AI Receptionist after the Transparency message is read out.

For our use-case today, we are going to use an existing Template. Click the “Apple template” drop-down and choose the option “Retail Store”

![Screenshot](./assets/image169.png)

<p class="lab-step" markdown="1">37. Take a minute to read the Template’s AI Receptionist Goal and the Welcome message. The Goal from the template is good for our lab today but if you would like to add more goals or instructions to the AI Receptionist – feel free to do so.</p>

<p class="lab-step" markdown="1">38. Welcome Message – The template will put in the tag “[FirmName] – [City]” – remove that and add the name as “Retail”. Your Welcome Message can be: “Hello! Welcome to Retail Store Support. How can I help you with store information, orders, or returns today?”. If you would like a different Welcome message – please change it to your choice.</p>

<p class="lab-step" markdown="1">39. Click “Next”</p>

![Screenshot](./assets/image170.png)

<p class="lab-step" markdown="1">40. In this page, click the “Select” drop-down and choose the knowledge base that you had created. Click “Next” in the bottom right corner after choosing the knowledge base.</p>

![Screenshot](./assets/image171.png)

<p class="lab-step" markdown="1">41. In this page, we can choose the “Default action” for our AI Receptionist. After the caller question is answered/unanswered by the AI Receptionist by referencing the knowledge base and the caller still has a question – we can perform the default action.</p>

<p class="lab-step" markdown="1">42. Click the drop-down and choose the option “Transfer Call” and choose the Contact type as “Resource” and choose the “Returns and Support” user here. Click “Review” on bottom right corner.</p>

![Screenshot](./assets/image172.png)

<p class="lab-step" markdown="1">43. Review all the settings and if everything looks good, click “Create”.</p>

![Screenshot](./assets/image173.png)

<p class="lab-step" markdown="1">44. Now, lets create some Intents for our AI Receptionist. Click “Next:Add Intents” on bottom right corner.</p>

![Screenshot](./assets/image174.png)

<p class="lab-step" markdown="1">45. We will create two Intents here. One is if the caller wants to talk to the Sales and Orders queue and the other if the caller wants to talk to the Returns and Support queue.</p>

Intent 1:

Intent Name: SalesOrders

Intent description: Use this intent if the caller is asking about purchasing products, placing an order, or getting assistance with an existing order. Use this intent if the caller is asking about any of the following:

<p class="lab-step" markdown="1">• Product availability or pricing<br>• Product information or recommendations<br>• Placing a new order<br>• Questions about an existing order<br>• Order status or tracking<br>• Changes or cancellations to an order<br>• Shipping or delivery questions<br>• Other sales or order-related questions requiring staff assistance</p>

Select Contact type as Resource and select contact as Sales and Orders

Click “Add Intent”

![Screenshot](./assets/image175.png)

Intent 2:

Intent Name: ReturnsSupport

Intent description: Use this intent if the caller is asking for assistance with a return, refund, exchange, replacement, or product-related issue. Use this intent if the caller is asking about any of the following:

• Questions about returns or refunds<br>• Exchange or replacement requests<br>• Issues with a product, including damaged, defective, or non-working items<br>• Warranty or product support questions<br>• Order issues or missing items<br>• Shipping or delivery problems<br>• Other returns or support-related questions requiring staff assistance

Select Contact type as Resource and Select Contact: Returns and Support

Click “Add Intent”

![Screenshot](./assets/image176.png)

<p class="lab-step" markdown="1">46. Now we have two intents created, lets move to the next step. Click “Next: Go to knowledge base” in the bottom right corner. Make sure, your knowledge base document is showing up in the files list.</p>

![Screenshot](./assets/image97.png)

