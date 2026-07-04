# Architecture

Frontend → API Layer → Director AI → Scene Engine → State DB → Output Pipeline

Core concept:
- Single Source of Truth (studio_state.json)
- All AI agents read/write same memory
