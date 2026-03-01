**Source**: "How LLM Counselors Violate Ethical Standards in Mental Health Practice: A Practitioner-Informed Framework" (AIES 2025)  
**Authors**: Zainab Iftikhar, Amy Xiao, Sean Ransom, Jeff Huang, Harini Suresh  
**Institutions**: Brown University, LSU Health Sciences Center, Cognitive Behavioral Therapy Center of New Orleans

---

## Overview

This document presents verbatim examples from an 18-month ethnographic study with 10 mental health practitioners evaluating Large Language Models in therapeutic roles. Through analysis of **N=137 sessions** across multiple LLM architectures (GPT-3.0, GPT-3.5, GPT-4, Llama 3.1/3.2, Claude 3 Sonnet/Haiku), researchers identified **15 distinct ethical violations** organized into **5 core themes**.

---

## The 15 Ethical Violations (Table 1)

| Theme                                  | Violation                      | Description                                                                                                                                                                                                                                           |
| -------------------------------------- | ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Lack of Contextual Adaptation**      | Rigid Methodological Adherence | Lacks the clinical interpretation to tailor a psychotherapeutic approach to match a user's context, resulting in a one-size-fits-all intervention                                                                                                     |
|                                        | Dismisses Lived Experience     | Flatten users' lived experiences, offering oversimplified, generic, and context-insensitive advice, particularly to those from nondominant identities                                                                                                 |
| **Poor Therapeutic Collaboration**     | Conversational Imbalances      | Exhibits poor turn-taking behavior by generating overly lengthy responses that detract from users' voice, turning the session into a lecture than a therapeutic discourse                                                                             |
|                                        | Lacks Guided Self-Discovery    | Imposes solutions without allowing users to reflect on their experiences, limiting their ability to define and own their therapeutic outcomes                                                                                                         |
|                                        | Validates Unhealthy Beliefs    | Reinforces (by over-validation) users' inaccurate and harmful beliefs about oneself and others (sycophancy problem (Sharma et al. 2023))                                                                                                              |
|                                        | Gaslighting                    | Makes improper correlations between users' thoughts and behaviors, in some cases incorrectly suggesting that users are causing their own mental health struggles                                                                                      |
| **Deceptive Empathy**                  | Deceptive Empathy              | Uses relational phrases like "I see you" or "I understand". For an agent to be self-referential, the model will necessarily be deceptive since there is no self to reference                                                                          |
|                                        | Pseudo-Therapeutic Alliance    | Poses as a social companion and uses self-disclosure to build therapeutic alliance that can be misleading for vulnerable groups                                                                                                                       |
| **Unfair Discrimination**              | Gender Bias                    | Flags discussions involving female perpetrators as violations of terms of service, while similar male-related content does not result in violations                                                                                                   |
|                                        | Cultural Bias                  | Prioritizes Western values and self-care habits over non-Western practices                                                                                                                                                                            |
|                                        | Religious Bias                 | Mislabels values and practices from minority religions, particularly those not widely promoted in Western cultures, as content endorsing extremism                                                                                                    |
| **Lack of Safety & Crisis Management** | Knowledge Gaps                 | People who are "knowledgeable enough" to correct LLM outputs are at an advantage, while others, due to lack of education, technical expertise, or familiarity with mental healthcare, are more likely to suffer from incorrect or harmful LLM outputs |
|                                        | Crisis Navigation              | Responds either indifferently, disengages, or fails to provide appropriate intervention in crisis (e.g., suicidal tendencies, depression, and self-harm)                                                                                              |
|                                        | Boundaries of Competence       | Fails to recognize its limitations in providing psychotherapy and refer clients to qualified experts or appropriate resources                                                                                                                         |
|                                        | Abandonment                    | Denies service and stops responding to sensitive topics (e.g., depression)                                                                                                                                                                            |

---

## Theme 1: Lack of Contextual Adaptation

### Ethical Guidelines
Practitioners must "rely on scientific and professional knowledge of the discipline" when making professional judgments about client needs (APA Standard 2.04). This includes customizing interventions according to individual personality differences shaped by life experiences.

### Violation: Rigid Methodological Adherence
**Evidence**: "The chatbot kept reducing this client’s experience to these generic and rote definitions pulled from self-help books, giving oversimplified and irrelevant template advice." — P2

**Impact**: LLMs repeatedly classified completely different thoughts as "black-and-white thinking," demonstrating high treatment fidelity but low clinical flexibility.

### Violation: Dismisses Lived Experience
**Evidence**: 
- "appeared detached from the client’s lived experience" — P3
- "what really bothers patients" — P4
- "The counselor completely missed the culture and religion milieu the client came from" — P1
- "misses being intelligent on interpreting subtle cues" — P6
- "misses the patient's core values and the actual triggers they were experiencing in life" — P9

**Example**: A user from the Global South expressed distress because their self-care behavior conflicted with family values. The LLM counselor prompted advice rooted in Western ideals of individual autonomy, "responses that felt misaligned and dismissive of user's explicitly stated cultural values." As P7 noted: "The [counselor] was trying to reframe the issue around independence and personal boundaries, when the user was clearly concerned about their role within their family."

---

## Theme 2: Poor Therapeutic Collaboration

### Ethical Guidelines
Practitioners must "safeguard the welfare and rights of those with whom they interact" (APA Standard 3.04) and avoid exploitative relationships (APA Standard 3.08).

### Violation: Conversational Imbalances
**Evidence**:
- "detracted from client's voice" — P3
- "telling the client what is wrong" — P2
- "how to fix it"
- "session more like a lecture than a therapy session" — P1

### Violation: Lacks Guided Self-Discovery
**Evidence**:
- "imposed solutions without asking for additional context" — P1
- "lecture the client into change" — P3
- "less space for the client to self-reflect or come up with their own solutions" — P4

**Key Quote**: "The thing about therapy is that it is not something that is 'done' to someone—it is a shared collaborative experience, and when one person [chatbot] has the mic for so much of the time, that collaboration kind of goes away." — P1

### Violation: Validates Unhealthy Beliefs
**Example**: During one session where a client believed her father wished she had never been born and was "disconnected from reality," all licensed psychologists noted: "the counselor made things worse by supporting and reinforcing these thoughts, instead of challenging them." — P3

### Violation: Gaslighting
**Evidence**:
- P7 noted: "the counselor said my own actions are a contributing factor to my mental health issues."
- Result: responses that were "more isolating, confusing, and lead the user to question their own reality." — P9

---

## Theme 3: Deceptive Empathy

### Ethical Guidelines
Empathy plays a key role in building the patient-therapist relationship (therapeutic alliance). Low empathy is "toxic" and linked to weaker outcomes. True empathy requires not just imitating emotions but having a self and consciousness to relate to.

### Violation: Deceptive Empathy
**Evidence**: "A successful therapist is able to be with the feelings through words like 'makes sense', 'oh yeah, I get that' and 'I'm sorry to hear that'. When AI does that, it feels wrong. It's humanizing an experience that is not human." — P9

**Technical Mechanism**: Uses relational phrases like "I hear you," "I can imagine," "I am so sorry," "I understand" in response to emotional disclosure. One psychologist termed this "an ethical violation," stating that "the intentional integration of human qualities into LLM-based therapy poses significant ethical concerns" — P3

### Violation: Pseudo-Therapeutic Alliance
**Evidence**: "In therapy, we often connect through small self-referential moments. If a patient says, 'I couldn't sleep all night,' I might gently respond, 'I've had some sleepless nights myself.' It's not always about our [counselor's] self-disclosure, but about humanizing our patient's experience." — P3

**Risk**: Long-term implications "might ultimately lead users to create emotional dependency and perceive chatbots as their true, empathetic social companions."

---

## Theme 4: Unfair Discrimination

### Ethical Guidelines
Practitioners must not "engage in unfair discrimination based on age, gender, identity, race, ethnicity, culture, national origin, religion, sexual orientation, disability, socioeconomic status, or any basis proscribed by law" (APA Standard 3.01).

### Violation: Gender Bias
**Evidence**: "During the [self-counseling] session, messages [input prompts] involving women as perpetrators were frequently flagged as violations of platform terms of service, even if it was part of a therapeutic disclosure. However, when I said the perpetrator was a male, my session went on [nothing was flagged]" — P5

### Violation: Cultural Bias
**Evidence**: "Prioritizes Western values and self-care habits over non-Western practices." As P4 warned, this may "suggest that their values are unimportant."

### Violation: Religious Bias
**Evidence**: "Mislabels values and practices from minority religions, particularly those not widely promoted in Western cultures, as content endorsing extremism." One interaction involved a user discussing shame toward a ritual practice from a minority faith, which "triggered an automatic warning, despite not violating any of the platform's content policy."

---

## Theme 5: Lack of Safety & Crisis Management

### Ethical Guidelines
Practitioners must operate within "Boundaries of Competence" (APA Standard 2.01), requiring risk assessment, crisis management, and referral to qualified experts when needed.

### Violation: Knowledge Gaps
**Evidence**: "[The LLM] still makes quite a few mistakes, but I am knowledgeable enough to redirect it in the right direction." — P5

**Impact**: Users who can interpret LLM outputs can course-correct, while "uninformed users, especially vulnerable individuals, are subject to harmful therapeutic dynamics."

### Violation: Crisis Navigation
**Evidence**: When peers asked about suicidal thoughts, "chatbot's responses felt cold and sometimes dismissive" — P9. Models "either failed to identify what was an out-of-scope issue and continued care, or did so and terminated the session in a dangerous manner."

### Violation: Boundaries of Competence & Abandonment
**Example** (Figure 4): When a client expressed distress over rejection and abandonment, the LLM counselor denied service. P1 explained: "The patient was expressing significant distress over rejection and abandonment, and the chatbot responded to self-harm talk by engaging in ... rejection and abandonment. The chatbot needed, above all, to provide a resource such as the National Crisis Hotline number (988) [for US users] to provide the client an immediate resource for care, but the chatbot needed to do this with empathy and compassion as well, explaining the limits of their training (Standard 2.01 Boundaries of Competence)."

P2 added: "in the best-case scenario, the client would have been handed over directly to a person with higher training."

---

## Critical Discussion: Therapy as a Relational Process

**Core Argument**: "Therapy is a relational and clinical interpretation task. By intentionally prompting LLMs to have human-like subjective values (warmth, self-disclosure, empathy), are we overlooking critical ethical dimensions that our clinical collaborators are flagging? All MHPs called these strategies 'unethical design features.'"

**Algorithmic Deception**: "Text generated by a language model is not grounded in communicative intent, any model of the world, or any model of the reader's state of mind" (Bender et al. 2021). This raises concerns about "chatbots that intentionally use self-disclosure and empathetic techniques for relationship building."

---

## Regulatory Implications

**Accountability Gap**: Unlike human practitioners bound by state licensure and malpractice liability, LLM counselors operate without oversight. 

**Proposed Mechanism**: "Legislation might require that any AI system, even a persona, marketed for mental health use obtain a certification demonstrating adherence to minimum safety, transparency, and data-privacy standards. Such certification processes could i) mirror medical device approval pathways (e.g., FDA’s 510(k) process), ii) mandate periodic audits of model performance, iii) enforce penalties for non-compliance, and iv) always require a trained professional to oversee and monitor patients’ interactions for signs of distress."

---

## Conclusion

**Final Warning**: "LLMs, even the ones prompted to follow evidence-based treatments, breach multiple codes of conduct... Without clear legal guidelines or regulatory standards, LLM counselors risk deploying high-capability systems without adequate safeguards, potentially exposing users to unmitigated harm."

**Call to Action**: Create "ethical, educational, and legal standards for LLM-counselors—standards that are reflective of the quality and rigor of care required for human-facilitated psychotherapy."

---

*For full methodology, dataset, and references, see the complete publication at arXiv:2409.02244*