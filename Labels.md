










      Competition: Flu Shot Learning: Predict H1N1 and Seasonal Flu Vaccines
    
























































Skip to main content






















Competitions






How it works






Partner with us






DrivenData
LABS






Blog






Log in






Sign up







































  
    health
  







Flu Shot Learning: Predict H1N1 and Seasonal Flu Vaccines







                  
                  
                  Can you predict whether people got H1N1 and seasonal flu vaccines using information they shared about their backgrounds, opinions, and health behaviors?

                  




#health


































beginner

      practice
    
  




















10 months
 
left






























8,311
 joined
    



































































          Join competition
          


















Navigation






Home






Problem description






About






Official rules







              Leaderboard
              
            




























Problem description


Your goal is to predict how likely individuals are to receive their H1N1 and seasonal flu vaccines. Specifically, you'll be predicting two probabilities: one for 
h1n1_vaccine
 and one for 
seasonal_vaccine
.


Each row in the dataset represents one person who responded to the National 2009 H1N1 Flu Survey.








Labels


Labels






Features


List of features


Example of features










Performance metric


Example






Submission Format


Format example










Labels




For this competition, there are two target variables:




h1n1_vaccine
 - Whether respondent received H1N1 flu vaccine.


seasonal_vaccine
 - Whether respondent received seasonal flu vaccine.




Both are binary variables: 
0
 = No; 
1
 = Yes. Some respondents didn't get either vaccine, others got only one, and some got both. This is formulated as a multilabel (and 
not
 multiclass) problem.




The features in this dataset




You are provided a dataset with 36 columns. The first column 
respondent_id
 is a unique and random identifier. The remaining 35 features are described below.


For all binary variables: 
0
 = No; 
1
 = Yes.




h1n1_concern
 - Level of concern about the H1N1 flu.


0
 = Not at all concerned; 
1
 = Not very concerned; 
2
 = Somewhat concerned; 
3
 = Very concerned.






h1n1_knowledge
 - Level of knowledge about H1N1 flu.


0
 = No knowledge; 
1
 = A little knowledge; 
2
 = A lot of knowledge.






behavioral_antiviral_meds
 - Has taken antiviral medications. (binary)


behavioral_avoidance
 - Has avoided close contact with others with flu-like symptoms. (binary)


behavioral_face_mask
 - Has bought a face mask. (binary)


behavioral_wash_hands
 - Has frequently washed hands or used hand sanitizer. (binary)


behavioral_large_gatherings
 - Has reduced time at large gatherings. (binary)


behavioral_outside_home
 - Has reduced contact with people outside of own household. (binary)


behavioral_touch_face
 - Has avoided touching eyes, nose, or mouth. (binary)


doctor_recc_h1n1
 - H1N1 flu vaccine was recommended by doctor. (binary)


doctor_recc_seasonal
 - Seasonal flu vaccine was recommended by doctor. (binary)


chronic_med_condition
 - Has any of the following chronic medical conditions: asthma or an other lung condition, diabetes, a heart condition, a kidney condition, sickle cell anemia or other anemia, a neurological or neuromuscular condition, a liver condition, or a weakened immune system caused by a chronic illness or by medicines taken for a chronic illness. (binary)


child_under_6_months
 - Has regular close contact with a child under the age of six months. (binary)


health_worker
 - Is a healthcare worker. (binary)


health_insurance
 - Has health insurance. (binary)


opinion_h1n1_vacc_effective
 - Respondent's opinion about H1N1 vaccine effectiveness.


1
 = Not at all effective; 
2
 = Not very effective; 
3
 = Don't know; 
4
 = Somewhat effective; 
5
 = Very effective.






opinion_h1n1_risk
 - Respondent's opinion about risk of getting sick with H1N1 flu without vaccine.


1
 = Very Low; 
2
 = Somewhat low; 
3
 = Don't know; 
4
 = Somewhat high; 
5
 = Very high.






opinion_h1n1_sick_from_vacc
 - Respondent's worry of getting sick from taking H1N1 vaccine.


1
 = Not at all worried; 
2
 = Not very worried; 
3
 = Don't know; 
4
 = Somewhat worried; 
5
 = Very worried.






opinion_seas_vacc_effective
 - Respondent's opinion about seasonal flu vaccine effectiveness.


1
 = Not at all effective; 
2
 = Not very effective; 
3
 = Don't know; 
4
 = Somewhat effective; 
5
 = Very effective.






opinion_seas_risk
 - Respondent's opinion about risk of getting sick with seasonal flu without vaccine.


1
 = Very Low; 
2
 = Somewhat low; 
3
 = Don't know; 
4
 = Somewhat high; 
5
 = Very high.






opinion_seas_sick_from_vacc
 - Respondent's worry of getting sick from taking seasonal flu vaccine.


1
 = Not at all worried; 
2
 = Not very worried; 
3
 = Don't know; 
4
 = Somewhat worried; 
5
 = Very worried.






age_group
 - Age group of respondent.


education
 - Self-reported education level.


race
 - Race of respondent.


sex
 - Sex of respondent.


income_poverty
 - Household annual income of respondent with respect to 2008 Census poverty thresholds.


marital_status
 - Marital status of respondent.


rent_or_own
 - Housing situation of respondent.


employment_status
 - Employment status of respondent.


hhs_geo_region
 - Respondent's residence using a 10-region geographic classification defined by the U.S. Dept. of Health and Human Services. Values are represented as short random character strings.


census_msa
 - Respondent's residence within metropolitan statistical areas (MSA) as defined by the U.S. Census.


household_adults
 - Number of 
other
 adults in household, top-coded to 3.


household_children
 - Number of children in household, top-coded to 3.


employment_industry
 - Type of industry respondent is employed in. Values are represented as short random character strings.


employment_occupation
 - Type of occupation of respondent. Values are represented as short random character strings.








 Feature data example




For example, a single row in the dataset, has these values:












Field


Value










h1n1_concern


1






h1n1_knowledge


0






behavioral_antiviral_meds


0






behavioral_avoidance


0






behavioral_face_mask


0






behavioral_wash_hands


0






behavioral_large_gatherings


0






behavioral_outside_home


1






behavioral_touch_face


1






doctor_recc_h1n1


0






doctor_recc_seasonal


0






chronic_med_condition


0






child_under_6_months


0






health_worker


0






health_insurance


1






opinion_h1n1_vacc_effective


3






opinion_h1n1_risk


1






opinion_h1n1_sick_from_vacc


2






opinion_seas_vacc_effective


2






opinion_seas_risk


1






opinion_seas_sick_from_vacc


2






age_group


55 - 64 Years






education


< 12 Years






race


White






sex


Female






income_poverty


Below Poverty






marital_status


Not Married






rent_or_own


Own






employment_status


Not in Labor Force






hhs_geo_region


oxchjgsf






census_msa


Non-MSA






household_adults


0






household_children


0






employment_industry


NaN






employment_occupation


NaN












Performance metric




Performance will be evaluated according to the area under the receiver operating characteristic curve (ROC AUC) for each of the two target variables. The mean of these two scores will be the overall score. A higher value indicates stronger performance.


In Python, you can calculate this using 
sklearn.metrics.roc_auc_score
 for this multilabel setup with the default 
average="macro"
 parameter.




Submission format




The format for the submission file is three columns: 
respondent_id
, 
h1n1_vaccine
, and 
seasonal_vaccine
. The predictions for the two target variables should be 
float probabilities
 that range between 
0.0
 and 
1.0
. Because the competition uses ROC AUC as its evaluation metric, the values you submit must be the probabilities that a person received each vaccine, 
not
 binary labels.


As this is a multilabel problem, the probabilities for each row do 
not
 need to sum to one.


For example, if you predicted...












h1n1_vaccine


seasonal_vaccine






respondent_id














26707


0.5


0.7






26708


0.5


0.7






26709


0.5


0.7






26710


0.5


0.7






26711


0.5


0.7






...


...


...










The first several lines of the 
.csv
 file that you submit would look like:


respondent_id,h1n1_vaccine,seasonal_vaccine
26707,0.5,0.7
26708,0.5,0.7
26709,0.5,0.7
26710,0.5,0.7
26711,0.5,0.7
...



Good luck!




Good luck and enjoy this problem! If you have any questions you can always visit the 
user forum
! If you want some help getting started, check out the 
walkthrough
 for our benchmark model.








On this page






Labels


The features in this dataset


Performance metric


Submission format


Good luck!




















Flu Shot Learning: Predict H1N1 and Seasonal Flu Vaccines: Rules and Terms of Data Use




DrivenData Competition Rules




GUIDELINES


One account per participant


You cannot sign up to DrivenData from multiple accounts and therefore you cannot submit from multiple accounts.


Private sharing of code


Privately sharing code or data outside of teams is not permitted. 


Public dissemination of entries


DrivenData has the right to publicly disseminate any entries or models.


Open licensing of winners


Winning solutions need to be made available under The MIT License (an open source software license commonly described at 
http://opensource.org/licenses/MIT
) in order to be eligible for recognition and prize money if offered.


Documentation for winning solutions


Winning solutions must be documented using the provided Winning Model Documentation Template in order to be eligible for recognition and prize money if offered.


Submission limits


The number of submissions per day is restricted to a fixed value on a per-competition basis. Any attempt to circumvent this limit will result in disqualification.


External data


External data is not allowed unless otherwise noted explicitly on these competition pages. Participants agree to make no attempt to use additional data or data sources not provided on these competition pages.  




FULL RULES


These are the complete, official rules for the Competition (the 
"Competition Rules"
) and incorporate by reference the contents of the Competition Website listed above.


By downloading a dataset linked from the Competition Website, submitting an entry to this Competition, or joining a Team in this Competition, you are agreeing to be bound by these Competition Rules which constitute a binding agreement between you and DrivenData and, if applicable, any rules and restrictions that may be imposed by the Competition Sponsor.


The Competition is hosted by DrivenData, Inc (
"DrivenData"
). The Competition will run according to the dates listed on the Competition Website (the "Competition Period").


Each registered individual or Team is referred to as a Participant. You may only compete using a single, unique DrivenData account registered at 
http://www.drivendata.org
. Competing using more than one DrivenData account per individual is a breach of these Competition Rules and DrivenData reserves the right to disqualify any individual (or Team including an individual) who is found to breach these Competition Rules.


Eligibility


The Competition is open to all natural persons over the age of 18 at the time of entry. Legal entities and organizations are not eligible for entry. There is no purchase or donation necessary to enter the Competition.


Officers, directors, employees and advisory board members (and their immediate families and members of the same household) of the Competition Sponsor, DrivenData and their respective affiliates, subsidiaries, contractors, agents, judges and advertising and promotion agencies are not eligible to participate in the Competition.


You are not eligible to receive any Prize in the Competition if you are a resident of a country designated by the United States Treasury's Office of Foreign Assets Control.


Registration


If you meet the eligibility requirements and would like to participate, then you must first complete the registration process through the relevant competition pages on 
  (the "Competition Website") within the Competition Period. After you complete the registration process, you will receive access to the Data (described on the Competition Website) that will enable you to develop and submit one or more Entries (as defined below). All Entries must be received during the Competition Period. To register, visit the Competition Website and follow the onscreen instructions to complete and submit your registration. All of the registration information that you provide is collectively referred to as your "Account". (If you have already created an Account at 
, enter your user name and password and follow the on-screen instructions). 


After you register individually, you may join a group of other participants with which to collaborate (each group, a 
"Team"
), only if expressly permitted by these rules below, but you may register only once. If you register for the Competition more than once, you will be, and the remainder of your Team may be, disqualified in DrivenData's sole discretion.


You acknowledge and agree that you are solely responsible for abiding by your employer's policies regarding participation in the Competition. Sponsor disclaims any and all liability or responsibility for disputes arising between an employee and employer related to this Competition.


Once you have completed the registration process, you or your Team will be provided with access to the Data that you use to develop your Entries.


BY ENTERING THE COMPETITION YOU ACCEPT THE CONDITIONS STATED IN THESE OFFICIAL RULES INCLUDING THE RULES ON THE COMPETITION WEBSITE, AGREE TO BE BOUND BY THE DECISIONS OF THE JUDGES AND WARRANT THAT YOU ARE ELIGIBLE TO PARTICIPATE IN THE COMPETITION. IF YOU DO NOT ACCEPT ALL OF THESE OFFICIAL RULES, THEN PLEASE DO NOT REGISTER FOR THE COMPETITION. WE RECOMMEND THAT YOU PRINT OUT A COPY OF THESE OFFICIAL RULES FOR YOUR FUTURE REFERENCE.


Teams


FORMING A TEAM
. 
Multiple individuals or entities may collaborate as a Team. You may not participate on more than one Team. Each Team member must be a single individual operating a separate DrivenData account. You must register individually for the Competition before joining a Team. You must confirm your Team membership to make it official by responding to the Team notification message which will be sent to your Account.


TEAM PRIZES
. 
If a Team wins a monetary Prize, DrivenData will allocate the Prize money in even shares between the Team members unless the Team unanimously contacts DrivenData within three business days following the Submission deadline to request an alternative prize distribution.


Entry submissions


Each Entry must be uploaded to the Competition Website in the manner and format specified on the Competition Website. All Entries must be received during the Competition Period. An 
"Entry"
 is the data submitted in the manner and format specified on the Competition Website via the Entry form. The number of Entries a Participant may submit during each calendar day of the Competition Period will be displayed on the Competition Website. If the Competition is a multi-stage Competition with temporally separate training data and/or leaderboard data, one or more valid Entries must be submitted and selected during each stage of the Competition in the manner described on the Competition Website.


USER SUBMISSIONS MUST IN THEIR ENTIRETY COMPLY WITH ALL APPLICABLE FEDERAL, STATE, LOCAL, AND INTERNATIONAL LAWS AND REGULATIONS.  WITHOUT LIMITING THE FOREGOING, IN ORDER TO BE ELIGIBLE, YOU WARRANT THAT (UNLESS OTHERWISE SPECIFIED IN THE PROBLEM STATEMENT) YOUR SUBMISSION FOR THIS COMPETITION:




Does not include or anticipate the inclusion of any content that is in violation of or infringes third party intellectual property rights including, but not limited to copyrights, including music copyrights, patents, trade secrets, trademarks, and rights of publicity or privacy.


Is free and clear of all liens, claims, encumbrances or demands of any third parties. 


Does not include or anticipate the inclusion of any unsuitable or offensive content, including nudity, sexually explicit, disparaging, libelous or other inappropriate content. 


Has not been entered in previous challenges, or won previous awards. 


Has not been published or distributed previously in any media. 


Is suitable for a general audience. 


Does not contain any claims that are not and cannot be substantiated or that would be false and/or misleading to a reasonable consumer.




Selection of winners


This Competition is a challenge of skill and the final results are determined by evaluating a combination of quantitative and qualitative factors, as more fully described on the Competition Website. For that portion of the Competition evaluated quantitatively, the results will be determined solely by leaderboard ranking on the private leaderboard based on an objective statistical evaluation metric published on the Competition Website prior to commencement of the Competition  (subject to compliance with these Competition Rules). Participants' scores and ranks on the Competition Website at any given stage of the Competition will be based on the objective statistical evaluation metric described on the Competition Website, as determined by applying the predictions in the Submission to the ground truth of a validation dataset whose instances were a fixed set sampled from the Data. For that portion of the Competition evaluated qualitatively, the results will be determined by a panel of judges, as more fully described on the Competition Website. As more fully described on the Competition Website, the Competition may have a quantitative winner, a qualitative winner, a combined quantitative and qualitative winner, or all three.


The evaluation metric used for scoring and ranking Submissions will be displayed on the Competition Website.


Any prize awards are subject to verification of eligibility and compliance with these Competition Rules. All decisions of DrivenData, the Competition Sponsor and/or judges will be final and binding on all matters relating to this Competition. DrivenData reserves the right to examine the Submission and any associated code or documentation for compliance with these Competition Rules. In the event that the Submission demonstrates a breach of these Competition Rules, Competition Sponsor or DrivenData may at its discretion take either of the following actions:




disqualify your Submission(s); or 


require that you remediate within one week all issues identified in your Submission(s) (including, without limitation, the resolution of license conflicts, the fulfillment of all obligations required by software licenses, and the removal of any software that violates the software restrictions).




A tie between two or more valid and identically ranked submissions will be resolved in favor of the tied submission that was submitted first.


A Participant may decline to be nominated as a Winner by notifying DrivenData directly within one week following the Competition deadline, in which case the declining Participant forgoes any prize or other features associated with winning the Competition. DrivenData reserves the right to disqualify a Participant who so declines at DrivenData's sole discretion if DrivenData deems disqualification appropriate.


Prizes and conditions


If the Competition has a  prize, the Prize Winner(s) will be notified and announced within 30 days of the end of the Competition on the Competition Website.


The Prize Winner(s) will receive their prizes awarded as a check or electronic transfer from DrivenData. 


If a Team wins a prize, all Team members must submit a single written statement describing how the prize is to be allocated among the Team members. If the Team fails to submit such statement within 30 days after DrivenData requests it, then DrivenData will distribute the prize among Team members in equal shares and will have no further obligation to winning Team members.


As a condition of receipt of the prize, winner must deliver the algorithm's code and documentation to DrivenData. The source code must contain a description of resources required to build and run the algorithm. The accompanying documentation should be consistent with DrivenData's 
Winning Model Documentation Template
, which will be provided to winners within 30 days of the end of the Competition Period.


The prize may be awarded to an alternate winner if required documentation is not returned within thirty (30) days after mailing to winner, if prize notification letter/email or prize is returned as undeliverable, if winner does not respond to an email or other communication from DrivenData within ten (10) days of the date sent, or if the winner, in DrivenData’s judgment, does not respond to reasonable requests for information related to prize delivery or otherwise unable or unwilling to coordinate prize delivery within thirty (30) days after prize notification. Allow thirty (30) days for prize delivery. By accepting any prize/award, Winner agrees to allow DrivenData and/or the Competition Sponsor to disclose Winner’s first name, first initial of last name, and city of residence, as well as prize information to the extent required by law, and if so required by law, Winner agrees to the disclosure of additional personal information, all without additional compensation. 


DrivenData is responsible only for prize delivery and is not responsible for prize utility or otherwise. No substitution or transfer of prizes is permitted. All taxes, fees and expenses associated with participation in the Competition or receipt and use of a prize are the sole responsibility of the Prize Winner(s).


PARTICIPANT INTELLECTUAL PROPERTY LICENSING.

As a further condition of receipt of a Prize, each winning Participant thereby licenses their winning Submission and the source code used to generate the Submission according to the Winner License Type specified above (note: if no Winner License Type is specified above, the Winner License Type is deemed to be Non-Exclusive License).


NON-EXCLUSIVE LICENSE.

If the Winner License Type for the Competition (see Winner License Type above) is a Non-Exclusive License then each Winner by accepting a Prize thereby:




grants to Competition Sponsor and its designees a worldwide, non-exclusive, sub-licensable, transferable, fully paid-up, royalty-free, perpetual, irrevocable right to use, not use, reproduce, distribute, create derivative works of, publicly perform, publicly display, digitally perform, make, have made, sell, offer for sale and import their winning Submission and the source code used to generate the Submission, in any media now known or hereafter developed, for any purpose whatsoever, commercial or otherwise, without further approval by or payment to Participant; and


represents that he/she/it has the unrestricted right to grant that license.




OPEN SOURCE LICENSE.

If the Winner License Type for the Competition (see Winner License Type above) is Open Source License, then each Winner by accepting a Prize thereby:




licenses their winning Submission and the source code used to generate the Submission under the MIT License (an open source software license commonly described at 
http://opensource.org/licenses/MIT
); and


represents that he/she/it has the unrestricted right to grant that license.




CHEATING.
 
Participating using more than one DrivenData account is deemed cheating and, if discovered, will result in disqualification from the Competition and any other affected Competitions and may result in banning or deactivation of affected DrivenData accounts.


DrivenData reserves the right to request information associated with our investigation of suspected cheating. Failure to respond to these requests (including failure to furnish the requested information) within ten (10) days is grounds for disqualification.


RECEIVING PRIZES.

After verification of eligibility, if prizes are awarded, each Prize winner will receive the prize in the form of a check or electronic transfer made out to the Prize winner (if an individual, or to the individual Team members if a Team). Allow 30 days from final confirmation for Prize delivery. Any winners who are U.S. citizens will receive an IRS 1099 form in the amount of their prize at the appropriate time. Prize winners are responsible for any taxes, fees or other liability resulting from their receipt of a Prize.


Permissions


Except where prohibited by law, entry constitutes permission to use winners' names, hometowns and likenesses for online posting, and/or any advertising and publicity without additional compensation. Winners may also be required to sign and return a release of liability, declaration of eligibility and, where lawful, a publicity consent agreement, as conditions of receiving a prize. Failure to comply with the aforementioned conditions shall be grounds for forfeiture of a prize.


Data use and code sharing


DATA.

"Data" means the Data or Datasets linked from the Competition Website for the purpose of use by Participants in the Competition. For the avoidance of doubt, Data is deemed for the purpose of these Competition Rules to include any prototype or executable code provided to Participants by DrivenData or via the Competition Website. Participants must use the Data only as permitted by these Competition Rules and any associated data use rules specified on the Competition Website.


Unless otherwise permitted by the terms of the Competition Website, Participants must use the Data solely for the purpose and duration of the Competition, including but not limited to reading and learning from the Data, analyzing the Data, modifying the Data and generally preparing your Submission and any underlying models and participating in forum discussions on the Competition Website. Participants agree to use suitable measures to prevent persons who have not formally agreed to these Competition Rules from gaining access to the Data and agree not to transmit, duplicate, publish, redistribute or otherwise provide or make available the Data to any party not participating in the Competition. Participants agree to notify DrivenData immediately upon learning of any possible unauthorized transmission or unauthorized access of the Data and agree to work with DrivenData to rectify any unauthorized transmission. Participants agree that participation in the Competition shall not be construed as having or being granted a license (expressly, by implication, estoppel, or otherwise) under, or any right of ownership in, any of the Data.


EXTERNAL DATA.

Unless otherwise expressly stated on the Competition Website, Participants must not use data other than the Data to develop and test their models and Submissions. Competition Sponsor reserves the right in its sole discretion to disqualify any Participant who Competition Sponsor discovers has undertaken or attempted to undertake the use of data other than the Data, or who uses the Data other than as permitted according to the Competition Website and in these Competition Rules, in the course of the Competition.


CODE SHARING.

Participants are prohibited from privately sharing source or executable code developed in connection with or based upon the Data, and any such sharing is a breach of these Competition Rules and may result in disqualification.
Participants are permitted to publicly share source or executable code developed in connection with or based upon the Data, or otherwise relevant to the Competition, provided that such sharing does not violate the intellectual property rights of any third party. By so sharing, the sharing Participant is thereby deemed to have licensed the shared code under the MIT License (an open source software license commonly described at 
http://opensource.org/licenses/MIT
).


OPEN-SOURCE CODE.

A Submission will be ineligible to win a prize if it was developed using code containing or depending on software licensed under an open source license:




other than an Open Source Initiative-approved license (see 
http://opensource.org/licenses
); or


an open source license that prohibits commercial use.




Participant warranties and obligations


By registering, you agree that (a) your Account is complete, correct and accurate and (b) your registration may be rejected or terminated and all Entries submitted by you and/or your Team may be disqualified if any of the information in your Account is (or Competition Sponsor of DrivenData has reasonable grounds to believe it is) incomplete, incorrect or inaccurate. You are solely responsible for your Account. All registration information is deemed collected in the United States.


Participation is subject to all federal, state and local laws and regulations. Void where prohibited or restricted by law. You are responsible for checking applicable laws and regulations in your jurisdiction before participating in the Competition to make sure that your participation is legal. You are responsible for all taxes and reporting related to any award that you may receive as part of the Competition. You are responsible for abiding by your employer's policies regarding participation in the Competition. Competition Sponsor and DrivenData disclaim any and all liability or responsibility for disputes arising between you and your employer related to this Competition.


Each Participant is solely responsible for all equipment, including but not necessarily limited to a computer and internet connection necessary to access the Competition Website and to develop and upload any Submission, and any telephone, data, hosting or other service fees associated with such access, as well as all costs incurred by or behalf of the Entrant in participating in the Competition.


By entering a Submission, you represent and warrant that all information you enter on the Competition Website is true and complete to the best of your knowledge, that you have the right and authority to make the Submission (including any underlying code and model) on your own behalf or on behalf of the persons and entities that you specify within the Submission, and that your Submission:




complies with all applicable federal, state, local and international laws and regulations;


is your own original work, or is used by permission, in which case full and proper credit and identify is given and the third party contributions are clearly identified within your Submission;


does not contain confidential information or trade secrets and is not the subject of a registered patent or pending patent application;


does not violate or infringe upon the patent rights, industrial design rights, copyrights, trademarks, rights of privacy, publicity or other intellectual property or other rights of any person or entity;


does not contain malicious code, such as viruses, timebombs, cancelbots, worms, Trojan horses or other potentially harmful programs or other material or information; 


does not and will not violate any applicable law, statute, ordinance, rule or regulation;


does not trigger any reporting or royalty obligation to any third party; and


was not previously published and has not won any other prize/award. 




A breach of any of these warranties will result in the corresponding Submission being invalid.


Confidentiality


Confidential Information Defined.

As used in this Section, "Confidential Information" means the Competition Sponsor Materials, and any information provided by DrivenData hereunder, whether of a technical, business, or other nature (including, without limitation, information relating to a party's technology, software, products, services, designs, methodologies, business plans, finances, marketing plans, Sponsors, prospects, or other affairs), that is received by Participant. 


Exclusions.

Participant's obligations under this Section as to the disclosing party's Confidential Information does not include any information that Participant can document: (a) was known to Participant prior to receiving the same from the disclosing party in connection with this Agreement; (b) is independently developed by Participant without use of or reference to the Confidential Information of the disclosing party; (c) is acquired by Participant from another source without restriction as to use or disclosure; or (d) is or becomes part of the public domain through no fault or action of Participant.


Nondisclosure.

In consideration of the terms and conditions of this Agreement, and for other good and valuable consideration, the receipt and sufficiency of which is acknowledged, during and after the term of this Agreement Participant will: (a) use the disclosing party's Confidential Information solely for the purpose for which it is provided; (b) not disclose the disclosing party's Confidential Information to a third party unless the third party must access the Confidential Information to perform in accordance with this Agreement and the third party has executed a written agreement that contains terms that are substantially similar to the terms contained in this Section; and (c) maintain the secrecy of, and protect from unauthorized use and disclosure, the disclosing party's Confidential Information to the same extent (but using no less than a reasonable degree of care) that Participant protects its own Confidential Information of a similar nature. If Participant is required by law or by any governmental or semi-governmental agency or court to disclose the disclosing party's Confidential Information or the terms of this Agreement Participant must give prompt written notice of such requirement to the disclosing party before such disclosure and assist the disclosing party in attempting to obtain an order protecting the Confidential Information from public disclosure. 


Return of Information.

Upon request, Participant will destroy or deliver to the disclosing party all Confidential Information Participant may have in its possession or control. 


Injunctive Relief.

Participant acknowledges that any violation or threatened violation of this Section may cause irreparable injury to the other party, entitling the disclosing party to obtain injunctive relief in addition to all legal remedies.


Equipment and costs of participation


Each Participant is solely responsible for all equipment, including a computer and modem, necessary to establish a connection to the World Wide Web, access to the World Wide Web and any telephone, data, hosting or other service fees associated with such access, as well as all costs incurred by or behalf of the Participant in participating in the Competition.


Delivery and receipt of entries


DrivenData is not responsible for (a) late, lost, stolen, damaged, garbled, incomplete, incorrect or misdirected Entries or other communications, (b) errors, omissions, interruptions, deletions, defects, or delays in operations or transmission of information, in each case whether arising by way of technical or other failures or malfunctions of computer hardware, software, communications devices, or transmission lines, or (c) data corruption, theft, destruction, unauthorized access to or alteration of Entry materials, loss or otherwise. DrivenData is not responsible for electronic communications or emails which are undeliverable as a result of any form of active or passive filtering of any kind, or insufficient space in any email account to receive email messages. DrivenData disclaims any liability for damage to any computer system resulting from participation in, or accessing or downloading information in connection with, the Competition.


Reservation of rights


DrivenData, in its sole discretion, reserves the right to disqualify any person tampering with the entry process, the operation of the Web site, the competition process, or is otherwise in violation of the rules. DrivenData reserves the right at any time to disqualify a Submission from a Competition where, acting in good faith, it believes there are reasonable grounds to warrant disqualification. For example, DrivenData determination that the Submission does not provide the functionality described or required, or the Submission appears to be purposely designed to circumvent these Rules or the spirit of the Competition would be grounds for disqualification. DrivenData reserves the right to cancel, terminate or modify the competition if it is not capable of completion as planned for any reason, including infection by computer virus, bugs, tampering, unauthorized intervention or technical failures of any sort.


General release


By entering the Competition, you release and discharge the Competition Sponsor and DrivenData from any liability whatsoever in connection with the Competition or with the acceptance, possession, use or misuse of any prize including, without limitation, legal claims, costs, injuries, losses or damages, demands or actions of any kind (including, without limitation: personal injuries; death; damage to, loss or destruction of property; rights of publicity or privacy; and defamation or portrayal in a false light). The Competition Sponsor and DrivenData will not be responsible for typographical, printing or other inadvertent errors in these Official Rules or in other materials relating to the Competition. Additionally, you hereby agree to indemnify the Competition Sponsor and DrivenData from any and all losses, damages, costs, expenses, rights, claims, demands and actions (including attorney's fees and expenses for litigation and settlement), which may be brought against any one or more of them by anyone claiming to have suffered loss or damage as a result of your participation in the Competition.


Limitations of liability


By participating in the Competition, each Participant agrees that: (1) any and all disputes, claims, and causes of action arising out of or in connection with the Competition, or any prize awarded, shall be resolved individually without resort to any form of class action; (2) any claims, judgments and awards shall be limited to actual out-of-pocket costs incurred, including costs associated with entering the Competition, but in no event attorney's fees; and (3) under no circumstances will a Participant be permitted to obtain any award for, and each Participant hereby waives all rights to claim, punitive, incidental or consequential damages and any and all rights to have damages multiplied or otherwise increased and any other damages, other than damages for actual out-of-pocket expenses.


All federal, state, and local laws apply.  DrivenData, Inc. and the employees, officers, directors, shareholders, agents, representatives, affiliates, subsidiaries, and advertising, promotional and legal advisors are not responsible and shall not be liable for: (i) late, lost, delayed, damaged, misdirected, incomplete, illegible, or unintelligible entries; (ii) telephone, electronic, hardware, or software program, network, Internet, or computer malfunctions, failures, or difficulties; (iii) errors in transmission; (iv) any condition caused by events beyond the control of DrivenData, Inc. that may cause the contest to be disrupted or corrupted; (v) any injuries, losses, or damages of any kind caused by a prize or resulting from acceptance, possession, or use of a prize, or from participation in the contest; or (vi) any printing or typographical errors in any materials associated with the contest.


Disclaimer of Warranties


You understand that we cannot and do not guarantee or warrant that files available for downloading from the internet or the Competition Website will be free of viruses or other destructive code. You are responsible for implementing sufficient procedures and checkpoints to satisfy your particular requirements for anti-virus protection and accuracy of data input and output, and for maintaining a means external to our site for any reconstruction of any lost data. DRIVENDATA AND SPONSORS WILL NOT BE LIABLE FOR ANY LOSS OR DAMAGE CAUSED BY A DISTRIBUTED DENIAL-OF-SERVICE ATTACK, VIRUSES OR OTHER TECHNOLOGICALLY HARMFUL MATERIAL THAT MAY INFECT YOUR COMPUTER EQUIPMENT, COMPUTER PROGRAMS, DATA OR OTHER PROPRIETARY MATERIAL DUE TO YOUR USE OF THE WEBSITE OR ANY SERVICES OR ITEMS OBTAINED THROUGH THE WEBSITE OR TO YOUR DOWNLOADING OF ANY MATERIAL POSTED ON IT, OR ON ANY WEBSITE LINKED TO IT.


YOUR USE OF THE WEBSITE, ITS CONTENT AND ANY SERVICES OR ITEMS OBTAINED THROUGH THE WEBSITE IS AT YOUR OWN RISK. THE WEBSITE, ITS CONTENT AND ANY SERVICES OR ITEMS OBTAINED THROUGH THE WEBSITE ARE PROVIDED ON AN "AS IS" AND "AS AVAILABLE" BASIS, WITHOUT ANY WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED. NEITHER THE COMPANY NOR ANY PERSON ASSOCIATED WITH THE COMPANY NOR SPONSORS MAKES ANY WARRANTY OR REPRESENTATION WITH RESPECT TO THE COMPLETENESS, SECURITY, RELIABILITY, QUALITY, ACCURACY OR AVAILABILITY OF THE WEBSITE. WITHOUT LIMITING THE FOREGOING, NEITHER THE COMPANY NOR ANYONE ASSOCIATED WITH THE COMPANY NOR SPONSORS REPRESENTS OR WARRANTS THAT THE WEBSITE, ITS CONTENT OR ANY SERVICES OR ITEMS OBTAINED THROUGH THE WEBSITE WILL BE ACCURATE, RELIABLE, ERROR-FREE OR UNINTERRUPTED, THAT DEFECTS WILL BE CORRECTED, THAT OUR SITE OR THE SERVER THAT MAKES IT AVAILABLE ARE FREE OF VIRUSES OR OTHER HARMFUL COMPONENTS OR THAT THE WEBSITE OR ANY SERVICES OR ITEMS OBTAINED THROUGH THE WEBSITE WILL OTHERWISE MEET YOUR NEEDS OR EXPECTATIONS.


THE COMPANY HEREBY DISCLAIMS ALL WARRANTIES OF ANY KIND, WHETHER EXPRESS OR IMPLIED, STATUTORY OR OTHERWISE, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY, NON-INFRINGEMENT AND FITNESS FOR PARTICULAR PURPOSE.
THE FOREGOING DOES NOT AFFECT ANY WARRANTIES WHICH CANNOT BE EXCLUDED OR LIMITED UNDER APPLICABLE LAW.


Governing Law and Jurisdiction


DrivenData shall be the sole interpreter of these Official Rules. 


All matters relating to the Official Rules or the Competition and any dispute or claim arising therefrom or related thereto (in each case, including non-contractual disputes or claims), shall be governed by and construed in accordance with the internal laws of the Commonwealth of Massachusetts without giving effect to any choice or conflict of law provision or rule (whether of the Commonwealth of Massachusetts or any other jurisdiction).


Any legal suit, action or proceeding arising out of, or related to, the Competition or the Competition Website shall be instituted exclusively in the federal courts of the United States or the courts of the Commonwealth of Massachusetts although we retain the right to bring any suit, action or proceeding against you for breach of these Terms of Use in your country of residence or any other relevant country. You waive any and all objections to the exercise of jurisdiction over you by such courts and to venue in such courts.


The invalidity or unenforceability of any provision of these Official Rules shall not affect the validity or enforceability of any other provision. In the event that any provision is determined to be invalid or otherwise unenforceable or illegal, these Official Rules shall otherwise remain in effect and be construed in accordance with their terms as if the invalid or illegal provision was not contained herein.










I agree


Cancel







































          We run data science competitions that
          

          create
          AI solutions for social good.
        










Work with us






As a partner






As a competitor






Join a competition






Careers










About us






What we do






Who we are






Blog






Open source










Get in touch






Contact us






Mailing list






Twitter






LinkedIn



























          
            © 2025
          
          Driven Data Inc.,
          700 Colorado Blvd #611, Denver, CO 80206,
          
info@drivendata.org












Terms






Privacy






Copyright policy







































