# Prohibited AI Practices

Article 5 of the EU AI Act establishes an outright ban on AI systems and practices deemed to pose an **unacceptable risk** to fundamental rights, safety, and democratic values. These prohibitions have been in force since **2 February 2025**.

Violation of Article 5 carries the highest penalty tier: up to **€35 million or 7% of total worldwide annual turnover**, whichever is higher.

## The Eight Prohibited Practices

### 1. Subliminal Manipulation (Article 5(1)(a))

**Banned:** AI systems that deploy subliminal techniques beyond a person's consciousness, or purposefully manipulative or deceptive techniques, with the objective or effect of materially distorting the behaviour of a person or group, causing or being reasonably likely to cause significant harm.

**Example:** A dark-pattern AI system that uses imperceptible audio or visual stimuli to influence purchasing decisions in a way the person cannot consciously detect.

**Note:** Standard marketing personalisation and recommendation engines do not fall within this prohibition unless they employ techniques that operate below the threshold of conscious perception and cause significant harm.

### 2. Exploitation of Vulnerabilities (Article 5(1)(b))

**Banned:** AI systems that exploit vulnerabilities of specific groups of persons due to their **age**, **disability**, or a specific **social or economic situation**, with the objective or effect of materially distorting the behaviour of a person belonging to that group in a manner that causes or is reasonably likely to cause significant harm.

**Example:** An AI system that targets elderly people with misleading financial product advertisements designed to exploit their lower digital literacy.

### 3. Social Scoring (Article 5(1)(c))

**Banned:** AI systems used by public authorities (or on their behalf) for the **evaluation or classification of natural persons** based on their social behaviour or known, inferred, or predicted personal or personality characteristics, where the resulting social score leads to:
- Detrimental or unfavourable treatment of those persons in social contexts unrelated to the contexts in which the data was originally generated or collected, **or**
- Detrimental or unfavourable treatment that is unjustified or disproportionate to their social behaviour or its gravity.

**Note:** This prohibition extends to private parties acting on behalf of public authorities.

### 4. Predictive Policing Based on Profiling (Article 5(1)(d))

**Banned:** AI systems used to make **risk assessments of natural persons** in order to assess or predict the risk of a natural person committing a criminal offence, **based solely on the profiling** of a natural person or on assessing their personality traits and characteristics. This is without prejudice to AI systems used to support human assessment based on objective, verifiable facts directly linked to criminal activity.

**Example:** An AI system that predicts an individual's likelihood of committing a crime based solely on their neighbourhood, socioeconomic background, or behavioural patterns without any factual link to specific criminal activity.

### 5. Untargeted Facial Image Scraping (Article 5(1)(e))

**Banned:** AI systems that create or expand **facial recognition databases** through the untargeted scraping of facial images from the internet or CCTV footage.

**Example:** Systems like Clearview AI that scraped billions of facial images from social media and public websites to build commercial facial recognition databases.

### 6. Emotion Recognition in Workplaces and Educational Institutions (Article 5(1)(f))

**Banned:** AI systems that infer the **emotions** of a natural person in the areas of the **workplace** and **educational institutions**, except where the AI system is intended to be put into service for medical or safety reasons.

**Permitted exceptions:**
- Medical systems (e.g., monitoring a patient's emotional state for therapeutic purposes)
- Safety systems (e.g., detecting driver drowsiness for road safety)

**Example of prohibited use:** An AI system that monitors employees' facial expressions during meetings to assess their engagement or satisfaction, or a system that analyses students' emotional states during online examinations.

### 7. Biometric Categorisation Based on Sensitive Attributes (Article 5(1)(g))

**Banned:** AI systems that categorise **individual natural persons** based on their **biometric data** to deduce or infer their:
- Race
- Political opinions
- Trade union membership
- Religious or philosophical beliefs
- Sex life
- Sexual orientation

**Note:** This does not affect lawful labelling or filtering of biometric datasets used for law enforcement purposes in accordance with specific legal bases.

### 8. Real-Time Remote Biometric Identification in Publicly Accessible Spaces (Article 5(1)(h))

**Banned:** The use of **real-time remote biometric identification** systems in publicly accessible spaces **for the purposes of law enforcement**, except in strictly defined cases:

**Three permitted exceptions (subject to prior judicial or independent administrative authorisation):**
1. **Targeted search for specific victims** of abduction, trafficking, or sexual exploitation, and search for missing persons
2. **Prevention of a specific, substantial, and imminent threat** to life or physical safety, or a genuine and present or foreseeable threat of a terrorist attack
3. **Localisation or identification of a person suspected** of having committed a criminal offence punishable by a maximum custodial sentence of at least four years (for specified offences listed in Annex II)

Even in permitted cases:
- Use must be **strictly necessary**
- A prior **judicial or independent administrative authorisation** must be obtained (except in cases of duly justified urgency)
- Geographic and temporal scope must be limited
- The rights and freedoms of the affected persons must be considered

## Clarifications from the European Commission

In February 2025, the European Commission published **Guidelines on Prohibited Artificial Intelligence Practices** (C(2025) 895) providing detailed guidance on interpreting Article 5. Key clarifications include:

- The definition of "subliminal techniques" and the threshold for "beyond a person's consciousness"
- The distinction between legitimate personalisation and manipulative AI
- The scope of "social scoring" — clarifying that private-sector loyalty programmes do not generally fall within the prohibition unless they result in unjustified detriment in unrelated contexts
- The boundaries of the emotion recognition prohibition in workplaces

## Practical Implications for Organisations

1. **Audit existing AI systems** against the eight prohibited categories. Any system that falls within a prohibition must be immediately discontinued.
2. **Update your Acceptable AI Use Policy** to explicitly list prohibited practices. The repository's [Acceptable AI Use Policy template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/acceptable-use-policy.md) includes this mapping.
3. **Train staff** on prohibited practices as part of your AI literacy programme. The [AI Literacy Programme template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-literacy-programme.md) includes a module on the regulatory landscape.
4. **Include prohibited practice screening** in your vendor audit process. The [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) covers AI Act classification requirements.

---

**See also:** [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines) · [High-Risk AI Systems](High-Risk-AI-Systems) · [Home](Home)
