# zhiweidoushu
docker run -p 6333:6333 -p 6334:6334    -v "$(pwd)/qdrant_storage:/qdrant/storage:z"    qdrant/qdrant
docker pull arizephoenix/phoenix:latest
docker run -p 6006:6006 -p 4317:4317 arizephoenix/phoenix:latest

uv run uvicorn rag_api:app --reload --host 0.0.0.0 --port 8000

# pip install rank llm