# Changes

Revisión y refactorización de código, orden de jerarquía de objetos en escena y re-ordenamiento de carpetas:
- Cambio de nombre de funciones de inglés a español, no se debe mezclar idiomas (EJ Tirar_pajaro -> ThrowBird)
- Eliminación de guión bajo _ en nombre de funciones
- Eliminación de números y strings mágicos que podían ser representados por nombres de variables (EJ: +0.5f para creación de ave multiple -> + _newBirdDistance)
- Camel Case para variables privadas y públicas
- Cambio de orden de instrucciones de Scripts: Declaración de Variables -> Awake -> Start -> Udpate -> Fixed Update -> LateUpdate -> Declaración de funciones -> Declaracion de Clases anidadas
- Creación y configuración de ScriptableObjects de tipo: Bird, Enemy y Structure, para configurar la utilidad de cada una (Tipo de ave, tipo de enemigo, tipo de estructura, puntos de vida, si instancian otro GameObject)
- Eliminación de funciones poco óptimas (FindGameObjectWithTag) debido al coste de esta y reemplazo por referencias en GameManager de los prefabs o gameobjects en escena
- Creación de Singleton para GameManager (Para manejo de estados: Menu, Start, Playing, GameOver)
- Creación de CANVAS para escalado -> SCALE WITH SCREEN SIZE
- Re-ordenamiento de estructura de carpetas para mejor visualización: Scripts, escenas, prefabs.

## Installation

Install Unity 2020.3.36f1 [Unity Editor Archives](https://unity.com/releases/editor/archive) to install Unity.


## Contributing

You cand do whatever you want with this project, is open to anyone and it will be only used for PRUEBA TECNICA UNITY - ANGRY BIRDS.

Please make sure to update tests as appropriate.

## License

[GNU 3.0](https://choosealicense.com/licenses/gpl-3.0/)
