## Installation

### Create an environment
Whatever you prefer (e.g. `conda` or `venv`)
```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

### Activate it
Mac / Linux:
```console
. venv/bin/activate
```
Windows:
```console
venv\Scripts\activate
```
### Install PyTorch and dependencies

For Installation of PyTorch see [official website](https://pytorch.org/).

You also need `nltk`:
 ```console
pip install nltk
 ```

If you get an error during the first run, you also need to install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

## Usage
Run
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```
## Customize
Have a look at [intents.json](intents.json). You can customize it according to your own use case. Just define a new `tag`, possible `patterns`, and possible `responses` for the chat bot. You have to re-run the training whenever this file is modified.
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```

## What can the chat bot do?
Ask questions such as:
1.	Hi
2.	Hey
3.	How are you
4.	Is anyone there?
5.	Hello
6.	Good day
7.	Bye
8.	See you later
9.	Goodbye
10.	Thanks
11.	Thank you
12.	That's helpful
13.	Thank's a lot!
14.	Which items do you have?
15.	What kinds of items are there?
16.	What do you sell?
17.	Do you take credit cards?
18.	Do you accept Mastercard?
19.	Can I pay with Paypal?
20.	Are you cash only?
21.	How long does delivery take?
22.	How long does shipping take?
23.	When do I get my delivery?
24.	Tell me a joke!
25.	Tell me something funny!
26.	Do you know a joke?
27.	What is malware?
28.	What is a malware?
29.	What is phishing?
30.	What is encryption?
31.	What is a firewall?
32.	What is an Intrusion Detection System (IDS)?
33.	What is a vulnerability?
34.	What is a cyberattack?
35.	What is a data breach?
36.	What is ransomware?
37.	What is Two-Factor Authentication (2FA)?
38.	What is a zero-day exploit?
39.	What is patching?
40.	What is social engineering?
41.	What is endpoint security?
42.	What is network security?
43.	What is a password policy?
44.	What is identity theft?
45.	Why is cybersecurity awareness important?
46.	What is a Security Operations Center (SOC)?
47.	What is incident response?
48.	How's the weather today?
49.	What's your favorite color?
50.	What's the latest news?
51.	Tell me about yourself
52.	Do you have any hobbies?
53.	What's your favorite movie?
54.	What's the meaning of life?
55.	Do you like to travel?
These patterns cover a wide range of topics and can be used for engaging in a conversation with the chat bot.