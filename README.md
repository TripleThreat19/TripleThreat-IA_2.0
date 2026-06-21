# TripleThreat-IA_2.0  Proyecto Orlando 🤖
---

## 🚀 Categoría: Futuros Ingenieros WRO 2026

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Diagrama%201.jpeg)


---

##  Presentación del Equipo

Desde que tenemos memoria, la robótica ha sido nuestra pasión. Somos Triple Threat, hermanos trillizos: Carlos, nuestro experto en programación; Valeria, la encargada del diario de ingeniería; y Valentina, la ingeniera mecánica detrás de cada diseño.

Hace dos años, nuestra aventura Desde que tenemos memoria, la robótica ha sido nuestra pasión. Somos Triple Threat, hermanos trillizos: Carlos, nuestro experto en programación; Valeria, la encargada del diario de ingeniería; y Valentina, la ingeniera mecánica detrás de cada diseño.

Hace tres años, nuestra aventura en la WRO comenzó en la categoría de Deportes Robóticos. No fue cualquier partido: era un tenis doble con cuatro pelotas en cada lado, una pared en contra y una rampa que agregaba una capa extra de complejidad al juego. Fue un reto estratégico donde aprendimos la importancia de la precisión y la presión del tiempo. Al año siguiente, la emoción se multiplicó cuando logramos clasificar a la etapa internacional en Turquía, una experiencia inolvidable que nos permitió medirnos en un escenario global y sumergirnos en diferentes culturas.

El año pasado, buscando un desafío que nos llevara al límite, decidimos dar el gran salto a la categoría de Futuros Ingenieros. Fue nuestra primera toma de contacto con problemas mucho más complejos, donde pudimos aplicar todo lo aprendido y evaluar nuestro crecimiento.

Este año, regresamos a Futuros Ingenieros con más fuerza, madurez y experiencia. No venimos solo a participar; volvemos para superarnos a nosotros mismos, perfeccionar nuestras estrategias y alcanzar los objetivos que nos hemos propuesto como equipo. Queremos demostrar de qué somos capaces cuando la creatividad, la lógica y nuestra complicidad como hermanos se unen para diseñar un robot que redefine sus propios límites.en la WRO comenzó en la categoría de Deportes Robóticos. No fue cualquier partido, era un tenis doble con una particularidad que lo hacía desafiante: cuatro pelotas en cada lado, una pared en contra y una rampa que agregaba una capa extra de complejidad al campo de juego. Fue un reto estratégico donde aprendimos la importancia de cada detalle, la precisión en el movimiento y la presión del tiempo. El año pasado, la emoción se multiplicó cuando, con mucho esfuerzo y dedicación, logramos clasificar para la etapa internacional en Turquía. Esa experiencia fue inolvidable: conocer a equipos de todo el mundo, sumergirnos en diferentes culturas y, sobre todo, poner a prueba nuestras habilidades en un escenario global.

Ahora, después de esas dos increíbles experiencias, queríamos un nuevo desafío, algo que nos llevara al límite. Queríamos medir hasta dónde hemos crecido, no solo individualmente, sino como equipo. Por eso, decidimos inscribirnos en la categoría de Futuros Ingenieros. Este no es solo otro concurso para nosotros; es la oportunidad perfecta para aplicar todo lo que hemos aprendido, para innovar, para enfrentarnos a problemas complejos y demostrar que nuestra pasión y nuestro trabajo en equipo son más fuertes que nunca. Queremos ver de qué somos capaces cuando la creatividad, la lógica y la camaradería se unen en un robot que redefine los límites.

---

## Diario de Ingeniería / Documentación Técnica

[![Imagen de Portada del Proyecto Orlando](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Portada1.jpeg)

Este repositorio centraliza toda la **documentación técnica** del proyecto **Orlando**, una iniciativa desarrollada por el equipo **Triple Threat** para la categoría **Futuros Ingenieros** de la **WRO 2025**. Aquí, desglosamos meticulosamente cada aspecto de nuestro robot: desde el **diseño detallado del vehículo** y la **programación del sistema de control**, hasta la **selección estratégica de componentes** y la **estructura de cableado** implementada para su óptimo funcionamiento.

Cada sección es un reflejo de nuestro **esfuerzo, dedicación y compromiso** como equipo frente a este emocionante desafío. El proyecto Orlando no es solo una solución técnica a un problema propuesto; es el culmen de incontables horas de **trabajo en equipo, investigación profunda, pruebas constantes y mejora continua**, todo impulsado por nuestra **pasión por la robótica y el aprendizaje colaborativo**.

Con este trabajo, nuestro objetivo es doble: no solo buscamos destacar en la competencia, sino también **inspirar a otros jóvenes** a sumergirse en el fascinante mundo de la ingeniería con creatividad, disciplina y un entusiasmo inquebrantable. ¡Esperamos que este diario sea una fuente de aprendizaje y motivación!

---

---

# Problema Identificado: Vehículo Autónomo para Competición "Time Attack" (WRO Futuros Ingenieros)

## Desafío del Reto

El desafío de la World Robot Olympiad (WRO) 2026 exige el desarrollo integral de un vehículo robotizado a escala que emule los sistemas de asistencia y navegación de un automóvil autónomo real. El robot debe completar tres vueltas al circuito en el menor tiempo posible, adaptándose de forma puramente reactiva a un entorno dinámico y desconocido que cambia antes de cada carrera.

## Problemas Clave a Resolver
Hemos desglosado el reto en tres pilares mecánicos y algorítmicos fundamentales:

### 1. Navegación en Carril y Control Dinámico de Velocidad
* **Seguimiento Óptimo de Trayectoria:** El vehículo debe trazar las líneas fronterizas de la pista con absoluta fluidez. No basta con mantenerse en el carril; el algoritmo debe calcular transferencias de peso y radios de giro eficientes durante las múltiples vueltas para mitigar subvirajes o sobrevirajes.

* **Control de Velocidad Adaptativo:** Implementar una lógica que module la potencia de los motores de tracción en función de la lectura de curvatura, permitiendo aceleraciones máximas en rectas largas y frenados controlados antes de entrar al vértice de los giros.

### 2. Percepción y Evasión de Obstáculos Variables (Muros y Pilares)

* **Mapeo Reactivo de Muros Interiores:** La configuración de las paredes del circuito varía de manera aleatoria. El robot no puede depender de mapas estáticos pregrabados; requiere una detección de proximidad en tiempo real que calcule zonas libres de colisión sobre la marcha.

* **Clasificación Visual de Señales de Tránsito:** Reconocimiento cromático de pilares (Verdes: giro a la izquierda / Rojos: giro a la derecha). El sistema de visión artificial debe filtrar ruidos de iluminación del entorno, identificar los objetos con precisión matemática y recalcular la trayectoria con el margen suficiente para evitar penalizaciones por desplazamiento de obstáculos.

#### Desafío de Señales de Tráfico (Pilares Verdes/Rojos):
* **Reconocimiento Visual de Señales:** Implementar un sistema fiable para detectar y diferenciar los pilares verdes (girar a la izquierda) y rojos (girar a la derecha).
* **Decisión y Maniobra Basada en Señal:** El robot debe ajustar su posición en el carril según la señal detectada, ejecutando la maniobra con precisión para no desplazar los pilares.

### 3. Secuencia de Estacionamiento en Paralelo Automatizado

* **Anclaje y Detección de Zona de Aparcamiento:** Al finalizar el ciclo de vueltas, el robot debe escudriñar los laterales de la pista para localizar el recuadro designado.

* **Cinemática de Maniobra en Espacio Confinado:** Ejecutar de forma secuencial y matemática una maniobra de reversa con dirección angular acotada para encajar el vehículo de forma perfecta en el espacio reducido, deteniendo el temporizador por completo de acuerdo a las normativas vigentes.

## 🎯 Nuestro Enfoque Tecnológico
Para afrontar la rigurosidad de la temporada 2026, nuestro proyecto integra una arquitectura de procesamiento en dos niveles:

Subsistema de Percepción Visual: Utilizaremos una Raspberry Pi AI Camera dedicada exclusivamente a la captura de fotogramas a alta velocidad, el filtrado de color y la detección de obstáculos mediante redes neuronales optimizadas en el chip de inteligencia artificial.

Cerebro de Control Central: El procesamiento lógico recaerá en una Raspberry Pi, la cual recibirá las coordenadas espaciales de la cámara, fusionará las lecturas con el resto de la arquitectura de sensores, resolverá las máquinas de estado del software y comandará el motor de dirección y tracción trasera para asegurar trayectorias milimétricas y veloces.

---

## 🛠️ Factor de Ingeniería / Diseño del Prototipo

---

## 1. Mecánica del Robot

El diseño mecánico se enfoca en una estructura **robusta y ligera**, optimizada para la distribución del peso y la integración de todos los componentes electrónicos y motrices.

### 1.1. Componentes Clave

* **Chasis**: Es la columna vertebral del robot, diseñada para soportar de manera rígida todos los componentes electrónicos y mecánicos bajo las fuerzas de aceleración de la competencia. Para esta temporada, hemos desarrollado un enfoque de construcción híbrido:
  
   La estructura base está modelada utilizando piezas y conectores LEGO, aprovechando su versatilidad y capacidad de iteración rápida. Esta base se complementa de forma estratégica con componentes de diseño propio impresos en 3D. Estas piezas personalizadas actúan como adaptadores estructurales y soportes específicos para la cámara y los sensores, garantizando una alineación milimétrica que el sistema comercial no permite y asegurando una rigidez estructural óptima sin comprometer la ligereza del vehículo.
  
* **Tren de Rodaje**: Se compone de un mínimo de cuatro ruedas. Las **ruedas delanteras** son las encargadas de la **dirección**, mientras que las **ruedas traseras** actúan como propulsoras, brindando el empuje necesario para el movimiento. 

---

## 2. Sistema de Dirección

El sistema de dirección es fundamental para la **maniobrabilidad** del robot, imitando el principio de un automóvil. Se basa en el movimiento angular de las **ruedas delanteras**.

### 2.1. Componentes Principales

* **Esqueleto y Chasis Base (LEGO EV3):** Toda la estructura portante y el esqueleto del vehículo están construidos utilizando vigas y conectores del kit LEGO EV3. Esto nos proporciona una plataforma ligera, altamente modular y fácil de reparar en la zona de pits ante cualquier imprevisto.

* **Ruedas Delanteras Direccionales:** Diseñadas para rotar sobre un eje vertical emulando el sistema de manguetas y pivotes de un automóvil real. Ambas ruedas están interconectadas mecánicamente para moverse en un ángulo simétrico y coordinado, garantizando la estabilidad del vehículo en curvas de alta velocidad.

* **Mecanismo de Dirección y Actuador:** Consiste en una barra de acoplamiento rígida que une los bloques de dirección de ambas ruedas. Para accionar este mecanismo, utilizamos el motor pequeño del kit LEGO EV3. Este motor fue seleccionado por su excelente resolución en el control de posición angular y su torque óptimo, permitiendo cambios de dirección fluidos, rápidos y con un margen mínimo de holgura (backlash).

* **Soportes e Integración de Componentes (Diseño 3D):** Debido a que las piezas comerciales no ofrecen un acople directo para la electrónica avanzada, modelamos y fabricamos piezas personalizadas en impresión 3D con dos propósitos críticos:

* **Anclaje de la Cámara:** Un soporte rígido diseñado específicamente para la Cámara Raspberry Pi AI, asegurando que el ángulo de visión de la IA se mantenga fijo y libre de las vibraciones mecánicas del motor de tracción.

* **Alojamiento de la Electrónica:** Bahías de montaje a medida para sujetar firmemente la Raspberry Pi 5 al esqueleto de LEGO, protegiendo las conexiones y optimizando la distribución de peso (centro de gravedad bajo).

* **Unidad de Procesamiento Central (Raspberry Pi 5):**Es el cerebro lógico del robot. Procesa los datos visuales de la cámara en tiempo real, calcula el error de trayectoria en la pista y envía las instrucciones de corrección angular directamente al motor pequeño de LEGO EV3 para ejecutar giros milimétricos.
---

## 3. Funcionamiento General

Para que el robot pueda moverse y girar eficientemente, el sistema opera de la siguiente manera:

* **Propulsión**: Los motores acoplados a las **ruedas traseras** (o un motor diferencial para ambas) giran para impulsar el robot hacia adelante o hacia atrás. La velocidad se regula mediante la potencia suministrada a estos motores.

* **Dirección**: Para iniciar un giro, la Rasberry PI 5 envía una señal al **motor mediano del EV3**. El motor, a su vez, activa el mecanismo de dirección, lo que provoca el cambio en el ángulo de las **ruedas delanteras direccionales**. El grado de giro de estas ruedas determina directamente el radio de giro del robot.

* **Coordinación**: La clave para un movimiento óptimo reside en la **coordinación** entre la velocidad de las ruedas propulsoras y el ángulo de las **ruedas delanteras direccionales**. Para ejecutar giros cerrados, las ruedas delanteras se angulan más, y la velocidad de las ruedas traseras puede ajustarse para facilitar la maniobra y asegurar un giro suave y controlado.

---

Este diseño, meticulosamente modelado en **3D**, permite una visualización detallada y una optimización exhaustiva de la ergonomía, la resistencia y la funcionalidad del robot antes de proceder con su construcción física. Esto asegura un rendimiento óptimo en todos los aspectos de su mecánica y dirección.


---

## Debate Técnico sobre la Gestión de la Movilidad

## 1. Arquitectura de Hardware y Desafíos de Integración

Para lograr un rendimiento óptimo en formato *Time Attack*, el vehículo requiere un mapa de profundidad local de alta frecuencia. Hemos integrado tres sensores ópticos multizona avanzados para construir un sistema de visión perimetral reactivo.

### Especificaciones del Sensor

* **Modelo:** STMicroelectronics VL53L5CX (Sensor de tiempo de vuelo *Time-of-Flight* multizona).
* **Principio Físico:** El dispositivo emite un pulso láser VCSEL infrarrojo invisible y mide el intervalo temporal del rebote del fotón. Esto genera una matriz geométrica bidimensional de lecturas de distancia de hasta **64 puntos independientes (grilla de 8x8)**, actuando como un LiDAR de estado sólido de estado sólido en miniatura.

### Trade-Offs (Compromisos) de Diseño y Gestión de Bus

Durante la fase de diseño técnico, priorizamos la disponibilidad de pines GPIO en la **Raspberry Pi 5** para la comunicación con los controladores de los motores LEGO EV3. Debido a esto, **prescindimos de los pines de interrupción física (INT)** de los sensores.

> ⚠️ **Implicación en el Software:** Esta decisión nos obligó a implementar un método de adquisición por **Polling** (muestreo cíclico activo). Para evitar que esta consulta constante sature el bus I2C y degrade el tiempo de ciclo de la CPU, desarrollamos una gestión asimétrica de la frecuencia de muestreo.

---

## 2. Gestión Eléctrica y Protocolo de Inicialización (Remapeo I2C)

El emparejamiento de tres sensores idénticos introduce dos problemas críticos: caídas de tensión por consumo síncrono y colisión de direcciones de red. Resolver esto desde el hardware fue vital para cumplir con los estándares de confiabilidad de la WRO 2026.

### Robustez Eléctrica y Control de Estados

* **Topología de Estrella Pasiva:** Las líneas de alimentación VCC (3.3V) y GND se distribuyen en paralelo desde un nodo regulado central hacia cada sensor individual, eliminando los bucles de tierra y los picos de caída de tensión (*brownouts*) cuando los tres arreglos de diodos láser se activan simultáneamente.
* **Líneas de Control Digital (Pines LPn):** Dado que todos los sensores VL53L5CX vienen configurados de fábrica con la misma dirección esclava I2C (`0x29`), implementamos un control secuencial de encendido utilizando los pines GPIO 6, 13 y 19 de la Raspberry Pi para conmutar el estado de bajo consumo (*Low Power* - LPn).
* **Mitigación del Pin Flotante:** Para evitar estados lógicos indeterminados debido a la alta impedancia de los cables largos, el software de la Raspberry Pi fuerza resistencias *pull-down* de forma interna al arrancar. Esto asegura que un sensor sin conexión explícita permanezca apagado en lugar de actuar como un dispositivo "zombi" que corrompa el bus.

### Algoritmo Lógico de Arranque e Identificación de Dispositivos

Para inicializar el bus I2C de forma segura, el software ejecuta la siguiente máquina de estados secuencial:

```
[INICIO] -> Forzar Pines LPn (GPIO 6, 13, 19) a LOW (0V) -> [Bus I2C Vacío]
               |
               v
[PASO 1] -> Conmutar GPIO 6 (Izquierdo) a HIGH (3.3V) -> Despierta en 0x29 -> Reconfigurar software a dirección 0x30
               |
               v
[PASO 2] -> Conmutar GPIO 13 (Frontal) a HIGH (3.3V)   -> Despierta en 0x29 -> Reconfigurar software a dirección 0x31
               |
               v
[PASO 3] -> Conmutar GPIO 19 (Derecho) a HIGH (3.3V)   -> Despierta en 0x29 -> Se mantiene fijo en dirección 0x29

```

---

## 3. Lógica de Navegación Asimétrica para Cinemática Ackermann

A diferencia de los robots de tracción diferencial, nuestro chasis utiliza **geometría de dirección Ackermann** (conducción tipo coche). El vehículo no puede rotar sobre su propio eje; se desplaza trazando arcos circulares continuos. Esto exige que la telemetría se adapte a la cinemática del robot, distribuyendo la carga de procesamiento de forma asimétrica.

### A. Control Lateral y Vector de Centrado (Sensores Izquierdo 0x30 / Derecho 0x29)

* **Configuración Operativa:** Resolución espacial de 4x4 zonas a una frecuencia de **60 Hz**.
* **Justificación Cinematográfica:** A velocidades competitivas de *Time Attack* (superiores a 1.2 m/s), la desviación lateral del robot debe corregirse de inmediato para evitar colisiones contra las líneas fronterizas de la pista. Reducir la matriz a 16 puntos nos permite maximizar la tasa de refresco a 60 Hz, entregando datos de baja latencia directamente al bucle del control PID que ajusta el ángulo del motor mediano de dirección LEGO EV3. Esto suprime las oscilaciones de trayectoria y el efecto de zigzagueo en las rectas.

### B. Análisis Topológico Frontal y Predictor de Evasión (Sensor Frontal 0x31)

* **Configuración Operativa:** Resolución espacial máxima de 8x8 zonas a una frecuencia de **15 Hz**.
* **Justificación Cinematográfica:** El sensor frontal está destinado a la toma de decisiones estratégicas de mediano alcance. Necesitamos la resolución completa de 64 píxeles para calcular el perfil geométrico de los muros y la signatura cromática de los pilares (Verde/Rojo). Esta densidad de datos permite estimar matemáticamente el **Tiempo para la Colisión (TTC)**. El vehículo puede planificar anticipadamente el radio de curvatura óptimo para esquivar el obstáculo sin necesidad de clavar los frenos, asegurando que el tren trasero (motor grande LEGO EV3) limpie el obstáculo con fluidez.

---

## 4. Pipeline de Procesamiento de Señal y Capa de Filtrado en Python

Para cumplir con los criterios de innovación de software de la WRO 2026, las lecturas crudas del sensor (*raw data*) se someten a un procesamiento matemático estricto en la Raspberry Pi 5 para mitigar falsos positivos provocados por reflejos ópticos de la pista o cambios bruscos de iluminación.

```
[Datos Crudos ToF] 
       |
       v
[Filtro de Descarte] -----------> Ignorar valores 'None' o distancias superiores a 4000 mm
       |
       v
[Mediana Espacial 3x3] ---------> Elimina ruido por fotones dispersos o polvo en suspensión
       |
       v
[Segmentación por Densidad] ----> Agrupa píxeles contiguos para aislar el volumen del obstáculo
       |
       v
[Histéresis Temporal] ----------> Valida la persistencia del obstáculo durante 'N' frames antes de actuar
       |
       v
[Comando de Dirección] ---------> Salida limpia hacia el actuador de dirección LEGO EV3

```

### Implementación del Procesamiento Matemático

1. **Filtro de Mediana Espacial (Ruido de Disparo):** Para evitar que lecturas espurias (píxeles aislados con caídas drásticas de distancia causadas por el sol o polvo) induzcan maniobras evasivas falsas, aplicamos una ventana kernel de $3 \times 3$ sobre la matriz. El valor central se reemplaza por la mediana de sus vecinos, homogeneizando la lectura del entorno.
2. **Segmentación y Extracción de Características (Clustering):** El software agrupa los sectores espaciales cuyas distancias relativas presenten una varianza mínima. Mediante un algoritmo simplificado de proximidad por densidad, definimos las fronteras físicas de un pilar, calculando su centro de masa o centroide espacial para determinar con precisión cuántos centímetros de desviación angular requiere el chasis para evadirlo.
3. **Filtro de Histéresis Temporal (Memoria de Estado):** Debido al método de *Polling*, un error de lectura en el bus I2C podría generar un cuadro vacío (*frame* perdido). Para evitar que el sistema interprete esto como una pista libre y enderece las ruedas en medio de una maniobra de evasión, el software retiene el estado físico del obstáculo durante al menos 3 ciclos de reloj antes de decretar que la zona está despejada.

---

## 5. Conclusión 

Nuestra arquitectura de control de movilidad demuestra una clara separación de responsabilidades entre hardware y software. El chasis híbrido (LEGO EV3 y soporte impreso en 3D) provee una plataforma estructuralmente rígida y térmicamente estable, permitiendo que la potencia matemática de la Raspberry Pi 5 sea aprovechada en su totalidad. Mediante este enfoque reactivo y asimétrico, mitigamos las debilidades del bus de datos físico para transformarlo en un sistema de posicionamiento dinámico y predictivo de alta velocidad, diseñado específicamente para dominar las exigencias de la temporada de Futuros Ingenieros 2026.


### Control del Movimiento (Actuadores):

* **Motor Grande LEGO EV3 (Propulsión y Tracción Trasera):** El encargado de la aceleración y velocidad punta del robot es el motor grande de EV3, el cual está acoplado directamente al eje de las ruedas traseras. Este motor no solo destaca por su alto torque y capacidad de respuesta rápida en rectas de Time Attack, sino que integra un encoder óptico interno de alta resolución. Este encoder nos proporciona retroalimentación (feedback) en tiempo real sobre los grados de rotación exactos de las ruedas, una información fundamental para calcular la velocidad angular, estimar la distancia recorrida mediante odometría y asegurar un control de velocidad de lazo cerrado preciso.

* **Motor Mediano LEGO EV3 (Mecanismo de Dirección):** En sustitución de un servomotor convencional, hemos implementado el motor mediano de EV3 para ejecutar el movimiento angular de las ruedas delanteras. A pesar de ser un motor de rotación continua, su diseño compacto, menor peso y la precisión de su encoder interno nos permiten programarlo para que actúe con la exactitud de un servomotor de alta gama.

* **Control y Lógica desde la Raspberry Pi 5:** La Raspberry Pi 5 traduce las decisiones de trayectoria de la cámara de IA en comandos específicos para estos dos motor.
  
 Al motor mediano (dirección) se le envían comandos de posición basados en los grados del encoder para colocar las ruedas delanteras en el ángulo de giro milimétrico que se requiere en cada curva.

Al motor grande (tracción) se le modula la potencia y velocidad de forma dinámica (acelerando a fondo en rectas y aplicando freno motor antes de entrar al vértice de los giros) para exprimir al máximo el tiempo de vuelta sin derrapar.

* **Puente H:** Funciona como la interfaz de potencia entre la Raspberry Pi 5 y los motores grande y mediano del EV3,  Permite a la Pi controlar la dirección y la velocidad de los motores (mediante PWM) con señales de bajo voltaje.


Percepción del Entorno (Sensores):

## 📷 Subsistema de Percepción Visual y Telemetría Láser

Para garantizar una navegación de alta velocidad en el formato *Time Attack*, el vehículo utiliza un sistema de percepción híbrido que combina visión artificial por transferencia de redes neuronales y un arreglo de sensores de rango láser activo.

### 1. Raspberry Pi AI Camera (Sensor Visual Principal)
Conectada de forma nativa a la Raspberry Pi 5, esta unidad constituye el núcleo de la percepción semántica y cromática del entorno. Su procesamiento se divide en tres tareas críticas:
* **Reconocimiento Cromático y Clasificación:** Identificación en tiempo real de los pilares de señalización (Verde/Rojo) mediante el aislamiento de espacios de color y filtrado de contornos.
* **Segmentación de Trayectoria:** Detección predictiva de los límites de las líneas de la pista para anticipar la curvatura del circuito antes de que el chasis ingrese a ella.
* **Inferencia en el Borde (Edge AI):** Al contar con un chip de aceleración de inteligencia artificial integrado en la propia cámara, la Raspberry Pi 5 queda libre de la carga del procesamiento de imágenes raw, permitiéndole usar el hilo principal de la CPU exclusivamente para la lógica de control.

### 2. Arreglo Multizona de Sensores ToF VL53L5CX (Sensores Láser Activos)
Como complemento crítico a la cámara de IA, implementamos una arquitectura de **Triple LiDAR de estado sólido** utilizando tres sensores *Time-of-Flight* STMicroelectronics VL53L5CX (configurados asimétricamente en direcciones I2C `0x29`, `0x30` y `0x31`). 
* **Mapeo de Proximidad:** Mientras la cámara clasifica *qué* objetos hay en la pista, este arreglo láser genera una matriz de profundidad geométrica de hasta 64 puntos independientes (grilla de 8x8) para medir con precisión milimétrica *a qué distancia exacta* se encuentran los muros y obstáculos, blindando al robot contra cambios imprevistos en la iluminación ambiental.

---

## 💻 Arquitectura de Software y Lógica de Control

Todo el ecosistema de hardware es gobernado centralizadamente por un firmware modular desarrollado en **Python**, el cual se ejecuta sobre el sistema operativo de la Raspberry Pi 5. 

El pipeline de ejecución del software sigue una arquitectura orientada a objetos que se divide en tres etapas cíclicas:


```

[Adquisición de Datos] -> (AI Camera + Matriz ToF I2C + Encoders EV3)
|
v
[Pipeline de Filtrado] -> (Mediana Espacial + Clustering + Histéresis Temporal)
|
v
[Lazo de Control PID]  -> (Cálculo de Error de Trayectoria y Radio Ackermann)
|
v
[Actuación Física]     -> (Comandos de Grados/Velocidad a Motores LEGO EV3)

```

### Funciones Principales del Software:

1.  **Fusión de Sensores (Sensor Fusion):** El script principal sincroniza las coordenadas de los obstáculos detectados por la **Raspberry Pi AI Camera** con las lecturas de distancia de los sensores **VL53L5CX**, validando la existencia real de un pilar antes de iniciar una maniobra.
2.    **Odometría de Lazo Cerrado:** Lee constantemente los *encoders* ópticos internos integrados en el **motor grande LEGO EV3 (tracción trasera)**. Esto permite calcular por integración matemática la distancia recorrida y ajustar dinámicamente la velocidad lineal para no perder tracción.
3..  **Control Cinemático Ackermann:** Calcula el error de centrado respecto al carril y ejecuta un algoritmo de control PID para enviar comandos de posición angular precisos al **motor mediano LEGO EV3 (dirección delantera)**, erradicando holguras y asegurando trayectorias fluidas a velocidades competitivas.

---

# 🤖 Sistema de Rueda y Eje para Nuestro Robot ⚙️

¡Bienvenidos a la sección de hardware de nuestro proyecto! Aquí explicaremos cómo se ensamblan las piezas clave para el movimiento de nuestro robot. La imagen de arriba muestra un "despiece" de los componentes esenciales que conforman una de las unidades de rueda.

---

### Visión General del Ensamblaje

Este sistema está diseñado para proporcionar una rotación fluida y robusta, fundamental para la locomoción de nuestro robot. Cada componente juega un papel crucial en la durabilidad y eficiencia del movimiento.

Es importante destacar que este diseño en particular está pensado para las ruedas delanteras de nuestro robot, actuando como las ruedas directrices. Esto significa que estas unidades serán responsables de la dirección del vehículo. Las ruedas traseras, por su parte, serán las que vayan impulsadas directamente por un motor, complementando este sistema para mejorar significativamente la movilidad y la capacidad de maniobra de nuestro vehículo.

---

# 🤖 Distribución de Componentes en el Chasis del Robot ⚙️

Nuestro chasis ha sido meticulosamente diseñado para una distribución específica de componentes, buscando optimizar el centro de gravedad y facilitar el proceso de montaje. A continuación, detallamos la ubicación estratégica de los elementos principales:

---

### Colocación de Componentes Clave:

* **Motor Grande LEGO EV3 (Propulsión Trasera):** Se ubica y fija firmemente en la sección posterior del esqueleto de LEGO. Esta posición concentra el peso sobre el eje motriz, optimizando la tracción de las ruedas traseras y maximizando el agarre en las rectas de alta velocidad para evitar derrapes.
* **Motor Mediano LEGO EV3 (Actuación de Dirección):** Se sitúa en la parte frontal del chasis, acoplado directamente al mecanismo de barra de dirección. Su diseño compacto y peso reducido permiten una respuesta angular inmediata sobre el eje delantero sin sobrecargar el morro del vehículo.
* **Baterías (Fuente de Energía):** Se colocan de forma simétrica en el centro geométrico del chasis, aseguradas mediante los soportes personalizados impresos en 3D. Esta disposición es crucial para mantener un centro de gravedad bajo y una distribución equilibrada del peso ($50/50$ entre ambos ejes), mejorando drásticamente la estabilidad en curvas.
* **Regulador de Voltaje (UBEC / Buck Converter):** Situado típicamente en la zona central cerca de las baterías. Su función es reducir y estabilizar el voltaje de la batería principal (por ejemplo, a $5\text{V}$ constantes) para alimentar de forma segura la Raspberry Pi 5 y los sensores ToF, protegiendo la electrónica de control contra picos de corriente.
* **Puente H (Driver de Motores):** Este componente clave se monta lo más próximo posible a los motores LEGO EV3. Su cercanía minimiza la longitud del cableado, lo que reduce la resistencia eléctrica, evita caídas de tensión y optimiza el control de velocidad (PWM) y sentido de giro dictado por la Raspberry Pi 5.
* **Soporte Frontal Vertical (Cámara y Módulo):** Esta estructura, parte del segundo piso o conectada a él, está diseñada específicamente para montar la cámara y su módulo adicional en la parte frontal elevada. Su posición estratégica garantiza un campo de visión despejado y alto, crucial para tareas como la detección de obstáculos, navegación y mapeo ambiental.
* **Raspberry PI:** se destinará el espacio para la Raspberry Pi. Esta ubicación es fundamental para mantener el "cerebro" del robot (Raspberry Pi) y su fuente de energía suplementaria (Pilas) accesibles, a la vez que se optimiza el cableado y se minimiza la altura total, contribuyendo al centro de gravedad general del conjunto.


🤖 Ensamblaje del Robot: Distribución de Componentes en el Chasis ⚙️
Nuestro chasis ha sido meticulosamente diseñado para una distribución estratégica de componentes, buscando optimizar el centro de gravedad, la funcionalidad y la facilidad de montaje. A continuación, detallamos la ubicación pensada para los elementos clave:



---

Disposición de Componentes de Percepción y Procesamiento (Segundo Piso):

Estos componentes vitales para la inteligencia y operación del robot se alojarán en una placa superior o "segundo piso", que se montará sobre el chasis principal, aprovechando estructuras como las mostradas en "Elemento 11.jpg".

---

# Electrónica

---

Nuestro sistema electrónico, que impulsa y controla cada movimiento de nuestro robot, está cuidadosamente ensamblado con los siguientes elementos clave:
-	Raspberry Pi 5
-	Raspberry Pi AI Camera
-	Motor Mediano EV3
-	Motor Grande EV3
-	Puente H
- Regulador de Voltaje
-	Baterías
-	Switch
-	STMicroelectronics VL53L5CX 

  
A continuación, se presentará el Diagrama de Cableado que ilustra cómo estos componentes se interconectan para funcionar en armonía.

![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/Diagrama%20de%20Cableado.jpg)

Explicación del Diagrama Expuesto

Raspberry Pi: Es la computadora principal del sistema. Recibe información de algunos componentes y envía órdenes a otros.

Power Bank: Este es la fuente de energía exclusiva para la Raspberry Pi. Le suministra la electricidad necesaria para funcionar.

Baterías: Estas baterías son la fuente de energía exclusiva para los motores. Suministran electricidad al Módulo Regulador de Voltaje y al Módulo de Driver de Motor.

Módulo de Driver de Motor: Este módulo se conecta a la Raspberry Pi (para recibir órdenes) y a las baterías (para obtener energía). Se usa específicamente para controlar el motor DC con encoder.

Servo Motor: Este motor puede moverse a posiciones específicas y se controla a través del drive.

Motor DC con Encoder: Este es un motor que gira continuamente, y el "encoder" le permite a la Raspberry Pi saber exactamente qué tan rápido está girando o qué posición tiene. También se controla a través del driver del motor.

Módulo Regulador de Voltaje: Este módulo toma la energía de las baterías (las rojas) y la ajusta a un voltaje específico que necesita el servomotor, asegurando que reciba la cantidad correcta de energía de manera estable. 

Cámara: Esta cámara se conecta directamente a la Raspberry Pi. Permite a la Raspberry Pi "ver" y capturar imágenes o video.

****
---

### 💡 Componentes del Vehículo

Hemos seleccionado cuidadosamente cada componente para asegurar el máximo rendimiento y fiabilidad de nuestro robot. A continuación, detallamos los elementos esenciales que dan vida a nuestro proyecto.

#### 🧠 Raspberry Pi 5

La **Raspberry Pi 5** es el cerebro de nuestro sistema, definida por la misma Raspberry Pi Foundation como una **PC de bajo coste del tamaño de una tarjeta de crédito**. Permite explorar el mundo de la informática y aprender lenguajes de programación como Scratch y Python, siendo una herramienta increíblemente versátil.

---
**_Características Destacadas:_**

* **CPU de alto rendimiento:** Procesador Broadcom BCM2712 Quad-core Arm Cortex-A76 a 2.4 GHz, ofreciendo un gran poder de procesamiento.
* **GPU avanzada:** GPU VideoCore VII para capacidades gráficas y de procesamiento de visión mejoradas.
* **Memoria RAM generosa:** Disponible con hasta 8GB de RAM LPDDR4X-4267, ideal para multitarea y aplicaciones exigentes.
* **Conectividad versátil:** Incluye Wi-Fi 5 de doble banda, Bluetooth 5.0 y Gigabit Ethernet para una comunicación robusta.
* **Almacenamiento de alta velocidad:** Soporte para tarjetas microSD de alta velocidad y una interfaz PCIe 2.0 x1 para SSDs M.2 externos (vía adaptador).
* **Salida de video dual:** Dos puertos micro HDMI que soportan hasta 4K a 60Hz.
* **Puertos USB 3.0:** Dos puertos USB 3.0 para conectar periféricos de alta velocidad.
* **Conectores MIPI duales:** Dos transceptores MIPI de 4 carriles para hasta dos cámaras o pantallas.
* **Control de ventilador:** Conector dedicado para un ventilador PWM, asegurando un rendimiento óptimo bajo cargas intensas.

---

La **Raspberry Pi 5** es ideal para nuestro robot por su **gran potencia de procesamiento para IA y visión**, lo que nos permite implementar algoritmos complejos. Su **amplia RAM** asegura una multitarea eficiente y su **conectividad avanzada** facilita la comunicación. Además, el **almacenamiento SSD ultrarrápido** y los **conectores MIPI duales para cámaras** son fundamentales para la percepción y toma de decisiones en tiempo real, garantizando un robot de **alto rendimiento y gran fiabilidad**.

![Raspberry Pi 5](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/raspberry-pi-5.jpg)

#### 🔌 Puente H

Un **Puente H** es un circuito electrónico crucial que nos permite **invertir la polaridad de la tensión** aplicada a una carga, comúnmente un motor de corriente continua. Esto se logra mediante la disposición de cuatro interruptores (transistores o relés) que permiten el flujo de corriente en dos direcciones opuestas, controlando así el sentido de giro del motor.

---
**_Características Esenciales:_**

* **Control del sentido de giro:** Permite invertir la polaridad del voltaje aplicado a un motor codificador Óptico, facilitando su rotación hacia adelante o hacia atrás.
* **Control de velocidad:** Al integrar una señal de Modulación por Ancho de Pulso (PWM), puede variar la velocidad del motor de manera eficiente.
* **Capacidad de corriente y voltaje:** Cada Puente H está diseñado para manejar un rango específico, crucial para que coincida con los requisitos del motor y evitar daños.
* **Protecciones integradas:** Muchos puentes H comerciales incluyen protecciones contra sobrecorriente, cortocircuitos y sobrecalentamiento, aumentando la seguridad y durabilidad.
* **Compatibilidad con microcontroladores:** Son fácilmente controlables por microcontroladores como la Raspberry Pi o Arduino, simplificando la lógica de control del motor.
* **Aislamiento y protección del microcontrolador:** Actúa como una interfaz de potencia, protegiendo los componentes de control sensibles de las altas corrientes y ruidos generados por el motor.

---

El **Puente H** es fundamental para nuestro robot porque permite el **control total del motor**: puede cambiar el sentido de giro (adelante/atrás) y, con PWM, controlar la velocidad con precisión. Además, actúa como un **escudo protector para el motor**, aislando los componentes sensibles y garantizando la fiabilidad y seguridad del sistema.

![Puente H](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/Purnte%20H.jpg)

#### 📸 Raspberry Pi AI Camera

La **Raspberry Pi AI Camera** está específicamente diseñada para aprovechar el **procesamiento avanzado de inteligencia artificial (IA)** en dispositivos Raspberry Pi, especialmente cuando se combina con hardware de aceleración como el Hailo AI Module.

---
**_Características Sobresalientes:_**

* **Procesamiento de IA en el chip (Edge AI):** Realiza la inferencia de redes neuronales directamente en el sensor Sony IMX500, liberando la Raspberry Pi principal de esta carga computacional. Esto permite IA en tiempo real con baja latencia.
* **Sensor de alta resolución:** Cuenta con un sensor de 12.3 megapíxeles (4056 x 3040 píxeles), capturando imágenes detalladas.
* **Salida de metadatos de tensor:** Además de la imagen, la cámara puede enviar directamente los resultados del procesamiento de IA, simplificando la integración con otras aplicaciones.
* **Compatibilidad y enfoque manual:** Se conecta vía CSI estándar con todas las Raspberry Pi compatibles y permite ajustar manualmente el enfoque para diversas aplicaciones.
* **Reducción de latencia y ancho de banda:** Los datos procesados de IA (como la detección de objetos) se generan directamente en la cámara, minimizando la latencia y reduciendo significativamente el ancho de banda necesario en el bus de datos CSI.

---

La **Raspberry Pi AI Camera** es fundamental para nuestro robot porque permite la **IA en el borde**, procesando visión directamente en el chip. Esto libera recursos de la Pi 5, reduce la latencia y la necesidad de ancho de banda. Su **alta resolución** y la capacidad de enviar **metadatos de IA pre-procesados** simplifican el desarrollo. Además, es **energéticamente eficiente**, clave para la autonomía del robot. En definitiva, convierte a nuestro robot en un agente **inteligente y reactivo** capaz de percibir e interpretar su entorno de forma autónoma.

![La Raspberry Pi AI Camera](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/Camara%20Rasberry%20PI%205.jpg)

(AC) convencionales por su capacidad de **controlar con precisión su posición angular, velocidad y, en algunos casos, su aceleración**. Piensa en él como un motor que no solo gira, sino que sabe exactamente dónde está y puede ir a una posición específica y mantenerla, incluso si hay una fuerza externa que intenta moverlo.

---

## ⚙️ Análisis Técnico de Actuadores: Servomotores LEGO EV3

A diferencia de los motores de corriente continua (DC) convencionales que giran libremente al recibir voltaje, los motores del kit LEGO EV3 funcionan bajo el principio de **servomotores de alta precisión**. Tienen la capacidad de controlar con exactitud su posición angular, velocidad y aceleración, sabiendo exactamente en qué posición están y manteniendo ese ángulo interactuando de forma reactiva ante fuerzas externas.

### 🔄 Arquitectura Interna Común (Sistema de Lazo Cerrado)

Ambos motores (Grande y Mediano) operan como un sistema de **lazo cerrado** gracias a sus componentes internos:
1. **Motor DC Interno:** El actuador electromecánico central que genera el movimiento.
2. **Tren de Engranajes Reductores:** Un sistema de piñones que reduce las RPM nativas del motor pero multiplica drásticamente su torque (fuerza de giro), permitiendo movimientos controlados y minimizando el juego mecánico (*backlash*).
3. **Encoder Óptico Integrado (Sensor de Posición):** Es el tacómetro digital interno que mide constantemente los grados exactos de rotación del eje. Envía esta retroalimentación (*feedback*) en tiempo real a la Raspberry Pi 5, la cual compara la posición actual con la deseada y ajusta la energía para corregir cualquier desviación al instante.

---

### Motor Grande LEGO EV3 (Servomotor de Propulsión)

* **Rol en el Robot:** Tracción y velocidad lineal (Eje Trasero).
* **Control de Posición y Velocidad:** Aunque se utiliza principalmente para el desplazamiento continuo del vehículo, el encoder interno nos permite implementar un **control PID de velocidad**. Esto asegura que el motor mantenga las RPM exactas calculadas por el algoritmo de *Time Attack*, sin importar si el robot está subiendo la rampa o tomando una curva cerrada.
* **Importancia de la Retroalimentación:** Los datos del encoder se procesan en Python para realizar **odometría**. Al saber los grados exactos que ha girado el motor grande, el software calcula la distancia en milímetros que el robot ha recorrido en la pista, vital para planificar el momento justo de frenado o el inicio de la maniobra de estacionamiento.

###   Motor Mediano LEGO EV3 (Servomotor de Dirección)

* **Rol en el Robot:** Control Angular del Mecanismo Ackermann (Eje Delantero).
* **Control de Posición Preciso:** Este motor sustituye al servomotor comercial clásico. Aprovechamos su alta resolución para mover las ruedas delanteras a ángulos específicos (ej. $-15^\circ$ para esquivar un pilar izquierdo, $+22^\circ$ para una curva cerrada a la derecha). Una vez alcanzado el ángulo, el lazo cerrado bloquea el motor en esa posición, resistiendo las fuerzas de fricción de las ruedas contra el suelo.
* **Ventaja Dinámica:** Al ser más ligero y compacto que el motor grande, reduce la inercia en el tren delantero, permitiendo correcciones de trayectoria sumamente rápidas generadas por los frames de la Raspberry Pi AI Camera a alta frecuencia ($60\text{ Hz}$).

---

### 📊 Tabla Comparativa de Aplicación en Competencia

| Característica | Motor Grande EV3 (Tracción) | Motor Mediano EV3 (Dirección) |
| :--- | :--- | :--- |
| **Prioridad de Control** | Velocidad constante y Torque elevado. | Posición angular milimétrica y Rapidez. |
| **Uso del Encoder** | Odometría, cálculo de distancia y frenado dinámico. | Alineación precisa de manguetas y control PID de centrado. |
| **Comportamiento Cinemático** | Modulación de potencia en rectas y curvas. | Retención rígida del ángulo de giro seleccionado. |

### 🎯 Conclusión para el Proyecto
La integración de estos dos servomotores EV3 simplifica drásticamente el desarrollo del software de control en la Raspberry Pi 5. En lugar de estimar a ciegas cuánto se mueve el robot, la lectura matemática de sus encoders integrados nos permite programar trayectorias curvas perfectas, asegurando que el vehículo interactúe con el circuito de la WRO de forma controlada, repetible y efectiva.

![Motores EV3](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/Motores%20EV3.jpg)

---

###  Sensor Láser Multizona STMicroelectronics VL53L5CX (Sensor de Distancia Activo)

A diferencia de los sensores ultrasónicos convencionales o los telémetros láser simples que solo miden un punto central, el **VL53L5CX** funciona como un LiDAR de estado sólido en miniatura. Este componente es fundamental para dotar al robot de una percepción espacial tridimensional y reactiva en tiempo real.

#### Características Principales y Funcionamiento:
* **Matriz de Profundidad Bidimensional:** El sensor cuenta con una óptica avanzada que divide su campo de visión (FoV) en una grilla de zonas independientes. Puede configurarse en una matriz de **4x4 zonas (a 60 Hz)** para máxima velocidad de respuesta, o de **8x8 zonas (a 15 Hz)** para máxima resolución espacial (64 puntos de lectura simultáneos).
* **Principio de Tiempo de Vuelo (Time-of-Flight - ToF):** Cada zona dispara ráfagas de fotones infrarrojos invisibles a través de un emisor VCSEL y mide el tiempo exacto que tardan en rebotar y regresar al receptor. Como la velocidad de la luz es constante, el sensor calcula la distancia matemática exacta de cada píxel de forma independiente.
* **Inmunidad al Entorno:** Al ser un sensor de luz activa (emite su propio mapa de luz), su precisión no depende del color de los obstáculos ni de los reflejos del suelo, lo que lo hace inmune a los cambios de iluminación ambiental de la pista de la WRO.

#### Componentes Internos:
1. **Emisor Láser VCSEL:** Diodo láser de emisión superficial con cavidad vertical que emite luz infrarroja segura para la vista ($940\text{ nm}$).
2. **Matriz de Receptores SPAD:** Diodos de avalancha de fotón único capaces de capturar el regreso de los fotones a nivel de picosegundos.
3. **Microcontrolador Integrado (Firmware de Bajo Nivel):** Un chip interno que procesa los tiempos de vuelo, aplica algoritmos de calibración y devuelve las distancias limpias en milímetros a través del bus I2C.

---

### 📌 Rol del Sensor Láser en la Estrategia del Vehículo

El uso de este sensor cambia por completo el juego para nuestro robot, resolviendo problemas de navegación complejos mediante software en Python:

* **Control en Lazo Cerrado de Distancia Lateral:** Al ubicar sensores en los flancos (Izquierdo y Derecho) configurados a **60 Hz**, creamos un lazo cerrado de centrado. El software en la Raspberry Pi 5 mide constantemente la distancia a los muros laterales, calcula el error de desvío y ajusta el motor mediano de dirección inmediatamente para mantener el robot perfectamente alineado en el carril.
* **Análisis Topológico y Predicción de Evasión:** El sensor frontal (configurado a 8x8 zonas) realiza un escaneo volumétrico. No solo detecta que hay un obstáculo enfrente, sino que identifica su ancho exacto y calcula el **Tiempo para la Colisión (TTC)**. Esto permite trazar una curva de evasión matemática suave, calculando el radio Ackermann exacto para que el tren trasero (motor grande EV3) esquive el pilar sin derrapar ni perder inercia.
* **Filtro de Ruido Óptico por Software:** Dado que el sensor entrega una matriz de datos, implementamos filtros de mediana espacial en Python. Si un solo píxel registra un obstáculo a $5\text{ cm}$ debido al polvo en la pista, pero los 63 píxeles circundantes marcan $150\text{ cm}$, el software ignora esa lectura espuria, evitando maniobras evasivas falsas que arruinarían el tiempo de la vuelta.

  ![Servomotor](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/descarga.jpg)


---

#### ⚡ Regulador de Voltaje

Un **regulador de voltaje electrónico** en robótica es un componente crucial diseñado para **mantener una tensión eléctrica de salida constante y estable** para los distintos sistemas del robot, sin importar las variaciones en la fuente de alimentación (como una batería que se descarga) o los cambios en la demanda de energía de los componentes del robot.

---
**_Características Esenciales:_**

* **Estabilización de la Tensión de Suministro:** Su función principal es vital para un robot. Asegura que la Raspberry Pi, los servomotores y los sensores reciban el voltaje exacto que necesitan (por ejemplo, 5V para la Pi), incluso si la batería del robot comienza a descargarse y su voltaje total disminuye. Esto es crucial para la estabilidad y fiabilidad del sistema.
* **Manejo de Diferentes Niveles de Voltaje:** Un robot suele tener varios componentes que operan a diferentes voltajes (ej. 5V para la lógica, 12V para los motores). Los reguladores permiten crear "rieles" de voltaje específicos a partir de una única fuente de alimentación, simplificando el diseño del sistema de energía.
* **Eficiencia Energética (para Robots Autónomos):** En robótica, la eficiencia es fundamental para la autonomía. Los reguladores conmutados (switching) son preferidos en robots. Son mucho más eficientes que los lineales, ya que minimizan la energía que se pierde como calor. Esto significa que la batería del robot durará más tiempo, aumentando su autonomía operativa.
* **Versatilidad:** Pueden ser reductores (buck) para bajar el voltaje de la batería (ej. de 12V a 5V para la Pi) o incluso elevadores (boost) si un componente necesita un voltaje mayor que el de la batería.

---

El **Regulador de Voltaje Electrónico** es indispensable para el robot porque asegura una **alimentación eléctrica constante y estable** específicamente para el/los servomotor(es). Es vital para:

* **Proteger los servomotores:** Garantiza que reciban siempre el voltaje óptimo, previniendo daños por fluctuaciones de la batería o picos de carga.
* **Asegurar su rendimiento preciso:** Un voltaje estable es clave para el funcionamiento fiable y la precisión de movimiento del/de los servomotor(es).
* **Maximizar la autonomía:** Al usar reguladores conmutados eficientes, minimiza la pérdida de energía en la alimentación del/de los servomotor(es), prolongando la duración de la batería del robot.

En esencia, el regulador es fundamental para la **fiabilidad y la prolongación de la vida útil** de los componentes eléctricos del robot.


![Regulador de Voltaje](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/Regulador%20de%20voltaje%201.jpg)


---

### 💡 Componentes Clave del Vehículo

Hemos seleccionado cuidadosamente cada componente para asegurar el máximo rendimiento y fiabilidad de nuestro robot. A continuación, detallamos los elementos esenciales que dan vida a nuestro proyecto.

#### 🧠 Raspberry Pi 5

La **Raspberry Pi 5** es el cerebro de nuestro sistema, definida por la misma Raspberry Pi Foundation como una **PC de bajo coste del tamaño de una tarjeta de crédito**. Permite explorar el mundo de la informática y aprender lenguajes de programación como Scratch y Python, siendo una herramienta increíblemente versátil.

La **Raspberry Pi 5** es ideal para nuestro robot por su **gran potencia de procesamiento para IA y visión**, lo que nos permite implementar algoritmos complejos. Su **amplia RAM** asegura una multitarea eficiente y su **conectividad avanzada** facilita la comunicación. Además, el **almacenamiento SSD ultrarrápido** y los **conectores MIPI duales para cámaras** son fundamentales para la percepción y toma de decisiones en tiempo real, garantizando un robot de **alto rendimiento y gran fiabilidad**.


#### 📸 Raspberry Pi AI Camera

La **Raspberry Pi AI Camera** está específicamente diseñada para aprovechar el **procesamiento avanzado de inteligencia artificial (IA)** en dispositivos Raspberry Pi, especialmente cuando se combina con hardware de aceleración como el Hailo AI Module.

La **Raspberry Pi AI Camera** es fundamental para nuestro robot porque permite la **IA en el borde**, procesando visión directamente en el chip. Esto libera recursos de la Pi 5, reduce la latencia y la necesidad de ancho de banda. Su **alta resolución** y la capacidad de enviar **metadatos de IA pre-procesados** simplifican el desarrollo. Además, es **energéticamente eficiente**, clave para la autonomía del robot. En definitiva, convierte a nuestro robot en un agente **inteligente y reactivo** capaz de percibir e interpretar su entorno de forma autónoma.


---

## ⚡ Gestión de la Potencia y los Sensores

# Gestión de Potencia y Control de Sentido del Vehiculo

---

Este documento detalla la estrategia de gestión de potencia y el sistema de control de sentido implementados en nuestro robot, utilizando una Raspberry Pi 5 y la Raspberry Pi AI Camera.

---

## Gestión de Energía y Sensores

# 🔋 Gestión de Energía y Distribución Eléctrica

Esta sección aborda cómo el vehículo gestiona su potencia y recursos eléctricos para alimentar tanto los sistemas de procesamiento de alta densidad como los actuadores mecánicos, garantizando la máxima eficiencia y estabilidad en pruebas de *Time Attack*.

---

## 1. Arquitectura de Fuente de Energía Unificada

Para optimizar el peso total del chasis y maximizar la aceleración, hemos unificado el sistema eléctrico utilizando **exclusivamente un paquete de baterías de Litio (Li-ion / LiPo)** de alta descarga. Toda la potencia del robot se centraliza en esta fuente, distribuyéndose en dos lazos de corriente independientes mediante hardware:

### Componentes de la Red de Potencia

* **Paquete de Baterías de Litio Principal:** Suministra energía directa de alta corriente. Al alimentar tanto la lógica como los motores desde una sola fuente, reducimos drásticamente la masa del vehículo, lo que mejora la relación peso-potencia crítica para la WRO 2026.
* **Regulador de Voltaje de Alta Eficiencia (Buck Converter / UBEC):** Dado que las baterías de litio entregan un voltaje nominal variable y superior a los $5\text{V}$, este componente DC-DC es indispensable. Actúa como un escudo electrónico reduciendo y estabilizando el voltaje a exactamente **5V con un mínimo de 5A**, alimentando de forma limpia y continua a la **Raspberry Pi 5** y a la **Raspberry Pi AI Camera**. Esto protege la electrónica sensible contra sobretensiones y fluctuaciones térmicas.
* **Módulo de Aislamiento y Puente H (Etapa de Potencia):** Conectado directamente a la línea de voltaje nativo de la batería de litio para suministrar la fuerza requerida por el **motor grande** (propulsión) y el **motor mediano** (dirección) de LEGO EV3. Las señales lógicas PWM enviadas desde los GPIO de la Raspberry Pi 5 controlan este módulo, manteniendo un aislamiento eléctrico relativo.
* **Switch Principal de Seguridad:** Un interruptor físico de alta corriente colocado en serie con el borne positivo de la batería. Permite el corte inmediato o el encendido seguro de todo el vehículo, controlando el flujo general de energía tanto para la etapa de potencia como para la de control.

---

## ⚡ Mitigación de Caídas de Tensión (*Brownouts*)

El mayor desafío técnico de utilizar una sola fuente de energía para motores y computación es el riesgo de que la Raspberry Pi 5 se reinicie debido a la demanda masiva de corriente cuando el motor grande de LEGO EV3 arranca o frena bruscamente. Para solucionar esto sin añadir un Power Bank, implementamos la siguiente estrategia de hardware:

1. **Filtrado por Condensadores (Capacitores de Desacoplo):** Añadimos condensadores electrolíticos en paralelo a la entrada del regulador de voltaje. Estos actúan como reservas de energía instantánea, absorbiendo las caídas de tensión milimétricas provocadas por los motores.
2. **Líneas Separadas desde el Nodo Central:** El cableado de potencia se estructuró en una topología de estrella. Los motores y el regulador Buck nacen del mismo conector de la batería pero corren por cables independientes, evitando que el ruido eléctrico de alta frecuencia de las escobillas de los motores interfiera con el bus I2C de los sensores láser o la estabilidad de la CPU.
   
## 2. Sensores
## 📡 Subsistema de Percepción y Captura de Datos

El vehículo integra una red de sensores ópticos y de telemetría mecánica que recopilan información del entorno en tiempo real. Esta configuración permite fusionar datos visuales, geométricos y de rotación para tomar decisiones de navegación con máxima precisión.

### 1. Raspberry Pi AI Camera (Percepción Semántica)

Es el sensor visual principal del robot. A diferencia de las cámaras estándar, cuenta con un acelerador de redes neuronales integrado que procesa el video en tiempo real directamente en el hardware periférico, reduciendo la carga de la CPU de la Raspberry Pi 5.
* **Misión Crítica:** Analiza el entorno mediante visión computacional, segmentando los carriles y aislando los espacios de color en formato HSV para identificar y clasificar las señales de tráfico (pilares verdes y rojos). Además, asiste en la detección de zonas clave como el recuadro de estacionamiento en paralelo.

### 2. Arreglo de Sensores Láser ToF VL53L5CX (Percepción Métrica)

Este sistema actúa como un LiDAR de estado sólido multizona de alto rendimiento que complementa la visión de la cámara.
* **Misión Crítica:** Proporciona un mapa de profundidad bidimensional mediante una matriz de hasta $8 \times 8$ zonas independientes. Su función es medir con exactitud matemática la distancia milimétrica hacia los muros laterales y frontales. Al emitir su propia luz infrarroja, permite que el robot mantenga un control PID de centrado perfecto e inmune a los cambios de luz ambiental del recinto de competencia.

### 3. Encoders Ópticos Internos (Motores LEGO EV3)

Hemos eliminado los sensores rotacionales externos acoplados a motores DC convencionales. En su lugar, aprovechamos los **tacómetros digitales (encoders) integrados** tanto en el motor grande (propulsión) como en el motor mediano (dirección) del kit LEGO EV3.
* **Misión Crítica en Motor Grande (Tracción):** Mide los grados de rotación exactos de las ruedas traseras. El software en Python procesa estos datos para ejecutar algoritmos de **odometría de lazo cerrado**, calculando la distancia recorrida en la pista para planificar con exactitud la frenada, el conteo de vueltas de respaldo y la secuencia de reversa para el estacionamiento en paralelo.
* **Misión Crítica en Motor Mediano (Dirección):** Proporciona retroalimentación instantánea sobre la posición angular real de las manguetas delanteras. Esto permite saber con precisión milimétrica el ángulo de giro del sistema Ackermann en cada frame, corrigiendo cualquier desviación provocada por la fricción del suelo.

  ## 3. Consumo de Energía
## 3. Estimación del Consumo Energético Unificado

Dado que el vehículo ha migrado a un sistema de alimentación único basado exclusivamente en baterías de Litio, todo el consumo se consolida en una sola línea de potencia. El consumo estimado bajo condiciones de máxima exigencia en pista (*Time Attack*) es el siguiente:

* **Raspberry Pi 5 + Raspberry Pi AI Camera:** $\sim 2.7\text{ A @ 5V}$ (Aproximadamente $13.5\text{ W}$ en picos de inferencia de IA y procesamiento matemático continuo).
* **Motor Grande LEGO EV3 (Tracción Trasera):** $\sim 0.12\text{ A}$ (en vacío) hasta $\sim 2.0\text{ A}$ (corriente de arranque/bloqueo en aceleración máxima) @ $7.4\text{V} - 9.0\text{V}$.
* **Motor Mediano LEGO EV3 (Dirección Delantera):** $\sim 0.08\text{ A}$ (en vacío) hasta $\sim 1.2\text{ A}$ (picos de corrección rápida a 60 Hz) @ $7.4\text{V} - 9.0\text{V}$.
* **Arreglo de 3 Sensores Láser ToF VL53L5CX:** $\sim 120\text{ mA @ 5V}$ (en total, alimentados a través del bus regulado).

> 📊 **Cálculo de Autonomía:** El consumo promedio estimado del sistema en carrera oscila entre los $18\text{ W}$ y $25\text{ W}$. Para cumplir holgadamente con las sesiones de prueba y las mangas oficiales de la WRO 2026, el paquete de baterías de litio seleccionado entrega una capacidad mínima de **$22\text{ Wh}$**, garantizando un funcionamiento estable y sin caídas de tensión por más de 45 minutos continuos.

---

## 4. Justificación Técnica de Selección de Componentes

La selección del hardware obedece a criterios estrictos de precisión cinemática, robustez mecánica y velocidad de procesamiento, eliminando módulos genéricos por soluciones de grado de ingeniería:

* **Motores LEGO EV3 (Grande y Mediano):** Se seleccionaron por encima de los motores DC y servomotores convencionales debido a sus **encoders ópticos internos de alta resolución**. El motor grande nos permite sustituir sensores ópticos externos, calculando la odometría de forma matemática para el control de vueltas y el estacionamiento en reversa. El motor mediano elimina las holguras mecánicas típicas de los servos comerciales pequeños, asegurando que las manguetas del sistema Ackermann mantengan el ángulo exacto exigido por el bucle PID.
* **Arreglo Láser ToF VL53L5CX:** Reemplaza a los sensores ultrasónicos tradicionales (los cuales sufren de eco y rebotes falsos en las esquinas de la pista). Al medir por Tiempo de Vuelo de fotones infrarrojos en matrices de hasta $8\times8$, este componente proporciona una telemetría milimétrica del ancho y distancia de los muros, siendo completamente inmune a las variaciones de luz del recinto de competencia.
* **Raspberry Pi AI Camera:** Su inclusión es el pilar del software de navegación. Al procesar redes neuronales directamente en su hardware dedicado (Edge AI), es capaz de clasificar y diferenciar instantáneamente las señales de tráfico rojas y verdes sin consumir ciclos de reloj de la CPU principal de la Raspberry Pi 5. Esto permite balancear la carga de trabajo y ejecutar el control cinemático en tiempo real sin retrasos (*lag*).
El código de control implementado en Python gestiona la interpretación de los datos de los sensores y actúa en consecuencia, ajustando la dirección, velocidad y decisiones del robot según las condiciones del entorno.


---

## 🚗 Gestión de Movilidad

Este robot, dise, se mueve como un coche: sus ruedas traseras lo impulsan y las ruedas delanteras directrices lo guían. Su diseño mecánico, detallado en el modelo 3D, busca ser robusto y ligero, con espacio para todos los componentes.

La dirección es clave: un servomotor mueve las ruedas delanteras, controlando los giros mediante un mecanismo de dirección (tipo Ackerman). Un controlador coordina estos movimientos para lograr una maniobrabilidad precisa. En resumen, es un vehículo ágil, diseñado para el control exacto de su trayectoria..

---
# *Lenguaje de Programación*

---

# Detección de Objetos y Límites de Pista 🤖
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/SRC/Python.png)

Para capacitar a nuestro robot con la habilidad de "ver" su entorno, integramos un conjunto de sensores clave. Si bien los sensores de proximidad (como los ultrasónicos o infrarrojos) son cruciales para detectar obstáculos cercanos y medir distancias, el componente central de nuestra visión es la Cámara Raspberry Pi AI.

La Cámara Raspberry Pi AI, en combinación con algoritmos de visión por computadora desarrollados en Python, aprovecha librerías potentes como OpenCV para el procesamiento avanzado de imágenes. Esta sinergia nos permite no solo identificar la presencia de obstáculos, sino también clasificarlos eficazmente, ya sean conos u otros elementos estáticos presentes en el entorno de la pista. La información obtenida de esta detección es indispensable para que el robot tome decisiones de navegación precisas, como la desaceleración o la evasión.

Paralelamente, para asegurar que el robot se mantenga dentro de su trayectoria, utilizamos la Cámara Raspberry Pi AI para el reconocimiento de los bordes de la pista. A través del procesamiento de imágenes en Python, el sistema analiza las características visuales de la pista, incluyendo líneas y paredes, permitiendo al robot ajustar su dirección de forma continua para permanecer dentro de los límites predefinidos.

# DIAGRAMAS DE LOS CODIGOS 


----

Este documento presenta los diagramas de código de nuestro prototipo de robot, donde este esquivara las paredes tanto internas como externas de la pista. El objetivo es ofrecer una comprensión clara y estructurada de la arquitectura de software y la lógica de control que permiten al robot navegar de forma autónoma en entornos con obstáculos.

Los diagramas visualizan el flujo de procesamiento de información, desde la percepción del entorno mediante los sensores hasta la toma de decisiones para evitar colisiones y la ejecución de movimientos por parte de los actuadores. Se detallará la interacción entre los módulos de detección de obstáculos, los algoritmos de navegación y la manipulación de los sistemas de propulsión y dirección.

Esta representación gráfica facilitará el entendimiento de la secuencia lógica y las interdependencias entre los componentes de software, proporcionando una visión integral del funcionamiento autónomo del robot.


![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Other/Diagrama%20de%20Flujo%20del%20Codigo%201%20Desafio%20Abierto%20.png)


---
# IMAGENES DEL VEHICULO/ROBOT

A continuación, se presentan las figuras que ilustran el prototipo de nuestro robot en su estado actual de desarrollo. Estas imágenes han sido seleccionadas para ofrecer una perspectiva clara de la implementación del diseño mecánico y la integración de los componentes clave. Se podra apreciar en como se jerarquizony se organizaron los componenetes en el chasis del robot.

---

# *Parte de Arriba* 

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Arriba.jpeg)

---

# *Parte de abajo*

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/ABAJO.jpeg)

---


# *Parte de Adelante* 
![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Adelante.jpeg)

---

# *Parte de Atras*

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Atras.jpg.jpeg)

---

# *Parte Dreceha*
![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Derecha.jpeg)


---

# *Parte Izquierda*
![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Vehiculo-Fotos/Izquierda.jpeg)

---

## 🧠 Estrategias Planteadas para Resolver los Retos

En esta sección, compartimos las metodologías y enfoques innovadores que hemos diseñado para superar los desafíos propuestos en la competencia WRO 2025.

## 🧠 Documentación de Pruebas: Pipeline de Visión Artificial e Inferencia de IA

Para superar con éxito el reto de obstáculos aleatorios (pilares verdes y rojos), hemos desarrollado un sistema de procesamiento visual en dos capas síncronas utilizando la **Raspberry Pi AI Camera**. 

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Prueba%201.jpeg)

### ⚙️ Explicación de la Lógica del Algoritmo

Nuestra arquitectura de software separa la tarea de "saber DÓNDE hay un obstáculo" de la tarea de "saber QUÉ SIGNIFICA ese obstáculo". Esto optimiza los recursos de la Raspberry Pi 5 y evita falsos positivos por cambios de luz:

#### 1. Capa Izquierda (IA: Blanco y Negro) - Detección de Bounding Boxes
* **Procesamiento:** La imagen raw de la cámara se convierte a escala de grises (o luminancia pura) y es procesada por una red neuronal optimizada (ej. MobileNet-SSD / YOLO-Nano) que corre directamente en el chip acelerador de la cámara.
* **Resultado:** El modelo de IA detecta la geometría del pilar y dibuja un cuadro delimitador (*Bounding Box*) azul. En este frame de prueba, la IA tiene una confianza del **$55\%$** confirmando que la estructura física existe.
* **Justificación de Ingeniería:** Al procesar la detección física en blanco y negro, la IA es inmune a si el pilar es rojo, verde o si hay sombras pesadas en la pista. Solo busca la forma geométrica tridimensional del obstáculo.

#### 2. Capa Derecha (Humano: Color) - Clasificación Cromática (Segmentación HSV)
* **Procesamiento:** Una vez que la IA le dice al código las coordenadas $(X, Y)$ exactas donde se encuentra el pilar, el software recorta esa región de interés (ROI) y analiza su espectro de color utilizando el espacio de color **HSV (Hue, Saturation, Value)**.
* **Resultado:** * Si el rango HSV detecta una saturación dominante en el espectro del **Verde**, el cuadro se torna **Rojo/Verde** en el código y se clasifica como: *Girar a la Izquierda*.
  * Si el rango HSV detecta una saturación dominante en el espectro del **Rojo**, se clasifica como: *Girar a la Derecha*.

---

### 🏎️ Integración en la Toma de Decisiones del Reto de Obstáculos

Este entrenamiento y pipeline de visión se traduce directamente en las acciones físicas de nuestros servomotores LEGO EV3:

1. **Fusión con los Sensores Láser (VL53L5CX):** La IA detecta el pilar a la distancia $\to$ los sensores ToF miden su distancia exacta en milímetros $\to$ el software calcula el *Tiempo para la Colisión* (TTC).
2. **Evasión Dinámica Ackermann:** * Si la capa cromática confirma **Pilar Verde**, la Raspberry Pi 5 calcula un radio de giro hacia la izquierda enviando los grados exactos al **motor mediano EV3**.
   * Si confirma **Pilar Rojo**, el giro se ejecuta hacia la derecha.
3. **Control de Velocidad:** El **motor grande EV3 (tracción)** modula su potencia reduciendo ligeramente la velocidad lineal durante la evasión para garantizar que el tren trasero no desplace el pilar, manteniendo el control de lazo cerrado mediante odometría.

   ---

   ## 📊 Telemetría en Tiempo Real: VL53L5CX Depth Visualizer

Para validar el comportamiento del bus I2C y calibrar los algoritmos de navegación reactiva, desarrollamos una herramienta de software personalizada: el **VL53L5CX Depth Visualizer**. Esta interfaz procesa y mapea en paralelo las tres matrices síncronas de $8 \times 8$ zonas (64 píxeles de profundidad por sensor) en la Raspberry Pi 5.

La captura de pantalla adjunta (`Diagrama 1.jpeg`) muestra el estado del entorno capturado por el bloque tridimensional de telemetría del robot:

### ⚙️ Desglose Técnico de la Telemetría por Sensor

El software asigna un código cromático dinámico a los valores numéricos (distancias en milímetros) recibidos por cada una de las zonas SPAD de los sensores:
* **Verde (Zonas Libres):** Distancias seguras y despejadas (típicamente $> 500\text{ mm}$ e inferiores a los límites físicos del carril).
* **Naranja/Marrón (Zonas de Transición / Aproximación):** Distancias intermedias que alertan de la proximidad de muros o el inicio de una curva.
* **Rojo (Zonas de Peligro / Obstáculo Inminente):** Distancias críticas (por debajo de $150\text{ mm} - 100\text{ mm}$) que indican una colisión inminente o la presencia directa de la base de un obstáculo.

---

### 🔍 Análisis de Escenario de Conducción en el Gráfico

Al evaluar las lecturas síncronas de los tres sensores, el software interpreta la física del entorno para guiar los actuadores LEGO EV3:

![Logo del Equipo Triple Threat](![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Diagrama%201.jpeg)
)
)

#### 1. Flanco Izquierdo (`IZQUIERDO - 0x30`)
* **Análisis de Datos:** La mitad inferior y el lateral derecho de la matriz están completamente saturados en rojo y naranja (valores entre $55\text{ mm}$ y $355\text{ mm}$). El cuadrante superior izquierdo se mantiene en verde ($570\text{ mm} - 720\text{ mm}$).
* **Interpretación Cinemática:** El vehículo se encuentra extremadamente cerca del muro izquierdo o está enfrentando un obstáculo en ese flanco. El algoritmo PID detecta un error de centrado negativo masivo, obligando al **motor mediano EV3** a corregir el ángulo de dirección hacia la derecha.

#### 2. Vector Frontal (`CENTRAL - 0x31`)
* **Análisis de Datos:** El visualizador muestra una clara división vertical. El pasillo izquierdo permanece en verde libre (valores estables de $\sim 1000\text{ mm} - 1055\text{ mm}$), mientras que la mitad derecha cae a zona naranja ($340\text{ mm} - 495\text{ mm}$).
* **Interpretación Cinemática:** El predictor de evasión detecta que el camino directo se está bloqueando por la derecha. Al combinar esto con los datos cromáticos de la cámara de IA, el software calcula el **Tiempo para la Colisión (TTC)** y planifica un arco Ackermann hacia la izquierda, aprovechando el espacio libre de un metro detectado por los píxeles verdes.

#### 3. Flanco Derecho (`DERECHO - 0x29`)
* **Análisis de Datos:** Predominancia casi absoluta de zonas verdes de alta distancia ($1200\text{ mm} - 1460\text{ mm}$), con pequeñas caídas aisladas en rojo en la periferia profunda.
* **Interpretación Cinemática:** El flanco derecho cuenta con un amplio margen de escape libre. Esto confirma la viabilidad de la trayectoria de evasión calculada por el sensor central; el robot tiene vía libre para abrirse hacia la derecha después de limpiar el obstáculo actual.

---

### 🛡️ Aplicación de Filtros Matemáticos Visibles en la Grilla

La interfaz gráfica nos permitió comprobar empíricamente la necesidad del **Pipeline de Filtrado en Python**:
* **Aislamiento de Ruido (Píxeles Espurios):** En el sensor Derecho (`0x29`), se observa un píxel aislado en rojo con valor $100$ rodeado por un entorno completamente verde de $\sim 600\text{ mm}$. Esto demuestra gráficamente el éxito de nuestro **Filtro de Mediana Espacial $3 \times 3$**: el software detecta matemáticamente que ese valor de $100$ es un fotón rebotado por polvo o reflejo, y lo ignora por completo antes de enviar comandos al actuador de dirección, evitando que el robot pegue un volantazo destructivo.
* **Estabilización del Horizonte:** La línea horizontal turquesa (`HORIZONTE 0°`) delimita el plano de cabeceo del robot. Permite al software ignorar las lecturas de los píxeles inferiores que apuntan directamente hacia el suelo cuando el chasis experimenta transferencias de peso o vibraciones al acelerar a fondo con el **motor grande EV3**.

---
# Codigo del Robot/Solución de problemas


```python
