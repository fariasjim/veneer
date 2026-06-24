# Veneer 🚀

Veneer is a remote-accessible database management and admin panel application built entirely using Python (FastAPI). Designed around absolute data portability, it hooks into local or remote relational databases by importing an external, human-readable configuration workspace file (`*.json`), transforming structural schemas into a functional dashboard.

## 🎯 Architecture Pillars

* **Decoupled Data Portability:** Workspaces are fully portable. A single configuration file contains database credentials, access locations, and frontend layouts. Swapping environments or loading an alternate database is as simple as importing another workspace configuration file.
* **Agile Engine Execution Strategy:** Built on a production-ready template from day one, features like fluid user-level drag-and-drop dashboard saving, detailed chart formatting handlers, and load-shedding resource gates are cleanly separated into Phase 2 execution branches.
* **Cooperative I/O Flow Control:** Database resource saturation is avoided by streaming large read tables through chunked generator loops using `await asyncio.sleep(0)`, naturally allowing high-priority updates to process without stalling.

---

## 🗺️ Engineering Development Blueprint

### Phase 1: Portable Configuration Engine & Connection Routing

* [ ] Construct the modular FastAPI core, custom exception handlers, and dynamic state routers.
* [ ] Define declarative Pydantic schemas validating external imported workspace layouts (`.json`).
* [ ] Build runtime engine hot-swapping drivers managing connection pools dynamically across local files or remote hosts.
* [ ] Write cooperative chunk-by-chunk dataset generators utilizing explicit event-loop execution slicing.

### Phase 2: Variable Schema Introspection Drivers

* [ ] Program type-agnostic system schema reflectors capable of querying engine structures (SQLite `PRAGMA` vs. standard SQL `information_schema`).
* [ ] Code deep introspection rules mapping column states, primary identities, and relational foreign definitions.
* [ ] Expose dynamic reflection topologies via the unified `/api/v1/introspect/schema` runtime path.

### Phase 3: Universal Dynamic CRUD Implementation

* [ ] Build streaming read APIs with native cursor limits, filtering arrays, and step pagination.
* [ ] Deploy dynamic parameter data-type enforcement checking input variables against database schemas.
* [ ] Code uniform write, point update, and removal pipelines mapped cleanly to the underlying query router.

### Phase 4: Manifest Updates & Container Packaging

* [ ] Build export endpoints (`/api/v1/workspace/export`) to serialize layout changes directly back into the imported file path.
* [ ] Setup coordinate canvas data schemas ($X, Y, W, H$) to natively support modular dashboard objects.
* [ ] Formulate multi-stage Docker configurations mapping external volume definitions to host storage paths.

---

## 🛠️ Technology Stack Definition

* **System Application Brain:** Python (FastAPI Engine)
* **Concurrency Architecture:** Cooperative Asyncio Data Generators (`yield`)
* **Connection Orchestration:** SQLAlchemy Dynamic Core Drivers
* **Workspace Manifest Specification:** Portable Independent Profile Schemes (`workspace.config.json`) veneer

