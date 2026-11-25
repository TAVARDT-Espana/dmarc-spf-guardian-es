# Guardián DMARC, SPF y DKIM

[![Licencia: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Auditoria Tecnica](https://img.shields.io/badge/TAVARDT-Seguridad%20Correo-5b3cf5.svg)](https://tools.tavardt.com/es/verificador-dmarc-correo/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Auditoría de registros DNS de correo para prevención de suplantación, phishing y cumplimiento del Esquema Nacional de Seguridad (ENS) y CCN-CERT.

Desarrollado y mantenido por la division de ciberseguridad e infraestructura de **TAVARDT**.

***

## Funcionalidades y Verificaciones

* **Validacion de Politica DMARC**: Inspeccion de directivas de proteccion (reject, quarantine y none), alineacion de subdominios (sp) y porcentaje de aplicacion (pct).
* **Auditoria de Registros SPF**: Verificacion de mecanismos autorizados, limite de consultas DNS y calificadores estrictos (-all vs ~all).
* **Comprobacion de Firma DKIM**: Validacion de claves publicas configuradas en selectores DNS especificos.
* **Mecanismos de Informes**: Chequeo de parametros de envio de informes agregados y forenses (rua y ruf).
* **Alineacion Normativa**: Estructurado de acuerdo con el Guías de Seguridad CCN-STIC del CCN-CERT y Esquema Nacional de Seguridad (ENS).

***

## Instalacion y Ejecucion

Requiere unicamente Python 3.8 o superior, utilizando exclusivamente modulos estandar sin dependencias externas.

```bash
git clone https://github.com/TAVARDT-Espana/dmarc-spf-guardian-es.git
cd dmarc-spf-guardian-es
python guardian.py empresa.es
```

Para verificar un selector DKIM especifico o generar salida en formato JSON:

```bash
python guardian.py empresa.es -selector mail -json
```

***

## Diagnostico Completo en la Web

Para auditorias corporativas continuas con interfaz grafica, utilice la herramienta oficial:

* **Verificador DMARC y Autenticacion de Correo**
* **[Portal Corporativo TAVARDT](https://ag.tavardt.com/es/)**

***

## Soporte y Consultoria Especializada

Para proyectos corporativos de ciberseguridad y proteccion de infraestructura en Espana, contacte al equipo de **TAVARDT**.

***

## Enlaces Útiles

* **Portal Corporativo:** https://ag.tavardt.com/es/
* **Suite de Diagnósticos:** https://tools.tavardt.com/es/
* **Contacto Técnico:** https://ag.tavardt.com/es/contacto/

***

### Licencia
Distribuido bajo la Licencia MIT. Consulte el archivo [LICENSE](LICENSE) para más detalles.

***

© 2026 TAVARDT. Todos los derechos reservados.
