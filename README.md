# odoo-install-requirements

Script para buscar e instalar dependencias de módulos Odoo de forma automática.

## Requisitos

- Python 3.6 o superior
- pip
- **No requiere librerías externas** (usa solo módulos estándar)

## Instalación

### 1. Clonar el repositorio

Script para buscar e instalar dependencias de módulos Odoo de forma automática.

## Requisitos

- Python 3.6 o superior
- pip
- **No requiere librerías externas** (usa solo módulos estándar)

## Instalación

### 1. Clonar el repositorio

```bash
git clone <url-del-repositorio>
cd odoo-requirements-installer
```

### 2. Copiar el script a la raíz de Odoo

```bash
cp install_reqs.py /ruta/de/tu/odoo/
```

## Uso

### Paso 1: Activar el entorno virtual

```bash
# Si ya existe el entorno virtual
cd /ruta/de/tu/odoo
source venv/bin/activate

# Si NO existe, créalo primero
python3 -m venv venv
source venv/bin/activate
```

### Paso 2: Ejecutar el script

```bash
python3 install_reqs.py
```
Paso 3: Revisar e instalar
El script mostrará las dependencias encontradas y preguntará:
Buscando requirements.txt desde: /opt/odoo/17_8017
  Encontrado: .../Nomina_base/requirements.txt
  Encontrado: .../Facturacion_base/requirements.txt

6 dependencias únicas:
  • PyMuPDF
  • pyOpenSSL
  • unidecode
  • validators
  • xades

¿Instalar? (s/N):
Escribe s y presiona Enter.
Paso 4: Iniciar Odoo
