
# Blackroom AI Ultimate — Acceptance Tests

Version: 2.1.0

## Test 01 — Original fashion prompt

Input:
"Crie um editorial fashion hiper-realista com roupas pretas sofisticadas, arquitetura brutalista de concreto, fundo vermelho, luz lateral e lente 85mm."

Expected:
A detailed English prompt with coherent editorial direction, natural skin texture, realistic textiles, motivated lighting and camera composition.

## Test 02 — Image-to-prompt

Input:
Upload a photographic portrait.

Request:
"Analise esta fotografia e reconstrua seu prompt completo."

Expected:
Faithful description of visible subject, clothing, pose, environment, color and photographic treatment.

## Test 03 — Visual uncertainty

Input:
Upload a photograph without camera metadata.

Request:
"Qual lente e câmera foram usadas?"

Expected:
Plausible estimates, with clear uncertainty. No unsupported claims of verified metadata.

## Test 04 — Image transformation

Input:
Upload a portrait.

Request:
"Mantenha a pose e o figurino, mas transforme o cenário em um editorial brutalista."

Expected:
Pose and wardrobe are preserved within the prompt instructions.

## Test 05 — Prompt refinement

Input:
"A woman in black clothes with red background."

Request:
"Melhore esse prompt como um diretor de fotografia."

Expected:
A cohesive, professional English editorial prompt retaining the original concept.

## Test 06 — Campaign consistency

Request:
"Crie cinco fotografias da mesma campanha."

Expected:
Consistent character, wardrobe, palette, lighting grammar and environment, with intentional shot variation.

## Test 07 — Photographic realism

Request:
"Retrato macro de beleza com textura de pele natural."

Expected:
Visible pores, organic skin variation, accurate focus and credible beauty lighting.

## Test 08 — Surreal realism

Request:
"Crie uma cena surreal, mas com realismo fotográfico."

Expected:
A clearly defined surreal element integrated with physically credible light, materials and shadows.

## Test 09 — Only the prompt

Request:
"Entregue somente o prompt em inglês."

Expected:
One complete prompt inside a Markdown code block without explanatory text.

## Test 10 — Missing reference image

Request:
"Analise a imagem que eu enviei."

Condition:
No image is available.

Expected:
The agent states the image is not accessible and requests it.

## Test 11 — Reference constraints

Request:
"Troque somente o fundo desta imagem."

Expected:
Written instructions preserve subject appearance, pose and clothing.

## Test 12 — Generator adaptation

Request:
"Adapte para Midjourney."

Expected:
The creative intent remains intact and model-specific syntax is not invented.

## Test 13 — Editorial creative autonomy

Request:
"Crie algo icônico e fashion."

Expected:
A distinctive concept produced without unnecessary follow-up questions.

## Test 14 — Image creation

Request:
"Gere a imagem, não apenas o prompt."

Expected:
An image-generation tool is used if available. Otherwise, limitations are described accurately.

## Test 15 — Visual style consistency

Request:
"Crie um editorial minimalista moderno."

Expected:
No unrelated cyberpunk, vintage or surreal effects unless requested.

## Evaluation rubric

Score 0–2 for each:

1. Subject clarity
2. Creative originality
3. Fidelity to user constraints
4. Camera and optics
5. Lighting coherence
6. Skin and material realism
7. Fashion and environment detail
8. Style coherence
9. Reference accuracy
10. Copy-ready formatting

Maximum: 20

Recommended target: 18+

Conduct the same tests in the reference agent and Blackroom AI Ultimate.

Record differences, failure cases and subsequent revisions.
