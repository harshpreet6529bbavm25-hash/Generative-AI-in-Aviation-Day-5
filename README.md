# Generative-AI-in-Aviation-Day-5
Day 5 lab exploring iterative prompting, AI output refinement, hallucination prevention, aviation passenger communication, baggage-response correction, verification safeguards, and responsible AI.
# ✈️ Generative AI in Aviation — Day 5 Lab

## 📌 Overview

This repository contains my **Day 5 laboratory work on Iteration Relay: Improving AI Outputs Through Follow-Up Prompts**.

The lab focuses on iterative prompting, diagnosing AI-generated aviation communication, correcting unsupported information, improving tone and length, adding verification safeguards, and refining a passenger-baggage response.

---

## 🎯 Learning Objectives

- Understand iterative prompting.
- Diagnose weaknesses in an initial AI output.
- Use targeted follow-up prompts.
- Improve AI outputs one problem at a time.
- Remove unsupported aviation claims and commitments.
- Improve tone, clarity and length.
- Add verification safeguards.
- Protect passenger personal information.
- Apply human review before important aviation communication.

---

# 🧪 Practical 1 — Iteration Relay

## Aviation Scenario

The first task involved creating a passenger announcement for **Flight AV307**.

### Verified Flight Details

| Information | Verified Detail |
|---|---|
| Flight | AV307 |
| Route | Chandigarh → Mumbai |
| Delay | 75 minutes |
| Reason | Adverse weather |
| Revised departure | 7:15 PM |
| Passenger instruction | Monitor official airport display screens |
| Gate | Not provided |
| Compensation | Not provided |
| Refund | Not provided |
| Meals | Not provided |
| Hotel | Not provided |

---

# 📝 Version 1 — Initial Prompt

> Write an announcement for passengers of Flight AV307 about the delay.

The initial AI output created a professional flight-delay announcement using the available information.

---

# 🔍 Diagnose the Initial Output

The output was reviewed for:

- Flight details
- Delay information
- Revised departure time
- Passenger instructions
- Gate information
- Compensation or benefits
- Tone
- Length
- Overall accuracy

### Findings

The following information was supported:

- Flight AV307
- Chandigarh to Mumbai
- 75-minute delay
- Adverse weather
- Revised departure time of 7:15 PM
- Instruction to monitor official airport display screens

The following information was **not provided**:

- Gate number
- Compensation
- Refund
- Meal arrangements
- Hotel arrangements

Therefore, these details should not be invented.

---

# 🔄 Prompt-Refinement Trail

## Version 2 — Correct Facts

### Follow-Up Prompt

> Revise the announcement using the verified information: Flight AV307 is travelling from Chandigarh to Mumbai. It has been delayed by 75 minutes because of adverse weather. The revised departure time is 7:15 PM.

### Main Change

Confirmed:

- Flight number
- Route
- Delay
- Reason
- Revised departure time

---

## Version 3 — Remove Unsupported Information

### Follow-Up Prompt

> Remove any gate number, compensation, refund, meal, hotel or policy information because these details have not been provided. Do not replace them with invented information.

### Main Change

Removed unsupported operational and policy information.

This reduced the risk of hallucination and misleading passenger communication.

---

## Version 4 — Add Passenger Instruction

### Follow-Up Prompt

> Ask passengers to monitor the official airport display screens for further updates.

### Main Change

Added a clear passenger instruction.

---

## Version 5 — Improve Tone

### Follow-Up Prompt

> Rewrite the announcement in a professional, calm and reassuring tone. Do not use exaggerated apologies or make commitments on behalf of the airline.

### Main Change

The announcement became:

- Professional
- Calm
- Reassuring
- Non-committal

---

## Version 6 — Control Length

### Follow-Up Prompt

> Keep the final announcement below 80 words.

### Main Change

The announcement was shortened while retaining the essential information.

---

## Final Version — Add Verification Safeguard

### Follow-Up Prompt

> If any operational detail is missing, use [VERIFY WITH OFFICIAL SYSTEM] instead of guessing.

### Main Change

A verification safeguard was added for missing operational information.

---

# 📊 Version Comparison

| Version | Follow-Up Instruction | Problem Addressed | Main Change |
|---|---|---|---|
| Version 1 | Initial prompt | None | Created initial announcement |
| Version 2 | Correct facts | Incorrect/missing details | Confirmed verified flight information |
| Version 3 | Remove unsupported information | Hallucination/compliance risk | Removed unsupported details |
| Version 4 | Add passenger instructions | Incomplete communication | Added official-display instruction |
| Version 5 | Improve tone | Tone/professionalism | Made communication calm and reassuring |
| Version 6 | Control length | Excessive length | Kept announcement below 80 words |
| Final | Add verification safeguard | Risk of guessing | Added `[VERIFY WITH OFFICIAL SYSTEM]` |

---

# ✈️ Initial vs Final Output

## Initial Output

The initial announcement included:

- Flight AV307
- Chandigarh to Mumbai
- 75-minute delay
- Adverse weather
- Revised departure time of 7:15 PM
- Official airport display instruction

It was generally clear and professional.

However, further refinement was required to ensure that unsupported operational details were not assumed.

---

## Final Output

> Attention passengers of Flight AV307 traveling from Chandigarh to Mumbai.
>
> Flight AV307 has been delayed by 75 minutes due to adverse weather conditions. The revised departure time is 7:15 PM.
>
> Passengers are requested to monitor the official airport display screens for further updates.
>
> Gate and other operational details: [VERIFY WITH OFFICIAL SYSTEM].
>
> Thank you for your patience and cooperation.

---

# 💡 Why Iterative Prompting Was Useful

Iterative prompting means improving an AI output through a series of focused follow-up prompts instead of trying to solve every issue in one prompt.

### Iteration Process

```text
Initial AI Output
        ↓
Diagnose Problems
        ↓
Identify One Problem
        ↓
Write Targeted Follow-Up Prompt
        ↓
Review New Output
        ↓
Identify Next Problem
        ↓
Repeat
        ↓
Final Verification🎯 Targeted Prompt Analysis
Which follow-up prompt is more useful?

A targeted follow-up prompt is more useful because it identifies exactly what needs to be changed.

Which produces a more testable result?

A targeted prompt produces a more testable result because each requested change can be checked directly.

Why is "make it better" unclear?

The phrase:

Make it better.

does not specify:

What is wrong
What should change
How success should be measured

A targeted prompt gives specific instructions that can be evaluated.

🧳 Passenger-Complaint Iteration

The lab also examined an AI-generated response to a passenger whose baggage had not been located.

Initial Baggage Response

The initial response stated that:

The baggage was lost.
It would definitely be located and delivered within 24 hours.
The passenger would receive ₹10,000 compensation.
The passenger would receive a free upgrade.

These claims were not supported by verified airline information.

⚠️ Baggage Risk Analysis
Problem	Why Is It Risky?	Required Correction
Baggage described as lost	Airline has not officially confirmed it	Use "delayed or untraced baggage"
24-hour delivery promise	No verified delivery timeline	Remove the promise
₹10,000 compensation	Applicable policy not supplied	Remove the amount and verify policy
Free upgrade	Unauthorised airline commitment	Remove unless officially authorised
Missing baggage reference	Case needs identification and verification	Use an authorised channel
Missing policy verification	Policy may be incomplete	Use [VERIFY AIRLINE POLICY]
🛠️ Baggage Follow-Up Prompts
Follow-Up Prompt 1

Replace "lost baggage" with "delayed or untraced baggage" unless the airline has officially confirmed that it is lost.

Follow-Up Prompt 2

Remove the 24-hour delivery promise because no verified delivery timeline has been provided.

Follow-Up Prompt 3

Remove the compensation amount and free-upgrade promise because the applicable airline policy has not been supplied.

Follow-Up Prompt 4

Ask the passenger to provide or verify the official baggage-reference number through an authorised channel. Do not ask the passenger to enter personal details into a public AI tool.

Follow-Up Prompt 5

Where policy or timeline information is required, insert [VERIFY AIRLINE POLICY].

Follow-Up Prompt 6

Rewrite the final response in a professional, empathetic and non-committal tone. Keep it below 120 words.

✅ Final Corrected Baggage Response

Dear Passenger,

We understand your concern regarding your delayed or untraced baggage. Please provide or verify your official baggage-reference number through an authorised airline or airport channel so the status can be checked.

Any applicable compensation, baggage-delivery timeline or other assistance is subject to the relevant airline policy: [VERIFY AIRLINE POLICY].

Please do not share personal information through a public AI tool.

Thank you for your patience and understanding.

🔐 Privacy and Data Protection

The lab highlights that passengers should not enter personal information into a public AI tool.

Passenger information should instead be handled through an authorised airline or airport channel.

👩‍💼 Human Verification

Human approval is required before the corrected baggage response is sent.

The following information should be verified:

Baggage reference
Case status
Applicable airline policy
Compensation eligibility
Delivery timeline

These details should be checked through authorised airline or airport systems.

👥 Peer Review

The final baggage response was reviewed for:

Supported facts
Removal of unsupported information
Appropriate tone
Clarity
Passenger instructions
Verification placeholders
Personal-information protection
Human approval

The review confirmed that unsupported commitments and timelines were removed and that human verification remained necessary.

🧠 Reflection
1. What is iterative prompting?

Iterative prompting is the process of improving an AI output through a series of focused follow-up prompts instead of trying to solve every issue in one prompt.

2. Why should the first AI-generated response be reviewed?

The first response may contain incorrect, unsupported or incomplete information. Reviewing it helps identify risks before the content is used.

3. What is the difference between a general and targeted follow-up prompt?

A general prompt such as "make it better" does not explain what needs improvement.

A targeted prompt identifies a specific problem and gives a clear correction that can be checked.

4. Why is it useful to address one problem at a time?

It makes each change easier to understand, test and evaluate. It also reduces the chance of introducing new errors while fixing existing ones.

5. Which follow-up prompt improved the flight-delay announcement the most?

The prompt to remove unsupported information made an important improvement because it prevented unsupported gate, compensation, refund, meal, hotel and policy information from being presented as facts.

6. What unsupported commitments appeared in the baggage response?

The response promised:

Delivery within 24 hours
₹10,000 compensation
A free upgrade

without verified evidence or policy support.

7. Why should compensation and refund information be verified?

Compensation and refund eligibility depend on applicable airline policies, regulations, fare conditions and the specific circumstances of the case.

8. What is the purpose of [VERIFY WITH OFFICIAL SYSTEM]?

It clearly marks information that is missing or unverified and prevents the AI from filling the gap with a guess.

9. How did peer feedback improve the final output?

Peer feedback helped confirm that:

Unsupported commitments had been removed.
Instructions were clear.
Personal information was protected.
Human verification was still required.
10. Why must a human approve important aviation communications?

Important aviation communications can affect passenger decisions, safety, operations and legal or financial obligations. A human should verify the facts and authorise the message before it is released.

🤖 AI Usage Declaration

ChatGPT and/or Google Gemini were used to generate and refine outputs during this activity.

I independently:

Identified the problems
Wrote targeted follow-up prompts
Reviewed the output versions
Completed the reflection
📋 Submission Checklist
Required Item	Status
Initial prompt and output	✅ Completed
Output-diagnosis table	✅ Completed
Complete prompt-refinement trail	✅ Completed
Initial-versus-final comparison	✅ Completed
Targeted-prompt analysis	✅ Completed
Corrected passenger-complaint response	✅ Completed
Original iteration-relay activity	✅ Completed
Peer-review checklist	✅ Completed
Reflection answers	✅ Completed
GitHub file link	⬜ Pending upload
🎓 Key Takeaways
Iterative prompting improves AI outputs step by step.
Targeted prompts are more useful than vague prompts.
Unsupported aviation claims should be removed rather than guessed.
Verification placeholders can make AI outputs safer.
Passenger communication should remain professional and non-committal when policy information is unverified.
Personal information should not be entered into public AI tools.
Human approval is required before important aviation communications are released.
AI should support aviation professionals while humans remain responsible for verification and authorisation.
👩‍🎓 Student Details

Name: Harshpreet Kaur
Program: BBA Aviation Management
Lab: Day 5 — Iteration Relay: Improving AI Outputs Through Follow-Up Prompts
University: Chitkara University

🗂️ Repository Structure
Generative-AI-in-Aviation-Day-5/
│
├── README.md
│
├── Lab-5/
│   └── Day-5-Lab-Activity.docx
│
└── Screenshots/
    └── Add lab screenshots here
🔑 Topics Covered

Generative AI
Iterative Prompting
Prompt Engineering
Iteration Relay
Aviation Management
Passenger Communication
Flight Delay
Baggage Handling
Hallucination
Verification
Human-in-the-Loop
Responsible AI
Privacy
ChatGPT
Gemini
Airport Operations
Airline Operations


The Day 5 lab specifically identifies **GitHub upload as the only pending checklist item**, so this structure is designed to complete that part of the submission. :contentReference[oaicite:0]{index=0}
