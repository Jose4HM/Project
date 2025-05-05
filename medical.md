   # Papers relacionados

   ### [Respiratory and Heart Rate Detection Using Continuous-Wave Radar Testbed Implemented in GNURadio](https://pubs.gnuradio.org/index.php/grcon/article/download/125/105/)

   #### Detalles
   - Hardware: USRP Ettus X310
   - Frecuencias: 4 GHz (transmitida) y 4 MHz (Muestreo), efecto Doppler, antena bi-estática (emisor y receptor), 
   - Software: GNUradio, Matlab, Python
   - Resultados: ±5 BPM, 2 metros de distancia, 2 minutos. Toma muestras cada 90s.
   - Posibles mejoras: Precisión en la lectura en diferentes ambientes, procesamiento en tiempo real (se hace le post procesamiento en matlab) desde GNU radio (se usa python actualmente), 
   ### [A Noncontact Vital Signs (NCVS) System for Potential Patient Monitoring Enabled by Robust Software Defined Radio (SDR)](https://www.researchgate.net/publication/358697763_A_Noncontact_Vital_Signs_NCVS_System_for_Potential_Patient_Monitoring_Enabled_by_Robust_Software_Defined_Radio_SDR)/[A Feasibility Study of Remote Non-Contact Vital Signs (NCVS) Monitoring in a Clinic Using a Novel Sensor Realized by Software-Defined Radio (SDR)](https://www.mdpi.com/2079-6374/13/2/191)

   #### Detalles
   - Hardware: Sistema basado en NI USRP-2901, acompañado de antenas de dipolo logarítmico de banda ancha con una ganancia de 6 dBi, diseñadas para operar en la banda de 2.4 GHz.
   
   - Frecuencia de operación: 2.4 GHz en modo full duplex, sin el uso de un aislador.
   
   - Resultados: La medición de distancia efectiva fue de 1.3 metros, logrando una precisión en la detección de la frecuencia cardíaca y respiratoria con un error promedio de ±3 BPM.
   
   - Mejoras respecto a trabajos anteriores: Se utilizó una arquitectura Low-IF en lugar de Zero-IF para reducir significativamente el ruido 1/f (ruido de desplazamiento de frecuencia baja), y se implementó un control automático de ganancia para optimizar la señal recibida y mejorar la precisión del monitoreo.
   
   - Condiciones experimentales: Las pruebas se realizaron a una distancia de aproximadamente 60 cm entre el sensor y el sujeto.


   ### [Software-Defined Doppler Radar Sensor for Human Breathing Detection](https://www.mdpi.com/1424-8220/19/14/3085)

   #### Detalles
   - Hardware: Radas Doppler, CW (onda continua) con receptor en I/Q, NI USRP-2920, usa Low-IF, antena transmisora (dipolo vertical) y receptora (antenna omnidireccional)
   - Condiciones: Distancia de 80cm
   - Mejoras: Tiempo real usando LabView.

   ### [SDR-based Radar for Human Detection](https://www.academia.edu/95620901/SDR_based_Radar_for_Human_Detection)

   #### Detalles
   - Hardware: SDR HackRF One, Sintetizador RF programable (ADF4351), gestionado a través de un microcontrolador Arduino que comunica por protocolo I2C, antenas Log-Periodicas y Vivaldi, operando en frecuencias cercanas a los 4.100 MHz
   
   - Frecuencia: La transmisión se realiza en modo CW (onda continua), debido a que las distancias cortas (alrededor de 2 metros) generan tiempos de ida y vuelta muy cortos (~13 ns), lo que impide el uso de pulsos.
   
   - La distancia máxima detectada en espacios abiertos fue de aproximadamente 9 metros.

- Las antenas estaban separadas 40 cm para evitar acoplamiento cercano y fenómenos de máximos secundarios.

- La detección de movimiento se realiza mediante análisis de variaciones en la amplitud, sin necesidad de emplear tecnología Doppler, debido a las limitaciones del SDR utilizado.

- La medición fue efectiva en detectar la presencia y movimiento de humanos en diferentes escenarios.


- Se propuso la futura utilización de aprendizaje automático para mejorar la clasificación de los movimientos y detectar específicamente actividad humana.