# AGENTS.md — awesome-comunidad-de-madrid

## Propósito

Selección de software open source que da **soporte específico a la Comunidad de Madrid** — su gobierno autonómico, ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es la Comunidad de Madrid: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **179 municipios** de la Comunidad de Madrid están dentro del ámbito.
- Principales ciudades: Madrid (capital), Alcalá de Henares, Móstoles, Fuenlabrada, Leganés, Getafe, Alcorcón, Torrejón de Ardoz, Parla, Alcobendas, San Sebastián de los Reyes, Pozuelo de Alarcón, Las Rozas, Coslada, Rivas-Vaciamadrid, Majadahonda, Aranjuez, Collado Villalba, San Fernando de Henares, Arganda del Rey.
- **Universidades**: UCM (Universidad Complutense de Madrid), UAM (Universidad Autónoma de Madrid), UC3M (Universidad Carlos III de Madrid), UPM (Universidad Politécnica de Madrid), URJC (Universidad Rey Juan Carlos), UAH (Universidad de Alcalá), UNED (Universidad Nacional de Educación a Distancia), Comillas (Universidad Pontificia Comillas), CEU (Universidad San Pablo-CEU), IE (IE University).
- **Instituciones**: CAM (Comunidad de Madrid), Ayuntamiento de Madrid, Metro de Madrid, EMT (Empresa Municipal de Transportes), CRTM (Consorcio Regional de Transportes de Madrid), SERMAS (Servicio Madrileño de Salud), BiciMAD, Medialab-Prado.

## Criterios de inclusión

### Incluir

- Software que interactúa con la **Comunidad de Madrid** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para el **Ayuntamiento de Madrid** u otros ayuntamientos de la comunidad.
- Software de **universidades madrileñas** (UCM, UAM, UPM, UC3M, URJC, UAH, UNED) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de la Comunidad de Madrid (datos.madrid.es, datos.comunidad.madrid).
- Software relacionado con **transporte madrileño** (Metro de Madrid, EMT, BiciMAD, CRTM, Cercanías Madrid).
- Herramientas de **calidad del aire** y medio ambiente específicas de Madrid.
- Software de **participación ciudadana** del Ayuntamiento de Madrid (Decide Madrid, CONSUL).
- Herramientas de **cartografía y SIG** específicas de la Comunidad de Madrid.
- Software sobre **turismo y patrimonio** de la región.
- Proyectos de **smart cities** para ciudades madrileñas.
- Software del **sistema sanitario madrileño** (SERMAS, hospitales).
- Software **educativo** específico de la región.
- Herramientas de **urbanismo y vivienda** de Madrid.
- Proyectos de **Medialab-Prado** que usen datos abiertos de Madrid.

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Madrid — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por madrileños que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.
- Cursos genéricos de programación impartidos en universidades madrileñas sin contenido específico de Madrid.

### Zona gris — usar criterio

- Proyectos de universidades madrileñas que podrían ser genéricos — incluir si tienen datos o configuración específica de Madrid.
- Software que cubre Madrid junto con otras regiones — incluir si Madrid es un foco principal.
- CONSUL Democracy nació en el Ayuntamiento de Madrid y se incluye por origen, aunque ahora es usado internacionalmente.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución madrileña** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-comunidad-de-madrid» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades madrileñas (Reddit, foros de universidades, Telegram de devs madrileños) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- Madrid es la capital tecnológica de España — tiene muchos más repos que otras comunidades, pero la mayoría son genéricos (empresas tech con sede en Madrid pero sin software específico de la ciudad/región).
- El **Ayuntamiento de Madrid** tiene organización GitHub `AyuntamientoMadrid` con repos de gobierno abierto, transparencia y participación ciudadana.
- **CONSUL Democracy** (consuldemocracy/consuldemocracy, 1500+ estrellas) es el proyecto estrella — plataforma de participación ciudadana nacida en el Ayuntamiento de Madrid, ahora usada en más de 100 ciudades de 35 países. Se incluye por origen madrileño.
- **PopulateTools** es una empresa madrileña con Gobierto (gobierno abierto) y herramientas de datos como gobierto-budgets-data e ine-places.
- **Medialab-Prado** tiene organización GitHub con múltiples proyectos de datos abiertos y ciencia ciudadana centrados en Madrid, pero muchos son antiguos o muy pequeños.
- **CiudadesAbiertas** es un proyecto colaborativo del Ayuntamiento de Madrid con API REST de datos abiertos.
- La búsqueda de repos de transporte es fructífera: Metro de Madrid (CRTM-NFC/Mifare-Desfire), EMT (fermartv/emt_madrid, Lorengamboa/EMT-library), BiciMAD (alexruperez/MADBike, silviluliuma/biciMAD-worker), MadridTransporte (xBaank/MadridTransporte).
- La calidad del aire de Madrid genera varios repos (Fictizia/aireMAD, medialab-prado/puremadrid) debido a los protocolos anticontaminación de Madrid Central.
- **oeg-upm/gtfs-bench** de la UPM usa datos GTFS de Madrid como benchmark para knowledge graphs.
- Las universidades madrileñas no tienen organizaciones oficiales fuertes en GitHub. La mayoría de repos son ejercicios de clase.

---

*Mantenido con [LynxPrompt](https://github.com/GeiserX/LynxPrompt) AGENTS.md framework.*
