# Entrega Práctica UD01 · Auditoría y fortificación Clínica Dental Sonrisas

- **Nombre y apellidos del alumno/a:** Vega Oncala Alba
- **Grupo:** 2º SMR
- **Fecha de realización:** 24/11/2026

---

### Actividad 1 · Mecanismos y objetivos de la seguridad informática

| ID | Mecanismo | Objetivo principal (C, I, D, NR) | Física / Lógica | Activa / Pasiva | Justificación |
|:---|:---|:---:|:---:|:---:|:---|
| 1.1 | SAI servidor | Disponibilidad | Física | Pasiva | Protege la disponibilidad a los datos y la corriente cuando se va la luz |
| 1.2 | Cifrado BitLocker | Confidencialidad | Lógica | Activa | Evita el robo o acceso a los datos haciendo que estos esten cifrados |
| 1.3 | Cortafuegos perimetral | Confidencialidad | Lógica | Activa | Evita el robo o acceso a los datos mediando las conexiones |
| 1.4 | Copias de seguridad NAS | Integridad | Lógica | Pasiva | Evita la perdida completa de datos tras un daño en estos |
| 1.5 | Antivirus corporativo | Integridad | Lógica | Activa | Protege la integridad de los datos evitando la ejecucion de software malicioso |

---

### Actividad 2 · Cadena del incidente de seguridad

1. **Activos afectados:**
   - Activo 1: Base de datos de pacientes
   - Activo 2: Registros de citas de la semana siguiente
2. **Amenaza:** Atacante
3. **Vulnerabilidad y clasificación:** Sistema sin parchear, conocida sobre el software instalado
4. **Riesgo previo:** Atacantes pueden obtener privilegios de aministrador
5. **Ataque:** Ejecutó un exploit para obtener privilegios, extraer una copia de la base de datos y borrar parte del registro de citas
6. **Impacto:**
   - Impacto cuantitativo: 3.200 € en tratamientos cancelados
   - Impacto cualitativo: quejas de pacientes

---

### Actividad 3 · Plan de contingencia

1. **Clasificación de medidas:**
   - Medida A: Plan de emergencia
   - Medida B: Plan de respaldo
   - Medida C: Plan de recuperación
   - Medida D: Plan de emergencia
   - Medida E: Plan de recuperación
   - Medida F: Plan de respaldo
2. **Diferencia entre plan de respaldo y plan de recuperación:** El plan de respaldo son medidas preventivas que se aplican antes y siempre están activas, el plan de recuperación son medidas que ayudan a recuperarse tras una emergencia y a curar daños.

---

### Actividad 4 · Software malicioso y test de intrusión

#### 4.1. Diagnóstico de malware
- **Caso 1:**
  - Tipo de malware: Virus, troyano y gusano
  - Justificación (archivo anfitrión e intervención usuario): Requería de un archivo anfitrion que aparentaba ser un pdf de un presupuesto y no necesitaba intervención de usuarios para esparcirse por la red.
- **Caso 2:**
  - Tipo de malware: Gusano
  - Justificación (archivo anfitrión e intervención usuario): No se coló mediante un archivo o aparentó ser un programa legítimo, pero se esparció por si solo por la red.
- **Medida preventiva para Caso 2:** Siempre mantener las actualizaciones del SMB al día o si todavía no hay actualización publicada desactivar el sistema para anular el riesgo.

#### 4.2. Secuenciación de test de intrusión
- Secuencia ordenada cronológicamente (letras):
- Fases correspondientes:
  - Acción Búsqueda de vulnerabilidades: Fase 3
  - Acción Fingerprinting: Fase 2
  - Acción Parche/Informe: Fase 5
  - Acción Footprinting: Fase 1

---

### Actividad 5 · Contraseñas e identificación digital

#### 5.1. Contraseñas
1. **Comparativa de seguridad frente a fuerza bruta:** porque el uso de más posibles carácteres como los símbolos especiales aumenta exponencialmente el tiempo que se tarda en conseguir la contraseña mediante fuerza bruta, más que solo añadiendo un carácter extra ya que hay más combinaciones posibles que podría llegar a ser
2. **Política de contraseñas (3 reglas):**
   - Regla 1: Longitud mínima de 8 carácteres
   - Regla 2: Usar mayúsculas, minúsculas, númmeros y carácteres especiales
   - Regla 3: Evitar diccionario

#### 5.2. Identificación digital
3. **Mecanismos aplicados:**
   - Trámite A: Certificado digital, vincula una identidad verificada con una clave criptográfica y lo emite una autoridad de certificación
   - Trámite B: Firma digital, vincula a una persona con el documento y aporta autoria, integridad y no repudio
4. **Objetivo de seguridad garantizado y diferencia con usuario/contraseña:** El no repudio, este asegura que alguien ha tenido una participación verificable y evita que digan que no han sido ellos ya sea con un certificado digital o una firma electrónica, cosa que no se puede asegurar solo con un usuario y contraseña simple.