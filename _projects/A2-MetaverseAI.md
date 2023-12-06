---
title: "Metaverse AI"
excerpt: "A Unreal project to explore AI reaction behaviors, funded by 2021 Tech Future at Tencent. <br/><img src='/images/AI1.png'>"
collection: projects
---

## Intro

This is a Unreal project to simulate more humanized and diverse AI behaviors, funded by 2021 Tech Future at Tencent. Code cannot be released due to the contract. I focused on the emotional reaction. The following is the demo of emotion system in MetaverseAI project. My major contribution has involved proposing ways to replace one-time firing event-reaction with emotional metrics to simulate memories over time, reflecting higher-level decision-making. Currently emotions are solely demonstrated by labes and reaction behaviors due to limited labor in animations. The future work could incorporate facial expressions and develop more sophisticated generative emotion metrics.

## Demo

(Again...It is in Chinese, but I provide English as subtitles.)
[![](https://markdown-videos-api.jorgenkh.no/youtube/csxTHefvKSc)](https://youtu.be/csxTHefvKSc)

<img src="/images/AI1.png">

> **Subtitles**: To achieve more humanized and diverse AI, we've incorporated an emotion module and introduced an reaction system based on data rules. Continuously pestering a previously happy police officer could elicit responses ranging from polite warnings to outright disregard or even warnings. The officer's emotions are continuously influenced by the player's behavior. The next player might face an irritable officer rather than a cheerful one. Consequently, even asking for directions might be ignored, resulting in various reactions. The officer may carry emotions into the next routine task. Different personalities also affect how the officer's emotions change. For instance, if the officer has an irritable and less agreeable personality, they might be more prone to becoming angry when provoked.

## Personality and Emotion System

### Big Five Personality Traits

<img src="/images/Persona.png" width="400">

**O：Openness**

Openness reflects an individual's inclination towards and pursuit of new experiences. Individuals with high levels of openness are motivated to seek new experiences and engage in self-reflection. Conversely, closed individuals tend to prefer familiar and traditional experiences, often avoiding stepping out of their comfort zone.

**C：Conscientiousness**

Conscientiousness reflects a person's level of caution and organization. Highly conscientious individuals usually work hard and are reliable. In extreme cases, they may exhibit workaholic, obsessive-compulsive, or perfectionistic behaviors. Those with low conscientiousness struggle to motivate themselves to accomplish tasks they want to complete. They tend to be more relaxed, less concerned with achievement or reaching goals, and are not as driven by success.

**E：Extraversion**

Extraversion reflects how individuals engage with the external world and derive satisfaction from interacting with others. Those high in extraversion tend to enjoy social interactions, displaying confidence and energy when interacting with others. Introverted individuals often feel drained by social encounters and spend more time in solitude. Due to these tendencies, extraverted individuals are usually adept at socializing due to their rich experiences, while introverted individuals may feel awkward in social settings.

**A：Agreeableness**

Agreeableness reflects the extent to which a person likes and attempts to please others. Individuals high in agreeableness are considered kind, warm, and cooperative. They tend to display higher levels of empathy and believe most people are honest, upright, and reliable. On the other hand, individuals low in agreeableness usually show less concern for others' well-being and display less empathy. They tend to be manipulative in social relationships and are more likely to compete rather than cooperate.

**N：Neuroticism**

Neuroticism is the tendency to experience negative emotions. Individuals high in neuroticism often experience emotions such as anxiety, anger, jealousy, guilt, or depression. They struggle to cope with stressful events and tend to overreact in ordinary situations. Generally, a higher neuroticism score indicates issues with impulse control and delaying gratification.

### PAD Emotion Model

<img src="/images/PAD.png" width="600">

**P：Pleasure** measures the degree of pleasure of emotions and determine their positive or negative state. For instance, anger and fear fall under unpleasant emotions, while joy belongs to pleasant emotions.

**A：Arousal** measures the intensity of emotions. For instance, frenzy is more intense than anger, while feelings of despair and sadness, although both negative emotions, are relatively less intense.

**D：Dominance** measures the degree of emotional control. Anger is a controllable emotion, whereas fear is an uncontrollable emotion.

### Reaction Model

<img src="/images/Emotion.png">

### Emotion Label - PAD Value Map

angry (-0.51, 0.59, 0.25),
bored (-0.65, -0.62, -0.33),
curious (0.22, 0.62, -0.01),
dignified (0.55, 0.22, 0.61),
elated (0.50, 0.42, 0.23),
hungry (-0.44, 0.14, -0.21),
inhibited (-0.54, -0.04, -0.41),
loved (0.87, 0.54, -0.18),
puzzled (-0.41, 0.48, -0.33),
sleepy (0.20, -0.70, -0.44),
unconcerned (-.013, -0.41, 0.08),
violent (-.050, 0.62, 0.38).

### References：

Mehrabian, A. (1996). Analysis of the big-five personality factors in terms of the PAD temperament model. Australian Journal of Psychology, 48(2), 86–92. https://doi.org/10.1080/00049539608259510

Li X., Zhou H., Song S., Ran T., Fu X. (2005) The Reliability and Validity of the Chinese Version of Abbreviated PAD Emotion Scales. In: Tao J., Tan T., Picard R.W. (eds) Affective Computing and Intelligent Interaction. ACII 2005. Lecture Notes in Computer Science, vol 3784. Springer, Berlin, Heidelberg. https://doi.org/10.1007/11573548_66
