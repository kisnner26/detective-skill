# detective

skill para claude code que investiga casos reales con método de inteligencia y periodismo de investigación: desapariciones, quién pudo hacer algo, mentiras e inconsistencias, fraudes, bulos, imágenes, documentos, empresas, casos sin resolver.

no adivina. llega a lo que se puede demostrar, dice con qué certeza y señala lo que falta.

## método

- pregunta comprobable y al menos tres hipótesis rivales, incluida la aburrida
- fuentes primarias primero, graduadas con la escala almirantazgo/otan (B2, C3...)
- control de eco: cinco notas que copian un mismo dato cuentan como una fuente
- recálculo de fechas, edades y cifras
- matriz de hipótesis rivales (ach): gana la que menos evidencia en contra tiene
- hecho, inferencia y especulación separados, con escala fija de confianza
- lista de control de calidad antes de entregar
- reporte con veredicto, cronología, huecos, qué cambiaría la conclusión y límites del análisis

## límites

- no perfila ni desanonimiza a personas privadas
- no nombra a un particular como culpable: trabaja con hipótesis y perfiles
- no concluye que alguien miente por su actitud, solo por contradicciones verificables
- no entra a cuentas ajenas ni evade paywalls
- en una desaparición o un delito en curso, primero la autoridad

## instalar

```bash
git clone https://github.com/kisnner26/detective-skill ~/.claude/skills/detective
```

después usa `/detective` en claude code y cuéntale el caso.

## estructura

```
SKILL.md                         núcleo: límites, ciclo, grados, confianza, reporte
referencias/
  desapariciones.md              línea base, hipótesis, señales de riesgo, difusión
  autoria.md                     medios, motivo y oportunidad, perfiles en vez de nombres
  mentiras.md                    versiones sucesivas, explicaciones alternativas, etiquetas
  fraudes.md                     señales, tipologías, qué hacer si eres víctima
  material.md                    imágenes, video, documentos, empresas, juicios, ciencia
  material-usuario.md            chats, capturas, audios y fotos que aportas tú
  analisis.md                    ach, premortem, sesgos, cronología
  herramientas.md                servicios públicos de consulta por tipo de material
plantillas/
  expediente.md                  archivo de un caso para retomarlo
  ficha-desaparecido.md          parte pública para difundir y privada para la autoridad
pruebas/
  casos.md                       casos con respuesta conocida, límites y método
```

el núcleo carga siempre; los módulos solo cuando el caso los necesita.

## probar

los casos de `pruebas/casos.md` traen lo que la respuesta debe y no debe hacer. córrelos en una sesión nueva después de cada cambio.

## licencia

mit
