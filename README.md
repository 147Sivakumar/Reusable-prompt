# South Indian 7-Day Meal Plan

## Assignment: Learn. Build. Operate.

This project is about creating a **reusable AI prompt** that generates a healthy 7-day vegetarian South Indian meal plan.

The prompt can be reused for different people by changing only the **FOR** section, such as age, activity level, allergies, dislikes, cooking time, and goal.

## Files

```text
├── README.md
├── meal_plan_prompt.md
├── South_Indian_7_Day_Vegetarian_Meal_Plan_Age30.pdf
├── South_Indian_7_Day_Weight_Gain_Meal_Plan_Age38.pdf
├── sequential_prompting.md
├── chain_of_thought.md
├── tree_of_thought.md
└──Prompt_Engineering_Exam_Question_Paper.pdf
```
## meal_plan_prompt.md
This is the reusable prompt used to generate the meal plans.

## The prompt includes:

- AI role

- Person's details

- Vegetarian and South Indian requirements

- Allergies and dislikes

- Activity level and goal

- Local ingredients

- Cooking-time limits

- Portion sizes

- 7 days of meals

- Breakfast, lunch, snack, and dinner

- Fixed table format

- Healthy-meal guardrails

## Output Format
Every generated plan follows this format:

Day	Meal	Dish	Portion
Mon	Breakfast	Idli with sambar	3 idli + 1 cup sambar
Mon	Lunch	Rice, kootu, beans poriyal	1 cup rice + 1 cup kootu + 1/2 cup poriyal
Mon	Snack	Sundal	1 small bowl
Mon	Dinner	Vegetable dosa with chutney	2 dosa + 2 tbsp chutney

The complete plan contains 7 days × 4 meals = 28 meal entries.

## Two Test Runs
I tested the same reusable prompt with different FOR blocks.

## Run 1
South_Indian_7_Day_Vegetarian_Meal_Plan_Age30.pdf

This run was created for a 30-year-old person working towards gradual weight loss.
- [📄 View Age 30 Meal Plan](./South_Indian_7_Day_Vegetarian_Meal_Plan_Age30.pdf)
## Run 2
South_Indian_7_Day_Weight_Gain_Meal_Plan_Age38.pdf

This run used the same prompt but changed the FOR details for a 38-year-old person with a weight-gain goal.

This shows that the prompt is reusable and can produce different plans by changing the person's details without rewriting the whole prompt.
- [📄 View Age 38 Meal Plan](./South_Indian_7_Day_Weight_Gain_Meal_Plan_Age38.pdf)
## What I Changed After Testing
After the first run, I made the prompt more specific about portion sizes, South Indian dishes, local ingredients, cooking time, allergies, and the exact table format.

I also added checks to make sure all 7 days and all 4 meals per day are included.


Note
The meal plans are AI-generated drafts for this assignment and are not professional medical or dietary advice. A personalised diet plan should be prepared with a qualified dietitian or healthcare professional.for this assignment and are not professional medical or dietary advice. A personalised diet plan should be prepared with a qualified dietitian or healthcare professional.

## sequential prompting
Absolutely. Here’s a practical sequential prompting example for a branding product, where each prompt builds on the output of the previous step.

## Example: Branding a New Product — Premium Organic Coffee
Product: A premium organic coffee brand aimed at young professionals.
## The sequential structure
## Research → Strategy → Naming → Identity → Visual Design → Packaging → Marketing → Brand Review

The key idea is that each prompt explicitly uses and validates the output of the previous prompt, rather than asking one giant prompt to create the entire brand at once. This makes the process easier to control, refine, and iterate.

## Chain of thought
Chain-of-Thought (CoT) prompting example for a branding product. I'll use a fictional skincare product so the difference is clear.

Note: For CoT, it’s better to ask the model for a concise rationale or key considerations rather than requesting its private hidden chain-of-thought.

## Flow
## Customer → Positioning → USP → Personality → Name → Tagline → Visual Identity → Brand Story

This is a linear reasoning approach: one decision leads to the next.

## Tree of thought
## Tree-of-Thoughts style — Branding Product
Here, instead of following only one path, you ask the model to explore multiple branding directions, compare them, and select the strongest one.

## Flow
                    BRANDING PRODUCT
                          |
          ┌───────────────┼───────────────┐
          ↓               ↓               ↓
     Direction A      Direction B      Direction C
      Natural          Premium           Modern
          |               |               |
      Evaluate         Evaluate         Evaluate
          └───────────────┼───────────────┘
                          ↓
                   Compare & Score
                          ↓
                  Select Best Route
                          ↓
                  Final Brand Identity

## CoT vs ToT for branding
Approach	How it works	Best for
CoT	One logical path, step by step	Developing one coherent brand
ToT	Multiple possible paths are explored and compared	Choosing between different brand concepts

## Simple example:
CoT says: “Let's develop one brand carefully from start to finish.”

ToT says: “Let's develop three different brands, compare them, and choose the strongest one.”
