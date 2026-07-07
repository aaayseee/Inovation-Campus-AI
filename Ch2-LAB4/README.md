# [Lab 4] General Prompt vs. Step-by-Step Instructions - A/B Comparison Lab

**Course:** Samsung Innovation Campus - Chapter 2: Prompt Engineering Basics

## Learning Goal
To experience the impact of logical sequencing by comparing a "General Prompt" with "Step-by-Step Instructions."

---

## Senaryo

İstanbul'a gideceğim sınav süreci için:
- Otel, uçak ve ulaşım giderlerini **10.000 TL bütçe** içinde tutmak
- Sınavdan önceki 3 günde toplam **15 saatlik konu tekrarını** verimli şekilde dağıtmak

Bu senaryo, aynı AI'a iki farklı prompt stiliyle (genel vs. adım adım) sorularak, sonuçların mantıksal tutarlılık ve doğruluk açısından nasıl farklılaştığını test etmek için kullanıldı.

---

## Lab 4-1: Understanding the Task and Scenario

**Mission:** Analyze a task scenario that requires multiple logical stages to identify why a single instruction might fail.

**Activity - Step-by-Step Sequence:**

> "To solve this task perfectly, the AI must first calculate fixed and variable travel costs, then allocate the remaining time for study sessions based on travel logistics, and finally integrate the budget and schedule into a cohesive plan."

**Note:** The AI is most likely to make a reasoning error at the integration step - specifically when travel time and study blocks overlap (e.g., placing study hours on exam day without knowing the exact exam time).

---

## Lab 4-2: Designing and Executing Prompt A (General)

**Mission:** Design and execute a "General Technique" prompt by providing all instructions in a single, unified block to test the AI's baseline performance.

**Prompt Used:**
> "I have a 10,000 TL budget for my 3-day trip to Istanbul for an exam. I need to fly, stay in a hotel, and use taxis. I also have 15 hours of study to complete. Create a study and budget plan that keeps me under budget while fitting in all the study hours. Give me the final plan."

**Activity - Result Evaluation:**

> "Prompt A produced a result that felt rushed and unreliable because the AI missed several specific constraints regarding the interplay between travel time and study blocks - most notably, it did not ask for the exact exam time, which meant the final study hours on Day 3 couldn't be placed with confidence."

---

## Lab 4-3: Designing and Executing Prompt B (Step-by-Step)

**Mission:** Design and execute an "Advanced Technique" prompt using Step-by-Step instructions to guide the AI's reasoning process.

**Prompt Used:**
> "Let's solve this step-by-step:
> 1. First, list the fixed costs for flights and estimate hotel/taxi costs to see the remaining budget.
> 2. Second, based on the remaining budget, suggest the most efficient transportation method between hotel and exam center.
> 3. Third, create a 3-day study schedule for the 15 hours, considering the travel time identified in Step 2.
> 4. Finally, present the full budget breakdown and the schedule together."

**Activity - Depth of Logic:**

> "By using Step-by-Step instructions, the AI was able to reason through the dependency between travel time and study availability, which was missing in the general approach of Prompt A."

---

## Lab 4-4: Comparing and Summarizing Results

**Mission:** Perform a side-by-side analysis of the outputs from both prompts to evaluate which technique delivers higher professional accuracy.

**Activity - Performance Comparison:**

> "The biggest difference was logical consistency. While Prompt A felt like a random list of suggestions, Prompt B provided a logically optimized solution because it forced the AI to finalize the travel logistics before scheduling study hours."

---

## Lab 4-5: Summarizing A/B Usage Criteria & My Own Rule

**Mission:** Synthesize findings to define exactly when to use "General" vs. "Step-by-Step" prompts in future workflows.

**Criteria:**
- **Prompt A (General):** Suitable for low-stakes, simple requests, or quick brainstorming where format doesn't matter.
- **Prompt B (Step-by-Step):** Mandatory for multi-stage logic, math/data accuracy, or professional-grade deliverables.

**Activity - Golden Rule:**

> "I will use Prompt A when I need quick brainstorming or low-stakes information and Prompt B when I need to ensure multi-step logic and data accuracy to ensure my AI outcomes are always reliable and professionally executable."

---

## Sonuç

Bu lab çalışması, aynı problemin (bütçe + çalışma planı) tek bloklu genel bir promptla mı yoksa adım adım yapılandırılmış bir promptla mı çözüldüğünde daha tutarlı sonuç verdiğini karşılaştırmıştır. Step-by-Step yaklaşım, ulaşım ve bütçe kısıtlarının çalışma programına doğru şekilde yansıtılmasını sağlayarak daha güvenilir ve uygulanabilir bir plan üretmiştir.