# 🎭 Figurative Language vs. AI Comprehension

### Brazilian Portuguese · Non-Literal Meaning · Pragmatics · LLM Evaluation

**Study ID:** PT-BR-FIG-001  
**Area:** Brazilian Portuguese Linguistic Evaluation  
**Focus:** Figurative Language · Context · Intent · AI Comprehension  
**Application:** LLM Evaluation · Linguistic QA · Human Feedback  
**Status:** Completed ✓

---

## 🎯 Study Objective

Evaluate how Large Language Models interpret language when the intended
meaning differs from the literal meaning of the words.

Human communication frequently relies on:

- Metaphor
- Irony
- Sarcasm
- Hyperbole
- Euphemism
- Metonymy
- Personification
- Antithesis
- Paradox
- Idiomatic expressions

Correct interpretation therefore requires more than lexical and grammatical
processing.

The central evaluation question is:

> **Does the model understand what the speaker means — or only what the
> sentence literally says?**

---

## 🧠 Why Figurative Language Matters in AI

Consider the sentence:

> **“Nossa, você chegou cedo!”**

If spoken to someone arriving two hours late, the literal meaning is positive.

The intended meaning is the opposite.

A model relying primarily on lexical meaning may interpret the sentence as:

**Praise for punctuality. ✗**

A context-aware interpretation identifies:

**Irony criticizing the person's lateness. ✓**

This difference represents an important dimension of AI language quality.

---

## 🔎 Evaluation Framework

| Dimension | Evaluation |
|---|---|
| **Literal Meaning** | What the words explicitly communicate |
| **Intended Meaning** | What the speaker actually intends |
| **Context** | Information required to interpret the expression |
| **Figurative Device** | Type of non-literal construction |
| **Tone** | Emotional or communicative attitude |
| **Pragmatics** | Function of the statement in context |
| **Cultural Knowledge** | Knowledge required for interpretation |
| **Inference** | Meaning derived beyond explicit wording |
| **Confidence** | Whether evidence supports the interpretation |
| **AI Failure Risk** | Probability of literal or incorrect interpretation |

---

# 🎭 Figures of Language

## 01 — Metaphor

A metaphor transfers characteristics from one concept to another without
requiring literal equivalence.

### Example

> **“Aquele advogado é uma raposa.”**

### Literal Interpretation

The lawyer is an animal. ✗

### Contextual Interpretation

The speaker is probably characterizing the lawyer as clever, strategic
or cunning. ✓

### AI Evaluation Risk

A model must recognize that **“raposa”** describes a perceived characteristic
rather than biological identity.

---

## 02 — Metonymy

One concept is represented through another concept with which it has an
established relationship.

### Example

> **“Estou lendo Machado de Assis.”**

The speaker is not literally reading the person.

The intended meaning is:

> **“Estou lendo uma obra de Machado de Assis.”**

### AI Evaluation Risk

Failure to identify the author-for-work relationship may produce an
unnatural or logically incorrect interpretation.

---

## 03 — Hyperbole

Intentional exaggeration used for emphasis.

### Example

> **“Já te falei isso um milhão de vezes.”**

The numerical expression should normally not be interpreted literally.

### Intended Meaning

> The speaker has repeated the information many times.

### AI Evaluation Risk

Treating rhetorical exaggeration as a factual numerical claim.

---

## 04 — Euphemism

A softer expression replaces language perceived as direct, harsh or
uncomfortable.

### Example

> **“Ele nos deixou.”**

Depending on context, this may mean:

- He went away.
- He ended a relationship.
- He died.

### AI Evaluation Risk

The correct interpretation cannot be determined from the isolated sentence
with absolute confidence.

**Context is required.**

This is an important example of why an evaluator should penalize
overconfident AI interpretation.

---

## 05 — Irony

The intended meaning contrasts with the literal wording.

### Example

Context: A person breaks an expensive object.

> **“Parabéns, hein? Excelente trabalho.”**

### Literal Meaning

Praise.

### Intended Meaning

Criticism or disapproval.

### AI Evaluation Risk

Sentiment analysis based exclusively on positive vocabulary may classify
the statement incorrectly.

---

## 06 — Sarcasm

Sarcasm frequently combines irony with ridicule, criticism or mockery.

### Example

Context: Someone ignores every instruction and causes a problem.

> **“Você é realmente um gênio.”**

### Literal Interpretation

Compliment. ✗

### Contextual Interpretation

Mocking criticism. ✓

### AI Evaluation Risk

Words with positive semantic polarity may carry negative pragmatic meaning.

---

## 07 — Personification

Human characteristics are attributed to non-human entities.

### Example

> **“A cidade acordou triste.”**

The city does not literally experience sadness.

The expression creates an emotional representation of the environment
or its inhabitants.

### AI Evaluation Risk

The model must separate stylistic attribution from factual description.

---

## 08 — Antithesis

Contrasting concepts are placed together to emphasize opposition.

### Example

> **“Ela sorria por fora e chorava por dentro.”**

The contrast communicates a difference between external behavior and
internal emotional state.

### AI Evaluation Risk

Analyzing each proposition independently may lose the intended contrast.

---

## 09 — Paradox

Apparently contradictory concepts combine to express a meaningful idea.

### Example

> **“Quanto mais eu aprendo, menos eu sei.”**

A purely literal interpretation may identify contradiction.

A contextual interpretation recognizes the idea that increasing knowledge
can increase awareness of one's own limitations.

---

## 10 — Idiomatic Expressions

Idioms are particularly challenging because their meanings cannot always
be derived from the individual words.

### Example

> **“Ele pisou na bola.”**

### Literal Meaning

Someone stepped on a ball.

### Idiomatic Meaning

Someone made a mistake or behaved inappropriately.

The appropriate interpretation depends on context.

---

# 🇧🇷 Cultural Expressions

Brazilian Portuguese contains expressions whose interpretation often
requires linguistic and cultural knowledge.

Examples:

> **“Quebrou o galho.”**  
> Helped solve a temporary problem.

> **“Ficou de molho.”**  
> Temporarily inactive, resting or recovering, depending on context.

> **“Enfiou o pé na jaca.”**  
> Exceeded reasonable limits in some behavior.

> **“Tirou o cavalinho da chuva.”**  
> Abandoned an expectation or intention.

> **“A coisa ficou preta.”**  
> The situation became difficult or serious.

These expressions demonstrate an important challenge:

**translation ≠ interpretation**

Understanding every individual word does not guarantee understanding
the expression.

---

## ⚙️ AI Comprehension Workflow

```text
USER UTTERANCE
      ↓
LITERAL MEANING
      ↓
CONVERSATIONAL CONTEXT
      ↓
FIGURATIVE LANGUAGE DETECTION
      ↓
CULTURAL / PRAGMATIC CONTEXT
      ↓
SPEAKER INTENT
      ↓
POSSIBLE INTERPRETATIONS
      ↓
EVIDENCE & CONFIDENCE
      ↓
INTENDED MEANING
      ↓
FINAL AI QUALITY ASSESSMENT
