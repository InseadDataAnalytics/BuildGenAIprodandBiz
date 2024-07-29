# Building genAI Products and Businesses 
   **T. Evgeniou, Professor INSEAD** [GitHub](https://github.com/tevgeniou) | [LinkedIn](https://www.linkedin.com/in/theodoros-evgeniou-5397b/)

During the course we will be using [Google Collab](https://colab.research.google.com/) (browser based) to run python scripts that will be calling openAI LLMs through the openAI API. This is why you will need to have a Gmail account (see [information here](https://support.google.com/mail/answer/56256?hl=en)) as well as an OpenAI one (see [information here](https://platform.openai.com/signup)) - in case you do not have these yet, please make sure you create them.  [Github](https://github.com/olivMertens)

You will find here instructions on how to prepare for the course. You will need to: 
- Purchase some openAI credit (e.g., worth $10) that you can use for API calls to the openAI LLM models
- Open a sample Google Colab notebook 
- Create your **secret** (do not share with anyone) OpenAI API Key
- Add your openAI API key in your colab notebook
- Run your first example of using API calls to the openAI LLMs
</br>
<it>Note:</it> This material was initially developed with the support of Olivier Mertens, Developer Audience, Azure Open AI Service, Microsoft [Github](https://github.com/olivMertens) | [LinkedIn](https://linkedin.com/in/mertensolivier/)
</br>
</br>

## Purchase some openAI credit that you can use for API calls to the openAI LLM models

1. [Log in your openAI account](https://platform.openai.com/)
2. Go to [billing](https://platform.openai.com/settings/organization/billing/overview) - Note: in case the links change, please search for "billing" or "API credit" or equivalent.
3. Purchase $10 worth of credit
4. You can see [information about pricing here](https://openai.com/api/pricing/) and you will also be able to monitor your spending in your billing dashboard. 

**Note: This is different from being an openAI subsrciber for using GPT, and you need to purchase credit even if you are a premium GPT user.**

## Open a sample Google Colab notebook

First you need to have loged in both to your Gmail and your OpenAI accounts. Make sure you are logged in at [Google Colab](https://colab.research.google.com/). 

Let's now start our first Colab Python notebook! All you need to do is to [click on this notebook](https://colab.research.google.com/drive/1Sds6CJffHtxCGF_bok9uwLnyETgKheGz?usp=sharing), which will open a browser tab with a python notebook on Google Colab. Once open, you can make a copy of the file in your personal Google drive (select "File -> Save a Copy in Drive"), that you will then be able to edit and use. 

## Add your openAI API key in your colab notebook

Open the copy of the file from you own drive (select "File --> Open Notebook"). Then, as indicated in the screenshot below, add your OpenAI API key. You can get your API key folowing the steps below. 

<img width="1120" alt="Add API Key Colab" src="https://github.com/user-attachments/assets/e44acb63-b89c-450a-9c87-61b9c2def099">

## Create your secret (do not share with anyone) OpenAI API Key

1. [Log in your openAI account](https://platform.openai.com/)
2. Go to the [OpenAI playground dashboard](https://platform.openai.com/playground)
3. Click on the "API keys" located on the left menu
</br>
<img width="287" alt="API Keys" src="https://github.com/user-attachments/assets/319e35af-752c-4607-88ac-00815f88191c">

4. Create a new API key by clicking on the "Create new secret key" button, and give it a name (e.g., INSEAD_BGenAIPB). Before selecitng "Done", copy the key and save it in a safe place! <b>Important: Never share your API key with others! Whoever has access to your API key can be charging your account when using it! It's also a good practice to regularly rotate your API keys, or create a new one for each application or usage.</b>
</br>
<img width="1107" alt="Create API Key" src="https://github.com/user-attachments/assets/c629563a-4db6-4e01-82ce-338ec5fcfbae">.

You can now also paste the API key in the Colab notebook as indicated in the previous step. When you create new Colab notebooks, the key will be automatically added. 


### Run the Google Colab notebook
To use/run a notebook you have to click on every small "play button" inside the notebook **on the left** of each code chunk. You may encounter warning pop-up windows - click **ok** or **execute** to continue.

![Alt text ](./img/warningnotebook.png)

</br>

>**[Note]** The very first "code chunk" (that installs the openai package) may take a few seconds to run and will be generating some messages. Simply wait till it completes running. 


</br>
</br>

## Exploring genAI: Three More Examples

Here are three colab notebooks as starting examples:
<br>
- Interview questions generation [https://aka.ms/inseadGenAi-1](https://aka.ms/inseadGenAI-1)
- Web article generation [https://aka.ms/inseadGenAi-2](https://aka.ms/inseadGenAI-2)
- (This one will require some more steps, see below) Extract audio with whisper and process the text [https://aka.ms/inseadGenAi-3](https://aka.ms/inseadGenAi-3)


For the third (audio analysis) Notebook, you can import you own mp4 file video or audio to analyse. To do so:
- Click on the folder button on the left
- Import your file inside the current path - click yes to the pop up warning. Note that you have to respect the file naming ("interview.mp4") or else you will have to change the name in the notebook itself in the line *inputFile = "/content/interview.mp4"*

</br>

![Alt Text](./img/finaluploadinterviewfile.png)

</br>



</br> 

## You are now ready to explore! Have Fun!

__Don't be afraid of **python** you will also get help!__

 :smiling_face_with_three_hearts:
