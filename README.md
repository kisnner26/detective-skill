# detective

skill para claude code que investiga casos reales con método: desapariciones, quién pudo hacer algo, mentiras e inconsistencias, fraudes, bulos, imágenes, empresas y misterios históricos.

## qué hace

- plantea una pregunta comprobable y escribe al menos tres hipótesis rivales
- gradúa fuentes y datos con la escala almirantazgo/otan (por ejemplo B2)
- compara hipótesis con una matriz ach: gana la que menos evidencia en contra tiene
- arma cronología, contradicciones y huecos
- separa hecho, inferencia y especulación, con una escala fija de confianza
- entrega un reporte con veredicto, fuentes y qué evidencia cambiaría la conclusión

## límites

- no perfila ni desanonimiza a personas privadas
- no nombra a un particular como culpable: trabaja con hipótesis
- no accede a nada protegido ni evade paywalls
- no concluye que alguien miente por su actitud, solo por contradicciones verificables
- en una desaparición o un delito en curso, primero la autoridad

## instalar

```bash
mkdir -p ~/.claude/skills/detective
curl -fsSL https://raw.githubusercontent.com/kisnner26/detective-skill/main/SKILL.md -o ~/.claude/skills/detective/SKILL.md
```

después usa `/detective` en claude code y cuéntale el caso.
