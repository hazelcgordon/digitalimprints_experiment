## Original survey and corresponding variable names

### Description of survey flow

The survey is split into four stages:

- Stage 1: 
  - Participants will be randomly split into one of two conditions, and half will see ‘training’ text informing them about the new laws for increased transparency.
- Stage 2: 
  - Participants will view four pieces of campaign material, two with digital imprints and two without.  
  - The material they view with and without imprints will be randomised, so that all pieces of material will be viewed with and without an imprint by different participants.
  - They will view each piece separately, and will be asked a set of questions after each one (these questions are only included once in this document, but will be viewed four times by participants)
- Stage 3: 
  - Participants will answer the same set of questions testing their recall of the content, their confidence in regulation, knowledge of regulation and online information self-efficacy.
- Stage 4:
  - Participants will answer the same set of questions about their demographics, levels of political trust/mistrust/cynicism, and social media use.
  
### Training
  
#### Training text

Some of the posts you might see when browsing on social media are political campaign posts.

A new transparency law for online political campaigning has just come into force. Now, most digital campaign material will require details of who paid for and produced it. This is designed to help voters know who is trying to reach them online and influence their vote.

You are about to see four randomly selected social media posts. Please review each example and answer a short number of questions about what you’ve seen.

#### No training text

You are about to see four social media posts. Please review each example and answer a short number of questions about what you’ve seen.

### Raw variables names

Thinking about the image you’ve just seen, to what extent do you agree or disagree with the following statements.

Response options: Strongly disagree (1) – Strongly agree (7)

**PK1_value** - The post feels like an advertisement;
**PK2_value** - This post promotes a particular viewpoint;
**PK3_value** - The post is an advertisement;
**PK4_value** - The post is intended to influence your opinion

*In the original dataset, this measure appears as PK_1_1, PK_1_2, PK_1_3 etc depending on which advertisement was viewed, the columns here are those in 'imprint_df' which reformats the dataset structure into long form with 4 rows for each pps*

**PK** - averaged score

---

**agree_value** - To what extent do you agree or disagree with the message promoted by the post? Response options: Strongly disagree (1) – Strongly agree (7)

---

To what extent do you agree or disagree with the following statements about the materials you have seen?

Response options: Strongly disagree (1) – Strongly agree (7)

Respondents indicate agreement with each statement separately.

**PG_value** - The material had a political goal; 
**informed2_value** - The material contained enough information to know who placed the material; 
**informed3_value** - I am not sure who is behind the material; 
**informed4_value** - I can make an informed judgement about who is behind this material

**informed** - averaged score of informed2, 3 and 4

---

Please circle the number in between each pair of words which represents how you feel about the material you’ve just seen.

The following sets of words are shown, and participants choose a number between 1 and 7 for each set.

**accurate_value** - Inaccurate (1) – accurate (7)

**trustworthy_value** - Untrustworthy (1) – trustworthy (7)

**believable_value** - Unbelievable (1) - believable (7)

**factual_value** - Opinionated (1) – factual (7)

---

The posts you just viewed were all examples of political campaign material. 

**election_reg** To what extent do you think there are sufficient laws to regulate online campaign material in the UK? Response option: Insufficient (1) – Sufficient (7)

---

Some of the campaign material contained information about its source. For example:

[example of digital imprint shown]

**recall_num** - Out of the individual Facebook posts you viewed, how many items do you recall containing transparency information about the source of the material?

0, 1, 2, 3, 4, Not sure

**recall_correct** - new column created to specify if the participant identified that they viewed 2 digital imprints. 2 = 'correct', any other value = 'incorrect'                

---

Which of the following groups do you remember being responsible for posting the material you were shown (you may select none or multiple)?
**FF** - Future First;  
**TPM** - The People’s movement;  
**VFP** - Voice for the People;  
**CSC** - Common Sense Collective (correct);
**BBA** - Breaking Barriers Alliance (correct);
**SFI** - Speak Freely Inc. (correct);
**CBB** -Campaign For a Better Britain (correct);
**AT** - All Together   

*The options were presented in a random order to participants*

**recall** - a variable created in the analysis script that matches if the campaigner name was recalled to the advert viewed in 'imprint_df', so each participant has 4 rows with the recall of the specific name corresponding to the advert row

---

Of the following actors, who do you think will find this information most useful? 

Please rank, with the actor who will find it most useful at the top.

**useful_rank_1** - Voters, to understand who is responsible for the campaign material; 
**useful_rank_2** -The electoral commission, to provide oversight of the democratic process; 
**useful_rank_3** - Academic researchers, to study political activity;
**useful_rank_4** - Journalists, to investigate political campaigns; 
**useful_rank_5** - The police, to ensure that electoral law is followed;
**useful_rank_6** - Other (please state); 
**useful_rank_6_TEXT** - *text for 'please state'*

---

**reg_know** - Countries vary in how much they regulate political advertising by campaigns and other organisations during elections. Thinking about the current controls on political advertising in the UK, which of the following statements do you think is most accurate?

- All political advertising (whether on television, radio, in newspapers or the internet) is subject to the same rules set by the UK government  
- All political advertising is regulated by rules set by the UK government, but there is one set of rules for advertising on television and radio and a different set of rules for advertising on the internet and social media  
- There are no regulatory controls on any type of political advertising during UK elections  
- Not sure  

---

Thinking about the types of political information available online, to what extent do you agree or disagree with the following statements.

Response options: Strongly disagree (1) – Strongly agree (7)

Respondents indicate agreement with each statement separately.

**EPE_1** - I feel confident that I can find the truth about political issues;
**EPE_2** - If I wanted to, I could figure out the facts behind most political disputes;
**EPE_3** - It is possible to figure out the truth about political issues;
**EPE_4** - There are objective facts behind most political disputes, and if you try hard enough you can find them

---

Please indicate the extent to which you agree or disagree with the following statements.

Response options: Response options: Strongly disagree (1) – Strongly agree (7)

**general_confidence_1** - Politicians often put the country above their own interests;
**general_confidence_2** - Most politicians are honest and truthful; 
**general_confidence_3** - In general, politicians are open about their decisions;
**general_confidence_4** - I monitor the behaviour of politicians closely; 
**general_confidence_5** - I check whether politicians have met their electoral promises; 
**general_confidence_6** - I double-check what politicians say in case of misleading information;  
**general_confidence_7** - Politicians are only interested in getting and maintaining power; 
**general_confidence_8** - Politicians pretend to care more about people than they really do;  
**general_confidence_9** - Our political leaders are prepared to lie to us whenever it suits their purposes

*The options were presented in a random order to participants*

political_trust = items 1-3 (Jennings et al., 2022)
political_mistrust = items 4-6 (Weinberg, 2023)
political_cynicism = items 7-9 (TO ADD)

---

**political_interest** - How interested would you say you are in politics?

- Not at all interested  
- Not very interested  
- Fairly interested  
- Very interested   
- Don’t know  

---

**external_efficacy** - How much do government officials care what people like you think?

- A great deal   
- A lot   
- A moderate amount     
- A little   
- Not at all   

---

**internal_efficacy** - How much can people like you affect what the government does?

- A great deal   
- A lot   
- A moderate amount    
- A little   
- Not at all   

---

**SM_use** - On an average day, how much time do you spend using the internet for news about politics and current affairs?

- None, No time at all   
- Less than 1/2 hour   
- 1/2 hour to 1 hour   
- 1 to 2 hours   
- More than 2 hours    
- Don’t know  

---

**SM_frequency** - How often do you use the following social media site, if at all? Facebook

- More than five times a day (1)
- 2-5 times a day (2)
- once a day (3)
- once every couple of days (4)
- once a week (5)
- less than once a week (6)
- never (7)

---

Demographic variable names should be clear.
