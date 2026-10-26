## ESPAÑOL | [ENGLISH VERSION ↓](#ENGLISH)
# Introducción a MNE-Python 🧠👨‍💻

**Tutorial exploratorio de procesamiento de datos de EEG en Python.**

> Este repositorio se encuentra en desarrollo y tiene un propósito principalmente educativo, exploratorio y de documentación metodológica. No debe interpretarse como un pipeline EEG validado, un protocolo metodológico universal ni una guía normativa para el análisis de datos neurofisiológicos.

## Propósito

Este proyecto documenta un proceso de aprendizaje y desarrollo metodológico autodirigido orientado al procesamiento de datos de EEG utilizando Python y [MNE-Python](https://mne.tools/).

El objetivo es explorar herramientas de ciencia abierta y flujos de trabajo reproducibles que permitan ampliar las posibilidades de procesamiento, visualización y análisis de datos neurofisiológicos dentro del área de las neurociencias cognitivas.

El repositorio está pensado especialmente como un recurso de aprendizaje y consulta para estudiantes, investigadores y personas en formación interesadas en comenzar a trabajar con EEG en Python.

## Contexto metodológico

Este proyecto forma parte de un proceso más amplio de desarrollo de competencias en análisis de datos neurofisiológicos. Hice parte de trabajos de investigación previos desarrollados con datos EEG que se han recolectado y usado mediante flujos de análisis establecidos utilizando el software NeuroGuide™, sus herramientas de procesamiento, filtrado y análisis, junto con herramientas y flujos de trabajo desarrollados en R.

El presente repositorio representa una línea metodológica complementaria. Su propósito no es reemplazar esos procedimientos, sino explorar una transición hacia herramientas basadas en Python y MNE-Python, con especial interés en:

* reproducibilidad;
* ciencia abierta;
* documentación explícita de las decisiones de análisis;
* automatización y programación;
* ampliación de las posibilidades de exploración y análisis de EEG.

El proceso que dio origen a este material comenzó en 2023. Después de un período de interrupción, el desarrollo se retoma durante 2025–2026 como parte de los esfuerzos por continuar desarrollando herramientas y competencias para la investigación en neurociencias cognitivas.

## Estado y alcance

Este repositorio documenta un proceso de desarrollo metodológico, no un método cerrado o validado. El material no ha sido objeto de revisión metodológica independiente ni de revisión por pares. En consecuencia, algunas decisiones de implementación, simplificaciones o elecciones de procesamiento pueden requerir corrección, ampliación o discusión según el tipo de datos, diseño experimental y objetivo científico.

Esta limitación se declara deliberadamente para distinguir entre:

1. procedimientos y recomendaciones respaldados por la literatura o la documentación oficial de las herramientas;
2. decisiones adoptadas como ejemplos pedagógicos;
3. elementos que forman parte del aprendizaje y desarrollo progresivo de este proyecto.

El objetivo de esta transparencia es evitar presentar decisiones exploratorias como recomendaciones universales.

## Referentes educativos e influencia metodológica

La estructura y parte de la secuencia pedagógica de este proyecto se inspiran en Newman et al. (2020), *Data Science for Psychology and Neuroscience - in Python* (https://neuraldatascience.io/), un recurso educativo de referencia para el aprendizaje de ciencia de datos aplicada a la psicología y las neurociencias. Actualmente se publica bajo el título *[Neural Data Science in Python](https://neuraldatascience.io/)*.

Este repositorio utiliza dicha obra como referente educativo, pero **no pretende reproducir su contenido original**. El presente proyecto desarrolla una propuesta propia, con ejemplos, explicaciones y decisiones de implementación seleccionados en función de sus objetivos educativos. No pretende traducir ni reproducir sistemáticamente el contenido de la obra original. Los fragmentos de código, recursos visuales y otros elementos que se reproducen o utilizan directamente se atribuyen en el lugar correspondiente, indicando su procedencia y las condiciones de licencia aplicables.

El tutorial también se apoya en la documentación oficial de MNE-Python y en literatura científica relacionada con el procesamiento, filtrado, referencia, detección de artefactos, análisis espectral y prácticas reproducibles en EEG. Cuando una explicación, procedimiento, ejemplo o recurso visual deriva directamente de una fuente específica, se procura identificarlo y atribuirlo en el lugar correspondiente, distinguiendo entre el contenido adaptado y las modificaciones o desarrollos propios.

## Datos

Los ejemplos incluidos en este repositorio combinan datos sintéticos preparados con fines pedagógicos y registros de acceso público. En particular, el archivo **`data/sample_eeg.edf`** contiene una señal EEG sintética, diseñada a partir de características generales del EEG y sin muestras procedentes de registros EEG de personas, para ilustrar la lectura, visualización y preparación de datos mediante MNE-Python. Asimismo, se utiliza un registro del conjunto de datos *EEG Motor Movement/Imagery Dataset* de PhysioNet, obtenido mediante las herramientas de acceso a datos de MNE-Python. Esta combinación facilita la reproducción de los ejercicios sin incorporar datos privados de investigación del proyecto, respetando las condiciones de uso y atribución de las fuentes externas.

## Idioma

Los cuadernos están escritos en **español**.

La decisión de desarrollar este recurso en español responde a un interés específico por contribuir a la disponibilidad de materiales introductorios sobre EEG, Python y MNE-Python para estudiantes e investigadores de habla hispana, especialmente en América Latina.

El idioma no pretende limitar la interacción con la comunidad internacional. Por el contrario, el proyecto busca facilitar un punto de entrada en español hacia herramientas y documentación científica que en gran medida están disponibles principalmente en inglés.

## Reproducibilidad

El objetivo del repositorio es que los ejemplos puedan ejecutarse de manera reproducible utilizando los archivos y dependencias indicados en el proyecto. Las versiones de software y las decisiones de procesamiento deben considerarse parte del contexto del análisis. MNE-Python recomienda utilizar sus propios formatos de almacenamiento y documentar adecuadamente las estructuras de datos y operaciones realizadas.

## Configuración del entorno

Este notebook fue desarrollado con Python 3.12 y MNE-Python 1.13.2.

Antes de ejecutar el notebook, instale las dependencias especificadas en `requirements.txt`:

```bash
python -m pip install -r requirements.txt
```

Las versiones completas de los paquetes utilizados se encuentran en `requirements.txt`.

## Licencia y atribución

El contenido original de este proyecto se distribuye bajo la licencia **Creative Commons Atribución-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)**. Puedes compartir y adaptar dicho contenido siempre que otorgues la atribución correspondiente, no lo utilices con fines comerciales y distribuyas las adaptaciones bajo la misma licencia, de acuerdo con sus términos.

Consulta el texto completo de la licencia: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es

Este repositorio contiene desarrollos propios y referencias a recursos de terceros. La licencia del proyecto se aplica únicamente a los materiales sobre los que el autor tiene derechos para otorgarla. Es decir, no se extiende automáticamente a los materiales de terceros. Las fuentes y atribuciones específicas se indican en el lugar pertinente del cuaderno o de la documentación.

El recurso *[Data Science for Psychology and Neuroscience - in Python](https://neuraldatascience.io/)*, de Newman et al. (2020), se utiliza como referente educativo y metodológico. Los elementos concretos reproducidos o utilizados directamente se identifican en el cuaderno. Este recurso también se distribuye bajo la CC BY-NC-SA 4.0. El uso de esta obra como referente no implica que la totalidad de este proyecto constituya una adaptación de su contenido. 

El conjunto de datos *EEG Motor Movement/Imagery Dataset* se obtiene desde PhysioNet mediante las herramientas de acceso a datos de MNE-Python. La fuente corresponde a la versión 1.0.0 del conjunto, DOI: https://doi.org/10.13026/C28G6P. Los archivos están sujetos a la Open Data Commons Attribution License v1.0 (ODC-BY 1.0), cuyas condiciones deben respetarse en los usos correspondientes.

Los restantes materiales de terceros conservan sus respectivas condiciones de licencia. Antes de reutilizar o redistribuir componentes del repositorio, se deben consultar sus atribuciones y licencias específicas.

## ENGLISH | [VERSIÓN EN ESPAÑOL ↑](#ESPAÑOL)

# Introduction to MNE-Python 🧠👨‍💻

**An exploratory tutorial on EEG data processing in Python.**

> This repository is under development and is intended primarily for educational, exploratory, and methodological documentation purposes. It should not be interpreted as a validated EEG pipeline, a universal methodological protocol, or a normative guide for neurophysiological data analysis.

## Purpose

This project documents a self-directed learning and methodological development process focused on EEG data processing using Python and [MNE-Python](https://mne.tools/).

The goal is to explore open-science tools and reproducible workflows that can expand the possibilities for processing, visualizing, and analyzing neurophysiological data in cognitive neuroscience.

The repository is intended primarily as a learning and reference resource for students, researchers, and trainees interested in beginning to work with EEG in Python.

## Methodological Context

This project is part of a broader process of developing skills in neurophysiological data analysis. I have contributed to previous research projects involving EEG data collected and analyzed using established workflows based on NeuroGuide™, including its processing, filtering, and analysis tools, as well as tools and workflows developed in R.

This repository represents a complementary methodological direction. Its purpose is not to replace those procedures, but to explore a transition toward Python-based tools and MNE-Python, with a particular interest in:

- reproducibility;
- open science;
- explicit documentation of analytical decisions;
- automation and programming;
- expanding the possibilities for EEG exploration and analysis.

The process that gave rise to this material began in 2023. After a period of interruption, development resumed during 2025–2026 as part of ongoing efforts to further develop tools and skills for cognitive neuroscience research.

## Status and Scope

This repository documents an ongoing process of methodological development rather than a finalized or validated method. The material has not undergone independent methodological review or peer review. Consequently, some implementation decisions, simplifications, or processing choices may require correction, further development, or discussion depending on the type of data, experimental design, and scientific objectives.

This limitation is stated deliberately to distinguish between:

1. procedures and recommendations supported by the literature or the official documentation of the tools;
2. decisions adopted as pedagogical examples;
3. elements that are part of the project's ongoing learning and development process.

The purpose of this transparency is to avoid presenting exploratory decisions as universal recommendations.

## Educational References and Methodological Influences

The structure and part of the pedagogical sequence of this project are inspired by Newman et al. (2020), *Data Science for Psychology and Neuroscience - in Python* (https://neuraldatascience.io/), an educational resource for learning data science applied to psychology and neuroscience. It is now published under the title *[Neural Data Science in Python](https://neuraldatascience.io/)*

This repository uses that work as an educational reference but **does not aim to reproduce its original content**. The present project develops its own approach, with examples, explanations, and implementation decisions selected according to its educational objectives. It is not intended to systematically translate or reproduce the original work. Code snippets, visual resources, and other elements that are directly reproduced or used are attributed where appropriate, with their sources and applicable licensing terms identified.

The tutorial also draws on the official MNE-Python documentation and scientific literature concerning EEG processing, filtering, referencing, artifact detection, spectral analysis, and reproducible research practices. When an explanation, procedure, example, or visual resource is directly derived from a specific source, the source is identified and attributed where appropriate, distinguishing adapted content from original modifications or developments.

## Data

The examples included in this repository combine synthetic data prepared for educational purposes with publicly available recordings.

In particular, the file **`data/sample_eeg.edf`** contains a synthetic EEG signal designed around general EEG characteristics. It does not contain samples derived from human EEG recordings and is intended to illustrate data loading, visualization, and preparation using MNE-Python.

The tutorial also uses a recording from the *EEG Motor Movement/Imagery Dataset* hosted by PhysioNet, accessed through MNE-Python's data-access tools. This combination facilitates the reproduction of the exercises without incorporating private research data from this project, while respecting the applicable terms of use and attribution requirements of external sources.

## Language

The notebooks are written in **Spanish**.

The decision to develop this resource in Spanish reflects a specific interest in contributing to the availability of introductory materials on EEG, Python, and MNE-Python for Spanish-speaking students and researchers, particularly in Latin America.

The language is not intended to limit engagement with the international community. On the contrary, the project aims to provide a Spanish-language entry point to scientific tools and documentation that are largely available in English.

## Reproducibility

The repository aims to ensure that the examples can be executed reproducibly using the files and dependencies specified in the project. Software versions and processing decisions should be considered part of the analytical context. MNE-Python recommends using its own storage formats and adequately documenting data structures and the operations performed.

## Environment Setup

This notebook was developed using Python 3.12 and MNE-Python 1.13.2.

Before running the notebook, install the dependencies specified in `requirements.txt`:

```bash
python -m pip install -r requirements.txt
```

The complete versions of the packages used are listed in `requirements.txt`.

## License and Attribution

The original content of this project is distributed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**. You may share and adapt this content provided that you give appropriate attribution, do not use it for commercial purposes, and distribute adaptations under the same license, in accordance with its terms.

Read the full license: https://creativecommons.org/licenses/by-nc-sa/4.0/

This repository contains original work and references to third-party resources. The project's license applies only to materials for which the author has the rights to grant such a license. It does not automatically extend to third-party materials. Specific sources and attributions are indicated in the relevant notebook sections or documentation.

The resource *[Data Science for Psychology and Neuroscience - in Python](https://neuraldatascience.io/)* by Newman et al. (2020) is used as an educational and methodological reference. Specific elements reproduced or directly used are identified in the notebooks.This resource is also distributed under the CC BY-NC-SA 4.0 license. Using this work as a reference does not imply that the project as a whole constitutes an adaptation of its content.

The *EEG Motor Movement/Imagery Dataset* is obtained from PhysioNet using MNE-Python's data access tools. The source corresponds to version 1.0.0 of the dataset, DOI: https://doi.org/10.13026/C28G6P. The dataset files are subject to the Open Data Commons Attribution License v1.0 (ODC-BY 1.0), whose terms must be respected in applicable uses.

Other third-party materials remain subject to their respective licensing terms. Before reusing or redistributing any components of this repository, consult their specific attributions and licenses.
