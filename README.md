# hitl2026ai

```shell
├──app
    ├── __init_.py 
    ├── main.py
    ├── config.py
    ├── api                 # Transport / API Layer
        ├── __init__.py
        ├── deps.py         # FastAPI route dependencies (Auth, DB, AgentDeps)
        ├── api.py        
        ├── endpoints          
            ├── __init__.py
            ├── router.py   # APIRouter aggregation
    ├── core                # Orchestration & Domain Logic
        ├── __init__.py
        ├── security.py
        ├── orchestrator.py # Multi-agent graph / router coordinator
        ├── agents:         # Agent Specifications
        ├── schemas:        # Shared Pydantic models (API Request/Response)
        └── models:         # Async SQLAlchemy / DB connection management
    ├── services:           # External integrations & data access layer
    └── tools:              # エージェントに持たせる外部ツール群
```
