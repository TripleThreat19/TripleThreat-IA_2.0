# TripleThreat-IA_2.0  Proyecto Orlando 🤖
---

## 🚀 Categoría: Futuros Ingenieros WRO 2026

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/logo%20del%20equipo/Logo%20del%20Equipo.jpg)


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
## ⚙️ Diseño Mecánico, Tracción y Dinámica Vehicular

### Configuración Geométrica y Chasis
El vehículo fue construido utilizando una estructura híbrida modular basada en vigas estructurales tipo LEGO Technic combinadas con placas de soporte impresas/cortadas a medida y fijaciones de alta rigidez para evitar torsiones mecánicas.

* **Geometría del Vehículo:**
  * **Distancia entre ejes (*Wheelbase*):** $\sim 170\text{ mm}$.
  * **Ancho de vía (*Track width*):** $\sim 145\text{ mm}$.
  * **Diámetro de neumático:** $\sim 56\text{ mm}$ (goma de alto agarre con banda de rodadura estriada).
  * **Sistema de Dirección:** Eje delantero pivotante accionado por un servomotor montado en posición vertical superior, conectado mediante bieletas rígidas de dirección.

### Distribución de Masas y Dinámica Vehicular
La disposición de componentes en varios niveles verticales optimiza el espacio pero requiere un control preciso de la transferencia de pesos:

* **Reparto de Pesos:** Estimado en **60% eje posterior / 40% eje anterior**. El posicionamiento del paquete de celdas Li-Ion 18650 y el driver L298N sobre el eje trasero incrementa la carga normal ($N$) sobre las ruedas motrices, maximizando el agarre mecánico y reduciendo el deslizamiento en aceleración.
* **Centro de Masa:** La Raspberry Pi 5 y la NPU Hailo-8L se sitúan en la plataforma superior. Para compensar este centro de gravedad elevado, se mantuvo un ancho de vía amplio ($145\text{ mm}$), otorgando estabilidad lateral en maniobras evasivas rápidas.

### Análisis del Sistema de Transmisión

| Parámetro Mecánico | Especificación / Configuración | Justificación Técnico-Práctica |
| :--- | :--- | :--- |
| **Configuración** | Tracción Trasera (RWD) con bloque cerrado | Garantiza transferencia directa de potencia sin pérdida de alineación. |
| **Relación de Transmisión** | Reducción interna diferencial ($\sim 1:30$) | Proporciona el torque adecuado para vencer la inercia del chasis cargado manteniendo velocidad constante. |
| **Puntos de Giro** | Vínculos rígidos en dirección delantera | Elimina el juego mecánico (*backlash*) para mantener la precisión en el ángulo de viraje. |
| **Rigidez Estructural** | Vigas perforadas reforzadas con abrazaderas | Soporta las vibraciones continuas de la pista sin desalinear los sensores ToF ni la cámara. |


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

### 📐 Colocación Estratégica de Componentes Clave

* **Motor Grande LEGO EV3 (Propulsión Trasera):** Se ubica y fija firmemente en la sección posterior del esqueleto de LEGO. Esta posición concentra la masa sobre el eje motriz, optimizando la tracción de las ruedas traseras y maximizando el agarre durante la aceleración en rectas para evitar derrapes.
* **Servomotor Digital de Dirección (MG995 / MG90S):** Se sitúa en la zona frontal sustituyendo al antiguo motor EV3. Se acopla directamente al mecanismo de barra de dirección tipo Ackermann mediante adaptadores dedicados. Su formato compacto reduce el peso en el morro y permite correcciones de ángulo inmediatas enviadas por hardware PWM desde la computadora central.
* **Banco de Baterías Li-ion 18650 (Alimentación Unificada):** Las celdas se posicionan de manera simétrica en la zona central-inferior sobre las bases 3D reutilizadas de nuestro proyecto anterior. Esta ubicación fija el centro de gravedad en la parte más baja del vehículo, garantizando una distribución de masa equilibrada para la estabilidad en curvas a alta velocidad.
* **Módulo Relé Electrónico con Display Digital:** Montado en el nivel superior de fácil acceso visual. Se conecta inmediatamente después de las baterías para actuar como interruptor general y voltímetro digital en vivo, permitiendo monitorear el voltaje en *pits* antes de salir a la pista.
* **Regulador de Voltaje Step-Down (Buck Converter LM2596):** Ubicado en el centro del chasis junto al relé. Recibe los $7.4\text{V}$ del banco de baterías y los convierte a $5.0\text{V}$ estables para alimentar en paralelo a la Raspberry Pi 5 y al servomotor de dirección, aislando la electrónica lógica de las interferencias.
* **Puente H (Driver L298N):** Se instala en la sección central-posterior, lo más cerca posible del Motor Grande EV3. Su cercanía minimiza la longitud de los cables de potencia de $7.4\text{V}$, reduciendo la resistencia eléctrica y la caída de tensión en las conmutaciones de PWM.
* **Módulo Frontal Personalizado (Raspberry Pi AI Camera):** Estructura vertical diseñada e impresa exclusivamente por el equipo para montar la cámara en la parte frontal elevada. Su elevación e inclinación calculadas garantizan un campo de visión (*FOV*) despejado e inmune a las vibraciones para la clasificación por IA de los pilares verdes y rojos.
* **Unidad Central de Procesamiento (Raspberry Pi 5):** Se destina una plataforma elevada de protección dentro del chasis. Su ubicación centraliza las conexiones del bus I2C (sensores ToF VL53L5CX), las señales PWM del servomotor, las salidas hacia el L298N y el puerto CSI de la cámara, optimizando el ruteo de cables y manteniendo el "cerebro" del robot seguro y ventilado.

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
-	Motor Grande EV3
-	Servo Motor 
-	Puente H
- Regulador Step Down
-	Switch
-	STMicroelectronics VL53L5CX
-	Pilas 18654

  
A continuación, se presentará el Diagrama de Cableado que ilustra cómo estos componentes se interconectan para funcionar en armonía.

![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/Dise%C3%B1o%20sin%20t%C3%ADtulo.jpg)

Explicación del Diagrama Expuesto

Aquí tienes la explicación técnica detallada del **diagrama de cableado (esquemático eléctrico)**, redactada en formato **Markdown (`.md`)** lista para copiar y pegar directamente en la documentación de tu repositorio de GitHub:

# 🔌 Explicación Detallada del Diagrama de Cableado (Esquemático Eléctrico)

El diseño del circuito eléctrico del robot sigue una arquitectura **de fuente única con división de etapas (Potencia vs. Lógica)**. Esta topología garantiza que los motores de alta demanda de corriente no interfieran con la sensibilidad de la **Raspberry Pi 5**, la **AI Camera** y los sensores láser ToF.

A continuación, se detalla el flujo de la corriente y la función de cada trayectoria representada en el esquema eléctrico:

---

## 🔴 1. Línea Principal de Alimentación y Control de Potencia (Línea Roja y Azul)

* **Fuente de Energía (2x Baterías Li-ion 18650):** 
  * Las celdas están conectadas en serie, entregando una tensión nominal combinada de **$7.4\text{V}$**.
  * El polo positivo (cable rojo) y el negativo (cable azul) van conectados directamente a la entrada del **Relé Electrónico con Display Digital**.
* **Relé Electrónico con Display:**
  * Funciona como la primera barrera de seguridad. Monitorea y muestra en la pantalla de 7 segmentos el voltaje en tiempo real del banco de baterías.
  * Permite el corte/paso digital de la corriente y protege el sistema contra caídas extremas de voltaje (*Corte por bajo voltaje*).
* **Interruptor Físico (Switch Principal):**
  * Conectado en serie en la línea positiva ($+$) inmediatamente después del relé. Funciona como el encendido/apagado general mecánico del robot.

---

## ⚡ 2. División de Etapas: Potencia vs. Lógica Regulada

Una vez que la corriente atraviesa el switch principal, la línea de $7.4\text{V}$ se divide en dos nodos paralelos:

### A. Etapa de Potencia Nativa ($7.4\text{V}$) — Motores de Alta Corriente
* **Puente H (Driver de Motor L298N):**
  * Recibe los **$7.4\text{V}$ nativos** directamente de la batería en sus bornes de entrada ($V_{CC}$ y $GND$). Esto le otorga al **Motor Grande LEGO EV3** de tracción el máximo torque y la mayor velocidad posible en rectas.
  * Las salidas del Puente H se conectan a los bornes del motor EV3 para alternar el sentido de giro y la velocidad mediante Modulación por Ancho de Pulso (PWM).

### B. Etapa Lógica Regulada ($5.0\text{V}$) — Electrónica de Control
* **Regulador Step-Down (Buck Converter LM2596):**
  * Recibe la línea positiva de $7.4\text{V}$ y la reduce de forma conmutada a exactamente **$5.0\text{V}$ estables con hasta $5\text{A}$ de salida**.
* **Raspberry Pi 5 y AI Camera:**
  * La salida regulada de $5.0\text{V}$ alimenta la Raspberry Pi 5 a través de los pines de alimentación GPIO ($5\text{V}$ y $GND$).
  * La **Raspberry Pi AI Camera** se alimenta internamente desde el bus de datos y energía (conector CSI/MIPI) conectado a la Pi 5.
* **Servomotor de Dirección (MG90S / MG995):**
  * Para evitar sobrecargar la Raspberry Pi 5, la línea de potencia ($V_{CC}$ y $GND$) del servomotor se toma **directamente de la salida regulada del Buck Converter ($5\text{V}$)**.
  * El cable amarillo de señal de control ($PWM$) del servomotor se conecta a un pin GPIO de la Raspberry Pi 5 para dictar el ángulo exacto de la dirección Ackermann.

---

## 🔵 3. Masa Común (GND Unificado)

Un aspecto crítico para el correcto funcionamiento del software y los buses de comunicación es el **GND Unificado** (representado por todas las líneas azules del esquema):

* Todas las tierras del sistema (Baterías, Relé, Puente H, Regulador Buck, Raspberry Pi 5 y Servomotor) están interconectadas en el mismo nodo.
* **Justificación Técnica:** Mantener un plano de masa común evita que existan voltajes flotantes entre los componentes. Esto garantiza que las señales lógicas PWM enviadas desde la Raspberry Pi 5 hacia el servomotor y hacia el Puente H sean leídas sin ruido ni interferencias electromagnéticas.

---

## 🛠️ Resumen de Conexiones por Pines


```

[Baterías 18650 (7.4V)] ──► [Relé con Display] ──► [Switch] ──┬──► [Puente H L298N] ──► Motor Grande EV3
└──► [Buck LM2596] ──┬──► Raspberry Pi 5 ──► AI Camera
└──► Servo MG995 (VCC/GND)
▲
[Raspberry Pi 5 GPIO Pin PWM] ──────────────────────────────────────────────────────────────┘

```




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
La **Raspberry Pi AI Camera** es fundamental para nuestro robot porque permite la **IA en el borde**, procesando visión directamente en el chip. Esto libera recursos de la Pi 5, reduce la latencia y la necesidad de ancho de banda. Su **alta resción** y la capacidad de enviar **metadatos de IA pre-procesados** simplifican el desarrollo. Además, es **energéticamente eficiente**, clave para la autonomía del robot. En definitiva, convierte a nuestro robot en un agente **inteligente y reactivo** capaz de percibir e interpretar su entorno de forma autónoma.

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

###   Servomotor

Servomotor
Un servomotor es un tipo de motor especial que se diferencia de los motores de corriente continua (DC) o alterna (AC) convencionales por su capacidad de controlar con precisión su posición angular, velocidad y, en algunos casos, su aceleración. Piensa en él como un motor que no solo gira, sino que sabe exactamente dónde está y puede ir a una posición específica y mantenerla, incluso si hay una fuerza externa que intenta moverlo.

---

**_Características Principales:_**

* **Control de Posición Preciso:** Esta es su característica principal. A diferencia de un motor DC que gira libremente cuando se le aplica voltaje, un servomotor puede ser instruido para moverse a un ángulo específico (por ejemplo, 45 grados, 90 grados, etc.) y mantenerse allí.
* **Sistema de Lazo Cerrado:** Un servomotor siempre forma parte de un sistema de "lazo cerrado". Esto significa que tiene un mecanismo de retroalimentación (generalmente un potenciómetro o un encoder) que constantemente informa al controlador sobre la posición actual del eje del motor. El controlador compara esta posición con la posición deseada y ajusta la energía al motor para corregir cualquier desviación.
* **Componentes Internos:**
    * **Motor DC o AC:** El motor eléctrico real que genera el movimiento.
    * **Engranajes reductores:** Un sistema de engranajes que reduce la velocidad del motor pero aumenta su torque (fuerza de giro), permitiendo movimientos más controlados y con mayor fuerza.
    * **Sensor de Posición (Potenciómetro/Encoder):** Mide la posición actual del eje del motor y envía esta información al controlador.
* **Tipos de Señal de Control:** Generalmente se controlan mediante señales de Modulación por Ancho de Pulso (PWM). La duración del pulso determina la posición a la que debe moverse el servomotor.

---

El **servomotor** es crucial para nuestro robot porque permite un **control de posición angular preciso**, a diferencia de los motores DC simples. Esto es fundamental para que el robot realice **movimientos exactos y articulados**, como orientar cámaras o manipular objetos. Su sistema de lazo cerrado y el control por PWM simplifican la programación de movimientos complejos, asegurando que el robot interactúe con su entorno de forma controlada y efectiva.

![Servomotor](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/Schemes/servomotor.jpg)

---

### 📊 Tabla Comparativa de Aplicación en Competencia

| Característica | Motor Grande EV3 (Tracción) | Servo Motor (Dirección) |
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

  ![Servomotor](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/VL53L5X.jpg)


---

#### ⚡ Regulador de Voltaje Step Dwon

Un regulador de voltaje Step-Down (o Buck Converter) es un circuito electrónico de conversión de corriente directa a corriente directa (DC-DC) de alta eficiencia. Su función principal es reducir (bajar) un voltaje de entrada más alto a un voltaje de salida más bajo y estabilizado, manteniendo la tensión constante sin importar los picos o caídas en la alimentación principal.

A diferencia de los reguladores lineales tradicionales (como el famoso LM7805), un regulador Step-Down opera mediante conmutación (PWM), lo que significa que "enciende y apaga" la corriente a altas frecuencias a través de un transistor y un inductor para ajustar el voltaje deseado sin desperdiciar energía.
---
**_Características Esenciales:_**

* **Alta Eficiencia Energética (85% – 95%):** Al ser un regulador conmutado, prácticamente no desperdicia energía. En lugar de quemar el exceso de voltaje en forma de calor, convierte la energía de manera eficiente.
* **Amplio Rango de Entradas y Salidas Ajustables:** Soporta voltajes de entrada elevados (ej. $7\text{V} - 28\text{V}$) y permite ajustar el voltaje de salida (ej. a $5\text{V}$ fijación continua) mediante un potenciómetro de precisión (Trimpot).
* **Baja Generación de Calor:** No requiere disipadores de calor voluminosos, lo que ahorra espacio y peso dentro de la estructura física del robot.
* **Regulación de Salida Estable (Bajo Ripple / Rizado):** Mantiene el voltaje de salida en una tolerancia muy fina, protegiendo los componentes sensibles contra fluctuaciones.
* **Protección Incorporada:** La mayoría de los módulos comerciales (como el LM2596 o MP1584) incluyen protección contra sobrecorriente, cortocircuitos y sobrecalentamiento.
---
**_¿Qué beneficios trae a nuestro robot en la WRO 2026?_**

En una arquitectura como la de nuestro robot, donde conviven componentes informáticos de alto consumo (Raspberry Pi 5, Raspberry Pi AI Camera) con componentes mecánicos de potencia (motores y actuadores LEGO EV3), el regulador Step-Down es una pieza crítica por los siguientes motivos:

* **Aislamiento Electrónico y Protección de la Raspberry Pi 5:** La Raspberry Pi 5 requiere un suministro de $5\text{V}$ extremadamente limpio y continuo. Las baterías LiPo o Li-Ion entregan voltajes mayores (ej. $7.4\text{V}$ a $11.1\text{V}$) y bajan progresivamente a medida que se descargan. El Step-Down garantiza que la Pi reciba siempre exactamente $5\text{V}$, evitando que la tarjeta se reinicie o se dañe por un pico de sobrevoltaje.
* **Prevención de Bajones de Tensión (Brownouts):** Cuando el motor grande LEGO EV3 de tracción acelera bruscamente o el motor mediano de dirección cambia de sentido, se producen caídas severas de voltaje en la batería principal. El regulador Step-Down absorbe estas caídas y mantiene la salida de $5\text{V}$ estable, evitando que la IA o los sensores ToF (VL53L5CX) pierdan energía a mitad de una maniobra.
* **Mayor Autonomía y Eficiencia para el Time Attack:** Como el regulador convierte la energía con una eficiencia cercana al $90\%$, no desperdicia la carga de la batería en forma de calor. Esto nos otorga mayor tiempo de prueba en pista y asegura que el robot mantenga el mismo rendimiento y velocidad constante desde la primera hasta la última vuelta.
* **Reducción de Peso y Compactación de Espacio:** Al no requerir disipadores metálicos pesados, nos permite mantener el chasis liviano y dentro de las dimensiones y restricciones de peso oficiales del reglamento de la WRO.


El **Regulador de Voltaje Electrónico** es indispensable para el robot porque asegura una **alimentación eléctrica constante y estable** específicamente para el/los servomotor(es). Es vital para:

* **Proteger los servomotores:** Garantiza que reciban siempre el voltaje óptimo, previniendo daños por fluctuaciones de la batería o picos de carga.
* **Asegurar su rendimiento preciso:** Un voltaje estable es clave para el funcionamiento fiable y la precisión de movimiento del/de los servomotor(es).
* **Maximizar la autonomía:** Al usar reguladores conmutados eficientes, minimiza la pérdida de energía en la alimentación del/de los servomotor(es), prolongando la duración de la batería del robot.

En esencia, el regulador es fundamental para la **fiabilidad y la prolongación de la vida útil** de los componentes eléctricos del robot.

"Utilizamos un regulador Step-Down para alimentar la Raspberry Pi 5 y los sensores a $5\text{V}$ estables a partir de nuestra batería principal. Gracias a su eficiencia del $90\%$, evitamos reinicios por caídas de tensión cuando los motores EV3 demandan picos de corriente, garantizando la estabilidad de la IA y reduciendo el peso en el chasis."

![Regulador de Voltaje](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/Regulador%20Step%20Down.jpg)

#### 📸 Relé Electrónico con Display (Módulo de Control de Potencia Digital)

Un relé electrónico con display es un interruptor conmutado digital de estado sólido o electromecánico que incorpora una pantalla (usualmente LED de 7 segmentos o pantalla OLED) y un microcontrolador interno. Su función principal es abrir o cerrar circuitos de alta potencia mediante señales de control de bajo voltaje, permitiendo visualizar en tiempo real parámetros críticos como el estado de conmutación, el voltaje de la línea, la corriente o el tiempo de activación programado.

A diferencia de los relés mecánicos simples que solo reaccionan al paso de corriente en la bobina, este módulo permite monitorear y gestionar de forma inteligente el flujo de energía sin depender de pantallas externas.

---
**_Características Sobresalientes:_**

* **Monitoreo Visual en Tiempo Real (Display Integrado):** Muestra de forma inmediata el estado del canal (ON/OFF), el voltaje de la batería principal, la corriente consumida o temporizadores de corte de energía.
* **Aislamiento Optoelectrónico (Optoacoplador):** Separa físicamente el circuito de control de bajo voltaje (ej. $3.3\text{V} / 5\text{V}$ de la Raspberry Pi o Arduino) del circuito de alta potencia de los motores, protegiendo los chips lógicos contra retornos de corriente electromagnética (EMF).
* **Conmutación Inteligente / Temporizada:** Permite programar retardos de encendido o apagado (Time-Delay), protegiendo la electrónica de picos de corriente durante la etapa de arranque (Inrush Current).
* **Retroalimentación de Seguridad y Diagnóstico:** Facilita el diagnóstico rápido en boxes (Pits) durante la competencia; el equipo puede verificar con un vistazo al display si el módulo tiene energía o si se ha disparado una protección.


---
**_¿Qué beneficios trae a nuestro robot en la WRO 2026?_**

En una arquitectura de carrera donde compartimos la energía de la batería de litio entre la Raspberry Pi 5 y motor LEGO EV3 junto a un servo motor, la integración de este módulo aporta los siguientes beneficios clave:

* **Diagnóstico e Inspección Rápida en Carrera:** Durante las pruebas y mangas de la WRO, no hay tiempo para conectar un multímetro. El display incorporado nos permite verificar instantáneamente la salud y el voltaje de la batería de litio, asegurándonos de no salir a la pista con una batería descargada que comprometa el rendimiento de la IA o los sensores ToF.
* **Protocolo de Encendido Secuencial (Protección de la Raspberry Pi 5):** El software o la lógica del relé permite retrasar el suministro de corriente a los motores LEGO EV3 hasta que la Raspberry Pi 5 haya arrancado por completo su sistema operativo. Esto evita que los picos de arranque del motor grande afecten el proceso de inicialización de la computadora central.
* **Parada de Emergencia y Protección Automática (Corte por Bajo Voltaje):** Si el voltaje de las baterías cae por debajo del límite seguro (para evitar dañar celdas Li-ion/LiPo), el módulo puede cortar automáticamente la potencia hacia la etapa de motores, alertando visualmente en el display y protegiendo el sistema eléctrico de sobrecargas o cortocircuitos.
* **Conmutación Segura desde la Raspberry Pi 5 / Arduino:** Permite que las señales lógicas de los pines GPIO abran o cierren líneas de alta corriente con total seguridad, garantizando cero interferencias electromagnéticas sobre el bus I2C de la AI Camera y los sensores láser VL53L5CX.

"Integramos un relé electrónico con display para gestionar de manera inteligente la alimentación principal del robot. Nos otorga telemetría visual inmediata del voltaje en boxes y proporciona un aislamiento completo entre los pines de la Raspberry Pi 5 y los motores LEGO EV3, evitando ruidos electromagnéticos y protegiendo el sistema contra sobredescargas de la batería."

![La Raspberry Pi AI Camera](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Schemes/rel%C3%A9%20electronico%20con%20display%20arduino.jpg)


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

### 3. Encoders Ópticos Internos (Motores LEGO EV3 y servomotor)

Hemos eliminado los sensores rotacionales externos acoplados a motores DC convencionales. En su lugar, aprovechamos los **tacómetros digitales (encoders) integrados** tanto en el motor grande (propulsión) como en el motor mediano (dirección) del kit LEGO EV3.
* **Misión Crítica en Motor Grande (Tracción):** Mide los grados de rotación exactos de las ruedas traseras. El software en Python procesa estos datos para ejecutar algoritmos de **odometría de lazo cerrado**, calculando la distancia recorrida en la pista para planificar con exactitud la frenada, el conteo de vueltas de respaldo y la secuencia de reversa para el estacionamiento en paralelo.
* **Misión Crítica Servomotor (Dirección):** Proporciona retroalimentación instantánea sobre la posición angular real de las manguetas delanteras. Esto permite saber con precisión milimétrica el ángulo de giro del sistema Ackermann en cada frame, corrigiendo cualquier desviación provocada por la fricción del suelo.

  ## 3. Consumo de Energía
## 3. Estimación del Consumo Energético Unificado

Dado que el vehículo ha migrado a un sistema de alimentación único basado exclusivamente en baterías de Litio, todo el consumo se consolida en una sola línea de [potencia. El consumo estimado bajo condiciones de máxima exigencia en pista (*Time Attack*) es el siguiente:


# ⚡ Análisis de Consumo Energético y Presupuesto de Potencia

Para garantizar la estabilidad operativa del robot durante las mangas oficiales de la WRO 2026, realizamos un cálculo minucioso del presupuesto de potencia (*Power Budget*) basado en la arquitectura de conexiones eléctricas del sistema.

El circuito se alimenta mediante un arreglo en serie de **2 celdas Li-ion 18650 ($7.4\text{V}$ nominales)**, dividiendo la carga entre una etapa de potencia nativa ($7.4\text{V}$) y una etapa lógica regulada a través del convertidor *Step-Down* LM2596 ($5.0\text{V}$).

---

## 📊 Tabla de Consumo Energético por Componente

| Componente | Línea de Alimentación | Voltaje de Operación | Consumo Promedio | Consumo Pico (Stall / Max) | Potencia Máx. Estimada |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Raspberry Pi 5** | Salida Buck ($5\text{V}$) | $5.0\text{V}$ | $1.5\text{ A}$ | $2.7\text{ A}$ | $13.5\text{ W}$ |
| **Raspberry Pi AI Camera** | Bus CSI/GPIO Pi 5 | $5.0\text{V}$ | $250\text{ mA}$ | $350\text{ mA}$ | $1.75\text{ W}$ |
| **Servomotor MG90S / MG995** | Salida Buck ($5\text{V}$) | $5.0\text{V} - 6.0\text{V}$ | $150\text{ mA}$ | $700\text{ mA}$ | $3.5\text{ W}$ |
| **Motor Grande EV3 (Tracción)** | Puente H (Driver L298N) | $7.4\text{V}$ (Nativo) | $300\text{ mA}$ | $2.0\text{ A}$ | $14.8\text{ W}$ |
| **Módulo Relé con Display Digital** | Directo Batería | $7.4\text{V}$ (Nativo) | $50\text{ mA}$ | $100\text{ mA}$ | $0.74\text{ W}$ |
| **Arreglo de Sensores ToF VL53L5CX** | Bus I2C / GPIO Pi 5 | $3.3\text{V} / 5.0\text{V}$ | $100\text{ mA}$ | $150\text{ mA}$ | $0.75\text{ W}$ |

---

## 📈 Resumen Global de Potencia y Eficiencia

* **Tensión Nominal del Banco de Baterías:** $7.4\text{V}$ ($2 \times 3.7\text{V}$ Li-ion 18650 en serie).
* **Consumo Promedio en Carrera (*Time Attack*):** $\sim 2.35\text{ A}$ @ $7.4\text{V}$ ($\sim 17.4\text{ W}$).
* **Consumo Máximo Transitorio (Picos de Arranque):** $\sim 5.0\text{ A} - 6.0\text{ A}$ @ $7.4\text{V}$ ($\sim 35\text{ W}$).
* **Eficiencia del Regulador Step-Down (LM2596):** $\sim 88\% - 90\%$ de conversión hacia la línea de $5\text{V}$.

---

## 🔋 Cálculo de Autonomía en Pista

Utilizando un paquete de celdas 18650 con una capacidad real combinada de **$2200\text{ mAh}$ ($16.28\text{ Wh}$)**:

$$\text{Autonomía Teórica} = \frac{\text{Capacidad de Batería (Wh)}}{\text{Consumo Promedio (W)}} = \frac{16.28\text{ Wh}}{17.4\text{ W}} \approx 0.93\text{ horas} \quad (\approx 56\text{ minutos})$$

> 💡 **Conclusión de Autonomía:** Aplicando un factor de seguridad del $20\%$ para mitigar la degradación térmica y picos imprevistos, el robot garantiza **más de 40 minutos de operación continua a máximo rendimiento**, superando holgadamente la duración de las pruebas de pista de la WRO 2026.

---

## 🛠️ Desglose del Esquemático Eléctrico

1. **Línea Principal de Control:** Las baterías entregan corriente directa al **Relé Digital**, el cual actúa como interruptor general y voltímetro de protección antes de pasar por el **Switch Físico**.
2. **División de Etapas:**
   * **Etapa de Potencia ($7.4\text{V}$):** Alimenta directamente el conector de potencia del **Puente H (L298N)** para entregar el mayor torque posible al motor de tracción EV3.
   * **Etapa Lógica y Control ($5.0\text{V}$):** El regulador **Step-Down** convierte los $7.4\text{V}$ a $5.0\text{V}$ estables, alimentando en paralelo el GPIO de la **Raspberry Pi 5** y el puerto del **Servomotor de Dirección**.
3. **Manejo de Masa Común (GND Unificado):** Todos los componentes comparten una misma línea de tierra (cable azul en el diagrama), evitando flotaciones de voltaje y garantizando una señal PWM limpia para la dirección y el control del Puente H.
---

## 4. Justificación Técnica de Selección de Componentes

La selección del hardware obedece a criterios estrictos de precisión cinemática, robustez mecánica, eficiencia energética y velocidad de procesamiento, reemplazando soluciones de baja especificación por módulos de grado de ingeniería adaptados a la competencia:

### 🏎️ Actuadores y Control de Movimiento
* **Motor Grande LEGO EV3 (Tracción):** Se seleccionó para el eje motriz debido a su encoder óptico interno de alta resolución. Nos permite prescindir de sensores ópticos externos, calculando la odometría de forma matemática para el control exacto de distancias, aceleración y maniobras de estacionamiento.
* **Driver de Potencia Puente H (L298N):** Encargado de conmutar la corriente hacia el motor grande EV3. Al alimentarse directamente con los **$7.4\text{V}$ nativos** del banco de baterías, entrega el máximo torque y velocidad posibles, permitiendo un control fino del sentido de giro y velocidad mediante Modulación por Ancho de Pulso (PWM).
* **Servomotor Digital de Piñonería Metálica (MG995 / MG90S):** Sustituye los motores y servomotores convencionales en la dirección Ackermann. Ofrece un torque elevado ($\ge 10\text{ kg}\cdot\text{cm}$) y elimina el juego mecánico (*backlash*) en las manguetas delanteras. Su control mediante impulsos PWM por hardware libera ciclos de procesamiento en la CPU principal.

### 👁️ Sistema de Percepción y Visión Computacional
* **Arreglo Láser ToF (VL53L5CX):** Reemplaza a los sensores ultrasónicos tradicionales (los cuales sufren de reflexiones falsas y eco en las esquinas). Al medir por Tiempo de Vuelo (*Time-of-Flight*) mediante matrices infrarrojas de $8 \times 8$, proporciona una telemetría milimétrica de la distancia hacia los muros, siendo completamente inmune a las variaciones de luz ambiental del recinto.
* **Raspberry Pi AI Camera:** Es el pilar del sistema de visión. Al procesar modelos de aprendizaje profundo directamente en su acelerador de red neuronal integrado (*Edge AI*), clasifica y diferencia instantáneamente las señales y obstáculos sin consumir ciclos de reloj de la CPU de la Raspberry Pi 5. Esto elimina el latido (*lag*) en la toma de decisiones dinámicas.
* **Computadora Central (Raspberry Pi 5):** Coordina la fusión sensorial del arreglo ToF y la cámara de IA, ejecutando el algoritmo de control en Python para ajustar la dirección, la velocidad y la trayectoria del vehículo en tiempo real.

### ⚡ Red Electrolítica y Gestión de Energía
* **Banco de Baterías Li-ion 18650 ($7.4\text{V}$):** Sustituye los *power banks* comerciales voluminosos. Su arreglo en serie otorga una alta densidad energética y capacidad de descarga en corriente ($\ge 5\text{A}$), reduciendo la masa del chasis y bajando el centro de gravedad.
* **Convertidor Step-Down Buck (LM2596):** Regulador conmutado de alta eficiencia ($\sim 90\%$) que reduce los $7.4\text{V}$ a unos **$5.0\text{V}$ estables**. Alimenta la Raspberry Pi 5 y el servomotor de dirección, protegiendo la electrónica lógica de bajones de tensión (*brownouts*) cuando el motor de tracción demanda picos de corriente.
* **Módulo Relé Electrónico con Display Digital:** Funciona como el sistema de gestión y protección eléctrica. Incorpora un voltímetro digital en tiempo real para verificar la carga de las baterías en *pits* y ofrece un aislamiento optoelectrónico que protege los microcontroladores contra retornos inductivos.


---

## 🚗 Gestión de Movilidad

E# 🏎️ Diseño Mecánico y Arquitectura del Chasis Híbrido

El vehículo utiliza una configuración cinemática de tipo automóvil (*Ackermann Steering*): las ruedas traseras proporcionan la fuerza de tracción principal, mientras que el eje delantero gestiona la dirección orientable. Su estructura física destaca por un **diseño híbrido sostenible y modular**, combinando la flexibilidad de las piezas **LEGO EV3**, la reutilización de componentes de ingeniería de nuestro robot anterior y diseños customizados propios.

### ⚙️ Integración Mecánica y Componentes Estructurales

* **Chasis Rígido con Piezas LEGO EV3:** Se utilizan vigas y elementos estructurales de LEGO EV3 como esqueleto base para mantener la rigidez del chasis y permitir un acople perfecto con el motor grande de tracción trasera y su sistema de transmisión.
* **Bases 3D Recicladas (Optimización de Recursos):** En línea con las buenas prácticas de ingeniería y sostenibilidad, reutilizamos las bases de fijación impresas en 3D de nuestro robot de la edición pasada. Estas placas y soportes adaptados nos permiten montar de forma segura y limpia el circuito eléctrico: las celdas Li-ion 18650, el driver L298N, el regulador Step-Down LM2596 y el módulo de relé con display.
* **Módulo Personalizado para la Cámara de IA (Diseño Propio):** Diseñamos e imprimimos en 3D un soporte exclusivo y dedicado para la **Raspberry Pi AI Camera**. Este módulo coloca la cámara a la altura e inclinación exactas necesarias para optimizar el campo de visión (*FOV*), aislando el lente de las vibraciones del chasis para garantizar un encuadre estable durante el reconocimiento de los pilares.
* **Dirección Tipo Ackermann:** Un servomotor digital acciona el mecanismo de dirección sobre las ruedas delanteras. Al ajustar los ángulos de giro de forma asimétrica, se evita el derrape de las llantas en curvas cerradas y se garantiza un control de trayectoria de alta precisión.

Esta combinación entre piezas LEGO EV3, el reciclaje técnico de bases 3D anteriores y el desarrollo de nuestro propio módulo para la cámara da como resultado un vehículo ágil, robusto y preparado para las exigencias de la WRO 2026.

---
# *Lenguaje de Programación*

---

# Detección de Objetos y Límites de Pista 🤖
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/Triple-Threat-AI/blob/main/SRC/Python.png)

Para capacitar a nuestro robot con la habilidad de "ver" su entorno, integramos un conjunto de sensores clave. Si bien los sensores de proximidad (como los ultrasónicos o infrarrojos) son cruciales para detectar obstáculos cercanos y medir distancias, el componente central de nuestra visión es la Cámara Raspberry Pi AI.

La Cámara Raspberry Pi AI, en combinación con algoritmos de visión por computadora desarrollados en Python, aprovecha librerías potentes como OpenCV para el procesamiento avanzado de imágenes. Esta sinergia nos permite no solo identificar la presencia de obstáculos, sino también clasificarlos eficazmente, ya sean conos u otros elementos estáticos presentes en el entorno de la pista. La información obtenida de esta detección es indispensable para que el robot tome decisiones de navegación precisas, como la desaceleración o la evasión.

Paralelamente, para asegurar que el robot se mantenga dentro de su trayectoria, utilizamos la Cámara Raspberry Pi AI para el reconocimiento de los bordes de la pista. A través del procesamiento de imágenes en Python, el sistema analiza las características visuales de la pista, incluyendo líneas y paredes, permitiendo al robot ajustar su dirección de forma continua para permanecer dentro de los límites predefinidos.

# DIAGRAMAS DE LOS CODIGOS 


# 🧠 Arquitectura de Software y Flujo de Datos del Sistema de Navegación

En este apartado se describe la arquitectura de control, el procesamiento de señales y la lógica de toma de decisiones implementada en el robot. El sistema procesa lecturas de sensores de tiempo de vuelo (ToF), filtra las perturbaciones físicas, determina la maniobra mediante una máquina de estados y aplica la respuesta correspondiente a los actuadores de tracción y dirección.

---

## 📐 Diagrama de Flujo de Datos (DFD)

El pipeline de navegación está diseñado bajo una arquitectura modular desacoplada en procesos independientes:

[3x Sensado VL53L5CX] ──► (1.0 Adquisición) ──► (2.0 Depuración) ──► (3.0 Reducción)
│
[Piloto Web] ◄── Telemetría ── (6.0 Actuadores) ◄── (5.0 Decisión) ◄── (4.0 Suavizado)
│                                                    ▲
└────── Parámetros / Armado ─────────────────────────┘


---

## ⚙️ Desglose de Procesos

### 1.0 Adquisición de Rejillas (`arranque.py` / `monitor.py`)
* **Función:** Captura sincrónica de las matrices de $4 \times 4$ zonas de los tres sensores Láser ToF VL53L5CX a través del bus I²C.
* **Mecanismo:** Estampa un sello temporal (*timestamp*) y número de fotograma (*frame number*) a cada captura para garantizar la trazabilidad del dato en el bus.

### 2.0 Depuración y Filtrado de Zonas (`percepcion.py`)
* **Función:** Eliminación de lecturas corruptas o físicamente imposibles generadas por rebotes o inclinación del chasis.
* **Criterios de Descarte:**
  * Si el chasis sufre un cabeceo exabrupto (*pitch*), la matriz frontal completa es ignorada temporalmente.
  * Se aplica un filtro de calidad zona por zona descartando lecturas con estados no fiables ($\notin \{5, 9, 4, 13\}$), distancias fuera del rango efectivo ($d < 25\text{ mm}$ o $d > \text{anillo}$), alta variabilidad ($\sigma > \max(15, 8\% \cdot d)$) o señal débil ($\text{señal} < 2$).

### 3.0 Reducción a Vector de Distancias (`percepcion.py`)
* **Función:** Transforma una matriz bidimensional cruda de 48 zonas ($3 \times 16$) en un vector compacto de 3 valores representativos (`frente`, `izquierda`, `derecha`).
* **Lógica:** Selecciona el segundo punto más cercano por lado para evitar falsos positivos y asigna a cada flanco una etiqueta categórica de estado (`pared`, `cerca`, `libre` o `ciego`).

### 4.0 Suavizado Temporal (`navegacion.py`)
* **Función:** Atenuación del ruido de alta frecuencia en las mediciones antes de entrar a la máquina de estados.
* **Filtros Aplicados:**
  * **Frente:** Filtro de mediana con una ventana temporal de 3 fotogramas.
  * **Laterales:** Filtro de moda (categoría mayoritaria) sobre una ventana temporal de 7 fotogramas.
  * **Sincronización:** La actualización del algoritmo se dispara únicamente al recibir un fotograma nuevo, evitando re-calculos innecesarios en el bucle principal.

### 5.0 Decisión de Maniobra y Selección de Sentido (`navegacion.py`)
* **Máquina de Estados de 5 Prioridades:**
  1. *Esquina:* Detección de giro obligado.
  2. *Antichoques:* Maniobra evasiva de emergencia.
  3. *Recuperación del Volantazo:* Corrección progresiva de trayectoria tras un giro brusco.
  4. *Deriva:* Compensación de alineación lateral.
  5. *Recta Libre:* Aceleración constante en tramo despejado.
* **Subproceso 5.1 (Votar Sentido):** En la primera esquina del circuito, evalúa cuál lado presenta un perfil más abierto, emite un voto y congela la dirección de giro (`IZQ` / `DER`) para el resto de las vueltas.

### 6.0 Aplicación a Actuadores (`actuadores.py`)
* **Función:** Conversión del vector de comando (`tracción`, `volante`) normalizado en el rango $[-1, 1]$ a señales físicas para los componentes hardware:
  * **Dirección:** Mapeo a microsegundos ($\mu\text{s}$) de pulso PWM para el servomotor ($500\mu\text{s} - 2000\mu\text{s}$).
  * **Tracción:** Mapeo a ciclo de trabajo (*Duty Cycle*) PWM hacia el Driver Puente H L298N.
* **Mecanismo de Seguridad (*Watchdog*):** Si se pierde el pulso de armado enviado desde el tablero web o falla el indicador de latido (*heartbeat*), los actuadores se detienen inmediatamente.

---

## 💾 Almacenes de Datos en Memoria (D1 - D5)

| Identificador | Nombre del Almacén | Contenido | Proceso Escritor | Procesos Lectores |
| :--- | :--- | :--- | :--- | :--- |
| **D1** | Rejillas Vigentes | Matriz cruda (distancia, estado, señal, $\sigma$), FPS y número de fotograma. | `1.0` | `2.0` |
| **D2** | Ventanas Temporales | Historial de las últimas 3 lecturas frontales y 7 lecturas laterales. | `4.0` | `4.0` |
| **D3** | Plan Vigente | Estado de la máquina, sentido congelado, conteo de esquinas y comandos de control. | `5.0` | `6.0`, `Piloto Web` |
| **D4** | Constantes y Armado | Parámetros de velocidad, umbrales de peligro, tiempos de giro y estado del *watchdog*. | `Piloto Web` | `5.0`, `6.0` |
| **D5** | Votos del Sentido | Registro de votos acumulados y sentido de giro bloqueado. | `5.1` | `5.1` |

---


 la arquitectura modular desacoplada en procesos independientes:
 
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/SRC/Diagrama%201.jpeg)
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/SRC/Diagrama%202.jpeg)
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/SRC/Diagrama%203.jpeg)
![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/SRC/Diagrama%204.jpeg)

![Motor Codificador Optico Makeblock 180](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/SRC/Diagrama%205.jpeg)










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

# 🔄 Cambios Estratégicos en la Arquitectura y Cambio de Componentes

Para optimizar la eficiencia dinámica, reducir el peso general y maximizar la velocidad de respuesta en la pista para la WRO 2026 (*Future Engineers*), el equipo **Triple Threat** ejecutó una reingeniería en los subsistemas de potencia y dirección.

---

## 1. Migración del Sistema de Alimentación: Eliminación del Power Bank por Celdas Li-ion 18650

Inicialmente, el sistema contaba con un Power Bank USB comercial dedicado exclusivamente a alimentar la Raspberry Pi 5. Tras las pruebas físicas en pista, rediseñamos la red eléctrica integrando un **paquete unificado de dos baterías Li-ion 18650 en serie ($7.4\text{V}$ nominales)** gestionadas a través de un regulador de voltaje *Step-Down* (Buck Converter) de alta eficiencia.

### 📊 Comparativa de Rendimiento

| Criterio | Configuración Anterior (Power Bank USB) | Nueva Configuración (2x Baterías 18650 + Buck) |
| :--- | :--- | :--- |
| **Peso y Volumen** | Elevado; estructura voluminosa y centro de gravedad alto. | Compacto; distribución simétrica e integración directa en chasis 3D. |
| **Suministro de Corriente** | Limitado por la electrónica interna del Power Bank ($\le 3\text{A}$). | Entrega de alta corriente sin cortes ($\ge 5\text{A}$ estables a $5\text{V}$). |
| **Eficiencia de Carga** | Pérdidas por doble conversión interna. | Línea directa de alta eficiencia ($\sim 90\%$) sin desperdicio térmico. |

### 🚀 Impacto en el Vehículo
* **Reducción de Masa Crítica:** Eliminamos el peso muerto de la carcasa y circuitos del Power Bank, bajando el centro de gravedad del vehículo.
* **Inmunidad a *Brownouts*:** La combinación de las celdas 18650 con el regulador Buck garantiza un flujo constante de $5\text{V}$ a $5\text{A}$ para la **Raspberry Pi 5** y la **AI Camera**, evitando reinicios accidentales cuando el motor de tracción genera picos de demanda.

---

## 2. Sustitución de Actuador de Dirección: Del Motor Mediano LEGO EV3 al Servomotor Digital MG995

En la geometría de dirección Ackermann, sustituimos el motor mediano de LEGO EV3 por un **servomotor digital de alta velocidad y piñonería metálica MG995**.

### 🔍 Justificación Técnica del Cambio

1. **Liberación de Cargas en CPU:** El motor mediano EV3 requería un lazo de control PID constante en Python mediante lecturas del encoder. El servomotor MG995 se controla directamente mediante **señales PWM por hardware**, liberando ciclos de reloj en la Raspberry Pi 5 para la visión computacional y los sensores ToF (VL53L5CX).
2. **Elevado Torque y Rigidez Mecánica:** Con un torque superior ($\sim 10 - 12\text{ kg}\cdot\text{cm}$) y engranajes de latón/aluminio, el MG995 elimina el juego mecánico (*backlash*) en las manguetas delanteras, resistiendo las fuerzas de fricción laterales en curvas cerradas.
3. **Respuesta Angular Inmediata:** La velocidad de corrección digital permite cambiar el ángulo de las ruedas en milisegundos, reaccionando de inmediato a las instrucciones del pipeline de la cámara de IA.

---

## 🛠️ Resumen de Beneficios en la Dinámica Global


```

[Baterías 18650 (7.4V)] ──► [Regulador Buck (5V/5A)] ──► Raspberry Pi 5 (Cero Reinicios)
└──► [Driver de Potencia]    ──► Motor Grande EV3 (Tracción)
──► Servo MG995 (Dirección PWM)

``` 
1. **Mayor Autonomía:** Maximización de la densidad energética para sesiones de prueba prolongadas.
2. **Chasis Híbrido Optimizado:** Menos volumen en el morro del vehículo y mayor agilidad espacial.
3. **Control Predictivo:** Sincronización precisa entre la percepción de los sensores y la respuesta de los actuadores sin cuellos de botella por procesamiento.

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

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Diagrama%201.jpeg)

### ⚙️ Desglose Técnico de la Telemetría por Sensor

El software asigna un código cromático dinámico a los valores numéricos (distancias en milímetros) recibidos por cada una de las zonas SPAD de los sensores:
* **Verde (Zonas Libres):** Distancias seguras y despejadas (típicamente $> 500\text{ mm}$ e inferiores a los límites físicos del carril).
* **Naranja/Marrón (Zonas de Transición / Aproximación):** Distancias intermedias que alertan de la proximidad de muros o el inicio de una curva.
* **Rojo (Zonas de Peligro / Obstáculo Inminente):** Distancias críticas (por debajo de $150\text{ mm} - 100\text{ mm}$) que indican una colisión inminente o la presencia directa de la base de un obstáculo.

---

### 🔍 Análisis de Escenario de Conducción en el Gráfico

Al evaluar las lecturas síncronas de los tres sensores, el software interpreta la física del entorno para guiar los actuadores LEGO EV3:

![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Diagrama%202.jpeg)


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
## 📐 Representación Vectorial 3D: Nube de Puntos (Point Cloud) y Mapeo Euclidiano

Para llevar la telemetría al siguiente nivel, nuestro software incluye un motor de proyección geométrica en tiempo real (módulo **"Solo 3D"**). Este componente traduce las matrices numéricas abstractas de los sensores ToF en un espacio tridimensional euclidiano estructurado sobre los ejes vectoriales tradicionales:
* **Eje X (Rojo):** Desplazamiento o coordenada lateral (Ancho de la pista).
* **Eje Y (Verde):** Vector de profundidad o distancia lineal hacia el frente (Eje longitudinal de avance).
* **Eje Z (Azul):** Cota de altura o cabeceo (Eje vertical de estabilidad).

La captura de pantalla de nuestras pruebas dinámicas (`Diagrama 2.jpeg`) ilustra el mapa tridimensional generado desde el centro de origen del robot (coordenada $0,0,0$ donde se cruzan las líneas de los ejes):

---

### ⚙️ Análisis de la Geometría del Entorno en 3D

El software calcula un vector de dispersión por cada zona SPAD activa de los sensores, mapeando la topología de la pista mediante dos clústeres o agrupaciones de puntos claramente diferenciados:

#### 1. Nube de Puntos Verdes (Zonas Libres y de Escape)
* **Análisis Visual:** Los puntos verdes se proyectan en el plano inferior a una distancia considerable en el eje longitudinal ($Y$). Están distribuidos en un abanico abierto que apunta hacia adelante y se desvía sutilmente hacia el cuadrante derecho.
* **Decisión Cinemática:** Estos vectores representan el asfalto libre de obstáculos y el suelo de la pista. Al registrar distancias largas en el eje $Y$, el software de navegación confirma que existe una ventana de escape óptima justo al frente y a la derecha. El coche tiene luz verde para acelerar utilizando el **motor grande LEGO EV3**.

#### 2. Nube de Puntos Amarillos (Detección de Estructuras y Muros)
* **Análisis Visual:** Se observan dos concentraciones de puntos amarillos elevados en el espacio. Un grupo forma una línea diagonal clara en el flanco izquierdo (eje $-X$) y otro grupo se concentra de manera densa en la zona central derecha.
* **Decisión Cinemática:** * El grupo de la izquierda mapea de forma tridimensional la pared o línea limítrofe izquierda del circuito.
    * La densa agrupación amarilla central derecha actúa como una alerta de obstáculo inmediato. El software detecta que una estructura vertical sólida está invadiendo el carril.

---

### 🏎️ Utilidad de la Proyección 3D en la Navegación Ackermann

Este pipeline de mapeo vectorial es el núcleo que permite al robot ejecutar una **conducción autónoma predictiva**:

1.  **Cálculo de la Tangente de Giro:** Al conocer las coordenadas tridimensionales $(X, Y, Z)$ de las nubes amarillas, el algoritmo calcula el centroide de la masa del obstáculo. En lugar de dar un volantazo brusco, el programa calcula el arco o radio de giro óptimo para rodear las esferas amarillas manteniendo la mayor velocidad lineal posible en el *Time Attack*.
2.  **Filtrado por Plano de Altura (Corte en Eje Z):** Al proyectar los datos en 3D, el software discrimina la altura de los objetos. Si los puntos se ubican muy abajo en el eje $Z$, el robot sabe que es el suelo y no un obstáculo. Esto evita que el vehículo interprete las imperfecciones superficiales o las uniones de la lona de la pista como muros, eliminando frenados fantasma.
3.  **Sincronización con la Cámara de IA:** Mientras la **Raspberry Pi AI Camera** encuadra el pilar en un plano bidimensional para clasificar su color, esta nube de puntos en 3D le otorga al robot la "profundidad de campo", permitiendo calcular con precisión milimétrica la trayectoria de evasión que debe ejecutar el **motor mediano LEGO EV3** de la dirección.
---

## 🎯 Optimización del Bus: Regiones de Interés (ROI) y Máscara de Horizonte

Para maximizar la eficiencia del procesamiento en la Raspberry Pi 5 y evitar la saturación en el muestreo por *Polling*, nuestro software implementa un algoritmo de aislamiento por **Regiones de Interés (ROI)**. Como se observa en la interfaz de telemetría (`Diagrama 3.jpeg`), no procesamos los 64 puntos de manera indiscriminada; aplicamos una **Máscara de Horizonte Matemático** que descarta dinámicamente las zonas irrelevantes para la conducción.


![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Diagrama%203.jpeg)
![Logo del Equipo Triple Threat](https://github.com/TripleThreat19/TripleThreat-IA_2.0/blob/main/Other/Leyenda.jpeg)

### 📊 Código de Estados y Umbrales de Proximidad

Utilizando los datos de calibración del sistema (`Leyenda.jpeg`), el firmware clasifica las distancias críticas en tres umbrales de control cinemático, ignorando las lecturas que caen fuera del plano de carrera:

* **🟩 Zona Libre ($> 50\text{ cm}$):** Trayectoria limpia. Permite al algoritmo de lazo cerrado incrementar el ciclo de trabajo (PWM) en el **motor grande LEGO EV3** para ganar velocidad lineal.
* **🟧 Precaución ($25 - 50\text{ cm}$):** Indica la aproximación a un límite de pista o pilar. Activa el estado de alerta en el código para preparar una maniobra de evasión.
* **🟥 Obstáculo ($< 25\text{ cm}$):** Umbral crítico de colisión inminente. Dicta una acción evasiva de alta prioridad o una corrección angular máxima al **motor mediano LEGO EV3**.
* **⬛ Suelo (Filtrado por Software):** Bloques marcados como `ROI` inactivos en gris oscuro. Son las zonas que apuntan debajo de la línea del horizonte; el software las ignora para evitar falsos positivos causados por imperfecciones en la superficie de la pista.

---

### 🔍 Análisis de la Escena Dinámica y Comportamiento Cinematográfico

En este cuadro de telemetría específico, el robot se encuentra en una condición de **curva cerrada o desvío crítico hacia la derecha**, interpretado de la siguiente manera por el software:

#### 1. Sensor Izquierdo (`0x30`) -> Estado: Obstáculo Crítico (`83 mm`)
La máscara de horizonte ha aislado una franja horizontal de 4 zonas activas justo por encima de la línea del suelo. El sensor registra valores críticos entre $85\text{ mm}$ y $115\text{ mm}$ (Saturación en **Rojo**).
* **Acción del Robot:** El flanco izquierdo está colapsado contra el muro de la pista. El control de centrado PID calcula un error de desvío masivo, enviando una instrucción de actuación inmediata para alejar el morro del vehículo de esa pared.

#### 2. Sensor Central (`0x31`) -> Estado: Vía Libre Abierta (`1060 mm`)
El sensor frontal confirma un pasillo completamente despejado a lo largo de su zona activa (lecturas estables de **Verde** entre $1195\text{ mm}$ y $1200\text{ mm}$). 
* **Acción del Robot:** Indica que el carril central está completamente abierto a un metro de distancia. La Raspberry Pi 5 valida que no hay obstáculos frontales directos interfiriendo con el avance longitudinal.

#### 3. Sensor Derecho (`0x29`) -> Estado: Precaución / Muro Lateral (`394 mm`)
Las zonas ROI activas se colorean de manera homogénea en **Naranja**, registrando lecturas constantes de $\sim 395\text{ mm} - 400\text{ mm}$.
* **Acción del Robot:** El robot detecta de forma geométrica el muro del lado derecho a una distancia segura de transición. 

### 🏎️ Conclusión del Diagnóstico de Conducción
Al fusionar las tres lecturas filtradas por el horizonte, el algoritmo determina que el robot está navegando en un pasillo donde el lado izquierdo está muy cerca ($83\text{ mm}$) y el derecho ofrece un margen intermedio ($394\text{ mm}$). El sistema ordena al **motor mediano EV3** girar sutilmente hacia la derecha para centrarse en el pasillo libre de $1.2\text{ metros}$ detectado por el sensor central, estabilizando la trayectoria de forma predictiva.

---
# 🧠 Avances y Errores

### Caso de Estudio: Resolución de Conflictos de Bus I²C en Sensores Láser VL53L5CX

#### 1. El Desafío de Hardware (Contexto)
Para lograr una visión tridimensional del entorno, el diseño del robot requería conectar **tres sensores de Tiempo de Vuelo (ToF) VL53L5CX** a la computadora principal (Raspberry Pi 5). Cada sensor proporciona una matriz de profundidad de $8 \times 8$ zonas, permitiendo detectar paredes y obstáculos en tiempo real. 

Para optimizar el espacio y simplificar el cableado, los tres sensores se conectaron compartiendo un único bus físico de comunicación **I²C** (pines comunes de Datos `SDA`, Reloj `SCL`, alimentación `3.3V` y Masa `GND`). Adicionalmente, el pin de control de encendido de cada sensor (`LPn` / *Low Power enable*) se conectó a un pin digital (`GPIO`) independiente de la Raspberry Pi.

#### 2. El Problema: Colisión de Direcciones en la Línea de Datos
El protocolo I²C funciona mediante un esquema Maestro-Esclavo, donde la Raspberry Pi se comunica con cada componente utilizando una **dirección lógica hexadecimal única**.

El fallo técnico ocurrió porque **todos los sensores VL53L5CX vienen configurados de fábrica con la misma dirección I²C por defecto (`0x52`)**. Al encender el robot, los tres sensores intentaban responder simultáneamente a la misma consulta de la Raspberry Pi sobre las mismas líneas físicas (`SDA`/`SCL`). Esto generó un choque de señales electrónicas (*interferencia y datos corruptos*), bloqueando por completo el bus de comunicación e impidiendo la lectura de las distancias.

[ Raspberry Pi 5 ] ─── Petición a 0x52 ───► [ Bus I²C (SDA/SCL) ]
│
┌─────────────────────────────────────┼─────────────────────────────────────┐
▼                                     ▼                                     ▼
[ Sensor 1 (0x52) ]                   [ Sensor 2 (0x52) ]                   [ Sensor 3 (0x52) ]
│                                     │                                     │
└──────── Responde al tiempo ─────────┴──────── Corrompe la señal ──────────┘


#### 3. La Solución: Secuencia de Inicialización Dinámica por Software
Para solucionar la colisión sin añadir un circuito integrado multiplexor adicional (*que sumaría peso, volumen y latencia al vehículo*), diseñamos un algoritmo de inicialización secuencial aprovechando los pines de control `LPn`:

1. **Apagado General por Hardware:** Al arrancar el sistema, la Raspberry Pi apaga los tres sensores bajando la señal de sus pines `LPn`.
2. **Encendido y Reasignación Individual:**
   * La Raspberry Pi activa únicamente el **Sensor 1** a través de su pin `LPn`.
   * Como es el único activo en el bus, escucha en la dirección `0x52`. Inmediatamente, el software le envía un comando para **cambiar su dirección en memoria volátil a `0x54`**.
   * Se repite el proceso con el **Sensor 2**, encendiéndolo y reasignando su dirección a **`0x56`**.
   * Finalmente, se activa el **Sensor 3**, manteniendo su dirección de fábrica o asignándole **`0x58`**.
3. **Lectura Multicanal Estable:** Una vez reconfigurados con direcciones únicas, el bus I²C lee los tres sensores a alta velocidad sin interferencias ni pérdida de fotogramas.

[ Paso 1: Apagar todos mediante LPn ]
[ Paso 2: Encender Sensor 1 ] ──► Cambiar dirección 0x52 ──► 0x54
[ Paso 3: Encender Sensor 2 ] ──► Cambiar dirección 0x52 ──► 0x56
[ Paso 4: Encender Sensor 3 ] ──► Mantener/Cambiar a    ──► 0x58
[ Resultado ]: Lectura simultánea y fluida de los 3 sensores en el mismo bus I²C.

#### 💡 Lección Aprendida e Impacto
Esta solución basada en firmware evitó agregar componentes de hardware extra al chasis, manteniendo el circuito ligero y garantizando un tiempo de respuesta de alta velocidad para la toma de decisiones en curva.

---

### Caso de Estudio: Compilación y Despliegue del Modelo YOLO en el Acelerador NPU Hailo-8L

#### 1. El Desafío de Software y Visión (Contexto)
Para clasificar los pilares rojos y verdes en tiempo real sin saturar el procesamiento central de la Raspberry Pi 5, delegamos las tareas de Visión Computacional a un acelerador de red neuronal (*NPU*) **Hailo-8L** conectado mediante el bus PCIe. 

El modelo de detección de objetos, entrenado previamente bajo la arquitectura YOLO y guardado originalmente en formato PyTorch (`.pt`), debía ser optimizado, cuantizado y compilado hacia el formato nativo ejecutable del hardware de Hailo: el archivo **HEF** (*Hailo Executable Format*). Para esta conversión se utilizó la herramienta oficial *Hailo Dataflow Compiler* (DFC) en la computadora de desarrollo (*Host PC*).

#### 2. El Problema: Incompatibilidad de ABI y Bloqueo de Ejecución
Durante las pruebas de despliegue en el robot, la Raspberry Pi 5 rechazó el archivo `.hef` compilado, arrojando un error fatal e impidiendo el inicio del pipeline de navegación por cámara.

El diagnóstico confirmó que no existía ningún fallo en los pesos de la red ni en la arquitectura YOLO, sino una **incompatibilidad estricta de ABI** (*Application Binary Interface*) en la pila de software de Hailo:
* **Falta de Retrocompatibilidad:** A diferencia de marcos de trabajo convencionales como ONNX o TensorFlow Lite, el ecosistema de Hailo exige una simetría exacta de versiones entre el compilador de la computadora central y el motor de ejecución (*Runtime*) del chip destino.
* **Desfase de Entornos:** El entorno virtual de la computadora de desarrollo tenía instalado una versión más reciente del compilador Hailo DFC. El archivo `.hef` resultante quedó "firmado" bajo las especificaciones de esta versión superior.
* **Bloqueo del Driver (HailoRT):** La Raspberry Pi 5 ejecutaba una versión previa y estable del driver **HailoRT** (*Hailo Runtime*, integrado con `libcamera`). Al detectar que el modelo provenía de una versión de compilador no soportada, el sistema operativo bloqueó la carga del modelo en el acelerador PCIe para prevenir corrupción de memoria o comportamientos erráticos.

  
  [ Host PC (DFC v2.X - Nuevo) ] ──► Compila modelo YOLO ──► Genera archivo .hef (v2.X)
│
▼
[ Raspberry Pi 5 (HailoRT v1.X - Estable) ] ◄──── Intenta cargar .hef
│
▼
❌ [ ERROR DE ABI ]: Rechazo por choque de versiones de software / Firma Incompatible

#### 3. La Solución: Sincronización Estricta de Versiones (*Downgrade*)
Para resolver el bloqueo sin desestabilizar la instalación de Linux y `libcamera` en la Raspberry Pi 5, ajustamos el entorno del servidor de desarrollo al estado del hardware destino:

1. **Reversión de Versión (*Downgrade*):** Desinstalamos la versión más reciente del *Hailo Dataflow Compiler* en la computadora principal e instalamos exactamente la versión equivalente que coincidía con la compilación del driver HailoRT activo en la Raspberry Pi 5.
2. **Re-ejecución del Pipeline de Compilación:** Volvimos a procesar el modelo `.pt` dentro del nuevo entorno sincronizado, regenerando el archivo `.hef` con la firma de ABI correcta.
3. **Despliegue Exitoso:** El nuevo binario fue aceptado de inmediato por el acelerador Hailo-8L, permitiendo ejecutar inferencias de visión artificial a **más de 30 FPS** sin sobrecargar la CPU de la Raspberry Pi.

[ Entorno de Desarrollo ] ──► Ajuste de versión (Downgrade) ──► Sincronización con HailoRT Pi 5
│
[ Modelo YOLO (.pt) ] ────► Re-compilación con DFC alineado ───► Nuevo binario (.hef)
│
▼
✔️ [ DESPLIEGUE EXITOSO ]: Inferencia en NPU Hailo-8L a >30 FPS con consumo mínimo de CPU

#### 💡 Lección Aprendida e Impacto
En sistemas integrados de alto rendimiento (*Edge AI*), la estabilidad depende tanto del diseño del código como del control estricto de las dependencias del entorno. Aprendimos a mantener entornos virtuales de desarrollo idénticos a las versiones del sistema operativo del robot, garantizando compilaciones fluidas y evitándonos retrasos de despliegue en competencia.


---

### Caso de Estudio: Conflicto de Protocolo PMIC en Módulo UPS y Solución por Relé

#### 1. El Desafío de Energía (Contexto)
Para asegurar el suministro ininterrumpido de energía a la Raspberry Pi 5 y sus periféricos de alto consumo (NPU Hailo-8L, AI Camera y sensores ToF), integramos un módulo **UPS** (*Uninterruptible Power Supply*) alimentado por un banco de celdas de litio 18650. La meta era aislar la electrónica sensible de los picos de voltaje e interferencias generados por los motores de tracción.

#### 2. El Problema: Incompatibilidad del Protocolo de Encendido (*Soft-Start*)
Al integrar el módulo UPS al circuito general del robot, descubrimos que la tarjeta no podía encenderse mediante un interruptor de retención estándar (*switch ON/OFF tradicional*).

Tras realizar pruebas de laboratorio sobre el puerto de control JST del UPS, diagnosticamos que el circuito integrado de gestión de energía (**PMIC**) del módulo operaba mediante un **protocolo de encendido por pulso prolongado** (*Soft-Start*):
* **Requisito de Conmutación:** El circuito del conector JST requería cerrarse de forma continua durante un intervalo de **3 a 5 segundos** y abrirse inmediatamente después para iniciar la secuencia de arranque (*booting*) de la Raspberry Pi 5.
* **Conflicto del Switch Tradicional:** Si se utilizaba un interruptor físico estándar, la línea permanecía cerrada indefinidamente. La lógica del PMIC interpretaba este contacto permanente como una orden de **apagado forzado** (*Force Shutdown*) o entraba en un bucle infinito de reinicios, dejando al robot inoperativo para la competencia.

  [ Switch Físico Tradicional (Cerrado Permanente) ] ──► PMIC del UPS ──► Interpretado como "Hard Reset"
│
▼
❌ Bucle de Reinicios / Apagado

#### 3. La Solución: Adaptación de Señal y Emulación de Pulso por Relé
Para cumplir con la normativa de la WRO (que exige un arranque limpio e inmediato del vehículo) sin manipular manualmente la placa interna, rediseñamos la etapa de control integrando un **módulo de relé electrónico**:

1. **Aislamiento Galvánico:** Desconectamos el puerto JST del mando manual y lo cableamos directamente a los contactos normalmente abiertos (NO) del relé.
2. **Emulación del Pulso de Encendido:** La bobina de control del relé se energiza mediante el circuito principal del vehículo. Un temporizador lógico en la etapa de potencia mantiene activo el relé durante el tiempo exacto que requiere el PMIC ($\sim 4\text{ s}$) y luego abre el contacto automáticamente.
3. **Arranque Seguro y Repetible:** El relé emula mecánicamente el "toque" prolongado exacto que necesita el UPS para despertar a la Raspberry Pi 5, liberando la línea a tiempo para evitar el corte por sobre-contacto.

[ Encendido General ] ──► Activa Temporizador/Relé ──► Cierra contacto JST (3 a 5 seg)
│
▼
[ Secuencia Terminada ] ◄── Abre contacto por hardware ◄── PMIC Inicia la Raspberry Pi 5
│
▼
✔️ [ ENERGÍA ESTABLE ]: Arranque automatizado, repetible y seguro para competencia

#### 💡 Lección Aprendida e Impacto
Mediante la caracterización empírica del puerto JST y la implementación del relé como adaptador de señal, resolvimos una incompatibilidad crítica entre componentes de potencia sin reemplazar hardware ni añadir circuitos complejos de estado sólido. El sistema garantiza un encendido robusto y confiable en pista con solo presionar el switch principal del vehículo.





---


# Codigo del Robot/Solución de problemas



```python

```


---

# Videos del Primer Desafio y Segundo Desafio

Video Desafio Abierto Futuros Ingenieros WRO 2025 https://youtu.be/I2WFhmv6V5k
Video Desafio Abierto 2 Futuros Ingenieros WRO 2026 https://www.youtube.com/watch?v=3iQoEDr1jIw
