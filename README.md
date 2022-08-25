# ArgenCon-2022-SizingTool-Data

El actual repositorio contiene los parámetros en serie temporal utilizados para los casos de estudio del artículo titulado: "Herramienta para el dimensionamiento ́optimo de microrredes hıbridas PV/Baterıas/Viento/Diesel e inversores hıbridos" para la conferencia **ArgenCon 2022**. Los parámetros citados se pueden encontrar con la información dada a continuación:

### Sets
- Tecnologías de módulos fotovoltaicos $G$ : [Sunergy-370W, Luxen-450W]
- Tecnologías de baterías $B$ : [PylonTech-UP5000, NCL-50Ah]
- Tecnologías de inversores híbridos $I$ : [InfiniSolar Plus 5kW, NCL-5kW]
- Tecnologías de turbinas eólicas $W$ : [FK-3kW, FX-400, FX-1000]


### Datos meteorológicos temporales en la ciudad de Puerto Carreño, Vichada:
- Irradiancia global Horizontal en $W/m^2$ ( $GHI_t$ ): Archivo: **MeteoData.csv**, Columna: **GHI_PC** 
- Temperatura medida a 2m en °C ( $tem_{t}^{a} )$: Archivo: **MeteoData.csv**, Columna: **TEM_PC**
- Velocidad del viento medida a 2m en m/s ( $WS_t$ ): Archivo: **MeteoData.csv**, Columna: **WS_PC**

### Generación renovable calculada con datos meteorológicos de Puerto Carreño, Vichada:
- Generación fotovoltaica de cada módulo del set $G$ calculada según los modelos [1], [2] ( $P^{PV_{gen}}_{g,t}$ ) : Archivo: **GEN_PV_PC.csv**
- Generación eólica de por cada turbina del set $W$ calculada según el modelo [3] ( $P_{w,t}^{WT_{gen}}$ ) : Archivo: **GEN_WT_PC.csv**


### Datos meteorológicos temporales en la isla de San Andrés:
- Irradiancia global Horizontal en $W/m^2$ ( $GHI_t$ ): Archivo: **MeteoData.csv**, Columna: **GHI_SA**
- Temperatura medida a 2m en °C ( $tem^a_t$ ): Archivo: **MeteoData.csv**, Columna: **TEM_SA**
- Velocidad del viento medida a 2m en m/s ( $WS_t$ ): Archivo: **MeteoData.csv**, Columna: **WS_SA**

### Generación renovable calculada con datos meteorológicos de la isla de San Andrés:
- Generación fotovoltaica de cada módulo del set $G$ calculada según los modelos [1], [2] ( $P^{PV_{gen}}_{g,t}$ ) : Archivo: **GEN_PV_SA.csv**
- Generación eólica de por cada turbina del set $W$ calculada según el modelo [3] ( $P_{w,t}^{WT_{gen}}$ ) : Archivo: **GEN_WT_SA.csv**

### Datos temporales usados en ambos casos de estudio
- Perfil de demanda de UCI de 175 $m^2$ en kW ( $L_t$ ): Archivo: **CaseData.csv**, Columna: **LOAD**
- Perfil de precios de compra de la red en  USD/kWh ( $C_{t}^{buy}$ ): Archivo: **CaseData.csv**, Columna: **C_BUY**
- Perfil de precios de venta de la red en USD/kWh ( $C_{t}^{sell}$ ): Archivo: **CaseData.csv**, Columna: **C_SELL**
- Perfil de disponibilidad de la red [1,0] ( $Av_{t}^{G}$ ): Archivo: **CaseData.csv**, Columna: **AV_GRID**
- Perfil de disponibilidad del generador diésel [1,0] ( $Av_{t}^{D}$ ): Archivo: **CaseData.csv**, Columna: **AV_DIESEL**


## Referencias (También utilizadas en el paper)

[1] D. A. A. Lozano, “Evaluación de la orientacion y el ángulo de inclinacion óptimo de una superficie plana para maximizar la captación de irradiación solar en cuenca-ecuador,” vol. 7, pp. 74–77, 2017.

[2] D. L. King, W. E. Boyson, and J. A. Kratochvil, “Photovoltaic array performance model, SANDIA Report SAND2004-3535,” Sandia Report No. 2004-3535, vol. 8, no. December, pp. 1–19, 2004.

[3] T. Ma and M. S. Javed, “Integrated sizing of hybrid PV-wind-battery system for remote island considering the saturation of each renewable energy resource,” Energy Conversion and Management, vol. 182, pp. 178–190, feb 2019.
