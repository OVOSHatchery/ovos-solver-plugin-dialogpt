# <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/robot.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> DialoGPT Persona
 
Give Mycroft some sass with [DialoGPT](https://github.com/microsoft/DialoGPT)

While this can not compete with [ChatGPT Persona](https://github.com/OpenVoiceOS/ovos-solver-plugin-openai-persona) it is an offline alternative, you can use any model from huggingface to have different personas

Find models [here](https://huggingface.co/models?pipeline_tag=conversational&search=dialogpt)

## Examples 
* "What is best in life?"
* "Do you like dogs"
* "Does God exist?"


## Usage

Spoken answers api

```python
from ovos_solver_dialogpt import DialoGPTSolver

d = DialoGPTSolver({"model": "microsoft/DialoGPT-large"})
sentence = d.spoken_answer("What is best in life?")
print(sentence)
# To be alive.

sentence = d.spoken_answer("Qual é o teu animal favorito?", {"lang": "pt-pt"})
print(sentence)
# Adoro todos os animais
```
