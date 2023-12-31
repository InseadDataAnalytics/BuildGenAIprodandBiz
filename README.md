   # INSEAD MBA Course "Building genAI Products and Business"
   **T. Evgeniou, Professor INSEAD** [GitHub](https://github.com/tevgeniou) | [LinkedIn](https://www.linkedin.com/in/theodoros-evgeniou-5397b/)

<b><it>The material for session 1 was developed by **Olivier Mertens**, Developer Audience, Azure Open AI Service, @Microsoft [GitHub](https://github.com/olivMertens) | [LinkedIn](https://linkedin.com/in/mertensolivier) </b></it>
</br>
</br>

In the first session, we will learn about some Gen AI tools that we will use for product prototyping during the class.

We'll use  OpenAI Service and keys to access/use models with the use of apis and [Google Collab](https://colab.research.google.com/) (browser based) for some python coding. 

> [NOTE]
> You can also use all notebooks in a local/your computer: with Visual studio code or using Conda to launch Jupyter notebook

## First steps 

### OpenAI Account
1. **Go to the OpenAI website**: Go to [https://www.openai.com/](https://www.openai.com/)

2. **Create an account**: Click on the 'Sign Up' button on the top right corner of the website. Fill in your details and follow the prompts to create your account.

3. **Verify your email**: Check your email for a verification link from OpenAI. Click on the link to verify your account.

4. **Log in to your account**: After verifying your email, log in to your account using your credentials.

#### Discover Sandbox GPTs 

To experiment with the key concepts of [prompt engineering](./pages/prompts.md), [models](./pages/models.md) and [RAG - retrieval Augmented Generation](https://learn.microsoft.com/en-us/azure/search/retrieval-augmented-generation-overview) you could visit and test the sandbox GPTs (just announced by OpenAI in November 2023) to play with a chatbot interface without the need to code ("No Code" environment). To do so, you can go to [https://platform.openai.com/playground](https://platform.openai.com/playground)

![Alt Text](img/assistantchatbotcreation.png)
Select your model (e.g., we can select gpt-4 or earlier - and less costly - ones like gpt-3.5-turbo)
![Alt Text](img/modelsGpts.png)

If you want to know about differences between the available LLM models, you can deep dive at [this link](https://platform.openai.com/docs/models/overview)

This interface will be shown after you have correctly created your chabot
![Alt text](img/playgroundChatbotOpenAi.png)

You can also read this for some more background [on basic prompt engineering](./pages/prompts.md)

Other resources:
- Sandbox / Playground Open AI [https://platform.openai.com/playground](https://platform.openai.com/playground)
- Documentation Assistants [https://platform.openai.com/docs/assistants/overview](https://platform.openai.com/docs/assistants/overview)
- API With openAI [https://platform.openai.com/docs/api-reference](https://platform.openai.com/docs/api-reference)


## Step-by-step guide to create a user login on OpenAI and prepare your organization and key


5. **Access the API dashboard**: Once logged in, navigate to the API dashboard named Api Keys. 

6. **Create a new API key**: If you don't already have an API key, you can create a new one by clicking on the 'Create new API key' button.

![Alt text](img/secretkeygenerate.png)
You can select the name you want

You will have this kind of view after creating a key (or several keys) ![Alt text](img/apiKeysexampleopenAi.png)
<br>
<br>

> <b>IMPORTANT</b>
> Don't forget every usage of a model with OpenAI will <b>cost</b>  something! (check this link to understand the difference in pricing / models)[https://openai.com/pricing]

7. **Copy your API key**: After creating your API key, make sure to copy it and store it <b>somewhere safe</b>. This key is used to authenticate your requests to the OpenAI API. <b>Whoever has access to it will be charging your account when using it!</b>

8. **Set up your organization**: In the API dashboard, you can also set up your organization if needed. This involves adding other users to your organization and managing their access levels.

![Alt text](img/organizationOpenAi.png)

**Remember**, keep your Open AI API key secure and **do not share** it with anyone. It's also a good practice to regularly rotate your API keys, or create a new one for each application or usage.


### Google account & Colab Notebook

In order to simplify potential issues with different python versions or different operating systems and installations on your personal computer, we will use **notebook Colab** for the course. You can of course also work on your computer if you choose to, using for example [Anaconda](https://www.anaconda.com/) (beyond the course).

- You need to have a Google Gmail Account. If not [create a new one](https://support.google.com/mail/answer/56256?hl=en-EN)

## Exploring genAI: Three Examples

We will use these three colab notebooks as starting examples. Go to [https://colab.research.google.com/](https://colab.research.google.com/) and follow these links to have the latest notebooks for course session 1:
<br>
- Interview questions generation [https://aka.ms/inseadGenAi-1](https://aka.ms/inseadGenAI-1)
- Web article generation [https://aka.ms/inseadGenAi-2](https://aka.ms/inseadGenAI-2)
- (This one will require some more steps, see below) Extract audio with whisper and process the text [https://aka.ms/inseadGenAi-3](https://aka.ms/inseadGenAi-3)

We will be adding more over time (as you will notice). 

You may encounter warning pop-up windows - click **ok**

![Alt text ](./img/warningnotebook.png)

When a notebook is correctly imported in your personal collab, you have to first import your "secrets"

- Add your secrets (Key and organization imported form OpenAI **sk-XXX** and **org-xxxxxx**) in the left panel in Google Collab

![Alt text](./img/secrets.png)
Create the variable secrets one at a time:

- Copy/paste this name: ````OPENAI_API_KEY```` 
- Copy paste your sk-key inside the right input 
- Click on the left blue button to render the secret available in your notebook

> Next, if needed (you do **not** need to do this for the course), you can also add "secret" for an organization:

- Copy/paste this name: ````OPENAI_ORGANIZATION````
- Copy paste your org-key inside the right input 
- Click on left blue button to render the secret available in your notebook

</br>

To use/run a notebook you have to click on every small "play button" inside the notebook

 ![Alt text](./img/playbuttonnotebook.png)

**Note** that for the three example notebooks the very first "code chunk" (that installs packages) may take a few seconds to run and will be generating some messages. Simply wait till it completes running. 

</br> 

For the third (audio analysis) Notebook, you can import you own mp4 file video or audio to analyse. To so so:
- Click on the folder button on the left
- Import your file inside the current path - click yes to the pop up warning. Note that you have to respect the file naming ("interview.mp4") or else you will have to change the name in the notebook itself in the line *inputFile = "/content/interview.mp4"*

</br>

![Alt Text](./img/finaluploadinterviewfile.png)

</br>

# You are now ready to explore! Have Fun!

### Don't be afraid of **python** you will also get help! 
 :smiling_face_with_three_hearts:


# Some reference links 

- [AI Term Glossary](./pages/glossary.md)
- [ Models ](./pages/models.md)
- [ Prompt Engineering](./pages/prompts.md)


[More information on Azure Open AI services can be found here](https://learn.microsoft.com/en-us/azure/ai-services/openai/overview)
