
# Lab Statement: Introduction to Creating RAGs (Retrieval-Augmented Generators) with OpenAI

# RAG con Gemini y Pinecone


Este proyecto implementa un sistema básico de Recuperación Aumentada con Generación (RAG) utilizando Google Gemini para embeddings y Pinecone como vector database. El flujo completo se ejecuta dentro de un Jupyter Notebook.

Construir un pipeline RAG funcional que permita:

- Convertir texto en embeddings
- Guardar embeddings en Pinecone
- Recuperar información por similitud
- Preparar el vector store para integrarlo con un modelo generativo

---

## Tecnologías utilizadas

- Google Gemini (gemini-embedding-001) para generar embeddings
- Pinecone para almacenar y consultar vectores
- LangChain
- Python 3.10
- Jupyter Notebook

---

## Estructura del proyecto

```
Rag-project
!--RAG_Pinecone.ipynb
!--README.md
!--.env
```

---

## Archivo .env

Se debe crear un archivo `.env` con el siguiente contenido:

```
GOOGLE_API_KEY=tu_api_key_de_gemini
PINECONE_API_KEY=tu_api_key_de_pinecone
```


---

## Instalación de dependencias

Instalar dependencias manualmente:

```
pip install langchain langchain-google-genai langchain-pinecone pinecone-client python-dotenv tqdm
```


---

## Ejecución del proyecto

1. Clonar el repositorio o copiar los archivos del proyecto.
2. Crear el archivo `.env` con las credenciales.
3. Abrir Jupyter Notebook:
4. Abrir y ejecutar `rag_gemini_pinecone.ipynb` celda por celda.

---

## Flujo del Notebook

El notebook incluye las siguientes etapas:

1. Instalación y carga de librerías
2. Carga de credenciales desde `.env`
3. Inicialización del cliente Pinecone
4. Creación del índice con dimensión 3072
5. Configuración del modelo de embeddings Gemini
6. Configuración del vector store conectado al índice
7. Inserción de documentos
8. Consulta por similitud
9. Creación del retriever

---



---
### Julian Santiago Cardenas Cubaque