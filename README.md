# RefEval
### Basketball Referee Evaluation App

RefEval helps evaluators assess **two or three referees during the same game**, with separate observations, ratings and feedback for each referee.
Direct Link: [https://dankerschen.github.io/ref-eval/](https://dankerschen.github.io/ref-eval/)
---

## Quick start

1. Enter the match details and evaluator’s name.
2. Choose **2 or 3 referees** and enter their names.
3. Select the referee you want to evaluate.
4. Record observations during the game.
5. Complete the criteria assessment and final comments.
6. Generate and review the final crew report.
7. Export a JSON backup before closing the app.

> **Important:** Your evaluation is kept in the current browser tab.
> Export JSON before refreshing or closing the page.

---

## 1. Game setup

Enter:

- Match name.
- Competition.
- Date.
- Evaluator’s name.
- Report language: English, French or Luxembourgish.
- Number of referees and their names.

Game details and the evaluator’s name are shared across all referee evaluations.

### Select a referee

Use the referee tabs or the **Referee evaluated** selector.

The selected referee has their own:

- Observations.
- Criterion ratings and evidence.
- Overall impression.
- Individual feedback.
- Internal notes.
- Development priorities.

**Partner(s)** are automatically populated from the other referees in the crew.

> Check the selected referee before entering or dictating an observation.

---

## 2. Record an observation

1. Select the **period** using the quick buttons.
2. Enter the official **game-clock time** in `M:SS` format.
3. Select the referee’s **position**.
4. Choose an **assessment**.
5. Describe the situation and enter your remark.
6. Check the main criterion.
7. Press **Add observation**.

### Example

| Field | Entry |
|---|---|
| Period | Q2 |
| Game time | 5:23 |
| Position | Trail |
| Assessment | Positive |
| Situation | Good no-call on a drive |
| Criterion | Contact criteria |

Use **General** for an observation that does not relate to a specific game-clock time.

### Edit an observation

Press **Edit** beside a saved observation, make your changes and press **Update**.

Save or cancel an unfinished observation before switching to another referee.

---

## 3. Automatic criterion suggestions

The app uses keywords in the situation and remark to suggest a criterion.

| Remark | Suggested criterion |
|---|---|
| Missed travelling on the drive | Travelling and dribbling violations |
| Wrong out-of-bounds decision | Out-of-bounds decisions |
| Good contact criterion on the drive | Contact criteria |
| Late call on an illegal screen | Screens |

### How suggestions behave

- **One clear match:** the criterion is selected automatically.
- **Several matches:** clickable options let you choose the main criterion.
- **No clear match:** the current criterion remains unchanged and a warning appears.
- **Manual selection:** your choice is retained until you press **Use automatic suggestion**.

> Suggestions use keyword matching, not an automatic refereeing judgment.
> Always check the criterion before saving.

Automatic suggestions do not change the observation’s assessment or the referee’s criterion ratings.

---

## 4. Voice entry

Press **Speak** and describe the observation.

### Example voice command

> “Quarter two, five twenty-three, Trail, good no-call on a drive, good contact criterion.”

Then:

1. Press **Stop & review**.
2. Check the original transcript.
3. Review the suggested period, time, position, assessment and criterion.
4. Correct any inaccurate or missing information.
5. Press **Confirm & add observation**.

**Nothing is saved automatically when you finish speaking.**

### Voice-entry limitations

- Voice recognition depends on browser support and microphone permission.
- The selected report language determines the requested recognition language.
- Structured parsing supports English and basic French expressions.
- Luxembourgish-specific structured parsing is not implemented.
- Missing or unclear game times must be corrected before confirming.

If voice entry is unavailable, use **Type / paste voice transcript** or enter the fields manually.

---

## 5. Criteria assessment

Each referee has **40 independent criterion ratings**.

| Rating | Meaning |
|:---:|---|
| **+2** | Clear strength |
| **0** | Satisfactory or not specifically evaluated |
| **−2** | Minor weakness |
| **−4** | Important weakness |
| **−5** | Serious deficiency |

Add concise evidence, preferably including the period and official game-clock time.

### Suggest evidence

Press **Suggest evidence** to copy relevant recorded observations into empty evidence fields.

This feature:

- Uses observations assigned to the selected referee.
- Leaves existing evidence unchanged.
- Does not assign or change ratings.

> A rating of **0** does not, by itself, establish that the criterion was observed.

---

## 6. Final comments and report

At the end of the game, complete the selected referee’s:

- General evaluation.
- Visible comment for the referee.
- Internal review.
- Development priorities.

Repeat for each referee, then press **Generate final crew report**.

### Report contents

The combined report includes a separate section for each referee:

- Overall evaluation.
- Recorded strengths.
- Areas for development.
- Situations requiring review.
- Individual feedback.
- Development priorities.
- Chronological observations.
- Criteria ratings and evidence.
- Internal evaluator notes.

### Language and review

Generated paragraphs use local templates in English, French or Luxembourgish.

Original notes and criterion names remain in the language entered. The app does not use an AI rewriting service to translate or polish all free-text comments.

Review the wording, evidence and assessments before sharing the report.

> **Confidentiality warning**
>
> Internal evaluator notes are included in the combined report.
> Remove them before distributing the report to referees.

### Report output options

- **Copy report**
- **Download text**
- **Print / PDF**

---

## 7. Save, back up and resume

### Export JSON

Use **Export JSON** to save the complete game evaluation, including all referee records.

Export regularly, especially before:

- Refreshing the page.
- Closing the tab or browser.
- Opening an updated version of the app.

### Import JSON

Use **Import JSON** to resume a saved evaluation.

Importing replaces the current evaluation after confirmation. Export the current work first if you need to keep it.

> A report or PDF is not a replacement for a JSON backup.
> Keep the JSON file if you want to continue editing the evaluation.

---

## Privacy and practical reminders

- Evaluation data is kept in the current browser tab.
- Voice recognition may use a browser-provider service.
- Keep referee information, backups and reports private.
- Do not upload confidential evaluation files to a public GitHub repository.
- Check the selected referee before every observation.
- Use official game-clock time, not elapsed recording time.
- Review automatic suggestions before saving.
- Back up your work before leaving the app.

---

*RefEval supports the evaluator’s work. Final assessments remain the evaluator’s responsibility.*
```
