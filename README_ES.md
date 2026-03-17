![Bash](https://img.shields.io/badge/Bash-Tool-blue)
![Nmap](https://img.shields.io/badge/Nmap-Scanner-red)
![Platform](https://img.shields.io/badge/platform-Linux-green)
![Status](https://img.shields.io/badge/status-active-brightgreen)

#  Flow4Scan – Advanced Nmap Automation & Analysis Tool

> Pipeline completo de escaneo, parsing y análisis automático orientado a ciberseguridad.

> Reconocimiento → Escaneo → Parsing → Análisis → Informe
---------------------

## 📌 Descripción

**Flow4Scan** es una herramienta avanzada que automatiza el flujo completo de auditoría de red:


Permite transformar resultados de Nmap en **información accionable**, detectando riesgos, servicios críticos y posibles vectores de ataque.

---------------------

##  Características principales

###  Automatización completa
- Ejecución de escaneos Nmap preconfigurados
- Generación automática de resultados estructurados
- Análisis de seguridad sin intervención manual

---------------------

###  Tipos de escaneo

- Fast Scan (rápido)
- Aggressive Scan (detección completa)
- Auto Port Scan (descubrimiento inteligente)
- Multi Target Scan
- Full Pro Scan (incluye análisis automático)
- UDP Scan (requiere root)
- Evasion Scan (evasión básica de firewall)

---------------------

### 📊 Output estructurado

La herramienta genera automáticamente:

| Archivo         | Descripción                |
|-----------------|----------------------------|
| `scan.xml`      | Resultado completo de Nmap |
| `services.json` | Servicios detectados       |
| `services.csv`  | Exportación CSV            |
| `summary.json`  | Resumen                    |
| `analysis.json` | Análisis de seguridad      |
| `report.md`     | Informe profesional        |
| `report.txt`    | Informe simplificado       |

---------------------

###  Análisis automático

Flow4Scan detecta:

-  Servicios críticos
-  Nivel de riesgo (LOW / MEDIUM / HIGH / CRITICAL)
-  Posibles CVEs (heurístico)
-  Vectores de ataque
-  Configuraciones inseguras

---------------------

### 📁 Organización automática

Cada escaneo genera su propia carpeta:

/output/
└── FullProScan_192.168.1.1_20260316_183000/


---------------------

##  Instalación

git clone https://github.com/tuusuario/Flow4Scan.git

cd Flow4Scan

---------------------

###  Permisos

Algunas funciones requieren root:

chmod +x Flow4Scan.sh

sudo ./Flow4Scan.sh

---------------------

🧠 Casos de uso

Pentesting básico

Auditorías internas

Reconocimiento de red

Laboratorios de ciberseguridad

Automatización de Nmap

⚠️ Limitaciones

CVEs basados en heurística

Parsing XML mejorable

No sustituye auditoría manual

🛡️ Aviso legal

Uso exclusivo para:

Auditorías autorizadas

Entornos educativos

👨‍💻 Autor

Francisco Javier Jiménez Cortés

Ciberseguridad

Desarrollo de software

DevSecOps
